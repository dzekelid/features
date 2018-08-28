swagger: "2.0"
x-collection-name: Coord
x-complete: 1
info:
  title: Users API
  description: the-users-api-allows-you-to-manage-user-data-on-the-coord-platform--sending-user-data-to-coordallows-you-to-perform-transactions-with-mobility-systems-like-renting-a-bike-parking-ina-parking-lot-or-booking-a-ridehail-trip-on-behalf-of-that-user-using-the-coord-platform-the-requirements-for-performing-a-transaction-for-a-given-user-vary-depending-on-the-systemyoure-connecting-with--some-systems-require-particular-data-about-a-user-in-order-for-thetransaction-to-take-place-and-some-systems-require-you-to-link-a-users-account--alltransactions-require-you-to-authenticate-the-user-using-a-jwt-every-coord-api-that-supports-transactions-has-an-endpoint-for-getting-information-aboutthat-apis-systems-along-with-what-you-need-to-provide-for-a-user-in-order-to-perform-atransaction-for-them--the-users-api-provides-tools-that-help-you-enable-users-to-performtransactions-as-well-as-tools-for-learning-about-the-transactions-that-a-user-can-alreadyperform-read-on-for-more-information-about-authenticating-users-linking-accounts-and-managing-userdata--authenticating-users-with-jwtsall-coord-api-endpoints-that-either-manipulate-data-or-perform-a-transaction-on-behalf-of-alogged-in-user-require-http-calls-to-include-an-authorization-bearer-jwt-token-so-thatthe-current-user-can-be-identified--all-endpoints-in-the-users-api-fall-into-this-categoryexcept-for-the-test-jwt-creation-endpoint-which-is-designed-to-allow-you-to-create-test-tokensfor-use-in-such-requests-for-information-on-how-to-create-nontest-user-authorization-tokensplease-contact-a-hrefmailtosalescoord-co-target-blanksalescoord-coaas-this-is-available-only-for-transaction-enabled-partners-see-post-v1userstestinguser-and-jwtreference0testjwtcreation-for-information-onhow-to-create-jwts-for-testing--linking-accountsmany-systems-require-you-to-link-a-user-in-order-to-perform-a-transaction--you-can-do-this-byredirecting-the-users-browser-or-webview-to-theget-v1userslink-accountreference0linkauseraccounttoenabletransactions-endpoint-this-will-allow-the-user-to-link-to-an-existing-account-with-that-system-if-they-have-one-orwill-create-a-new-one-for-them--if-you-call-this-endpoint-with-a-test-jwt-we-will-simulateaccount-linking-by-redirecting-the-user-to-a-demo-permission-page-you-can-also-simulate-linking-or-unlinking-test-users-accounts-serverside-by-calling-thepost-v1userstestingusercurrenttransactable-systemsreference0simulateaccountlinkingfortestingendpoint-remember-that-not-all-systems-are-transactable-and-not-all-transactable-systems-requireaccount-linking--getting-and-setting-user-infowe-automatically-ingest-user-information-like-email-addresses-and-names-from-the-jwtauthorization-token-you-send-us--information-about-a-users-vehicle-like-their-license-plateneeds-to-be-set-through-our-api--we-require-this-in-order-for-the-user-to-transact-with-certainparking-operators-you-can-call-get-v1usersusercurrentreference0getuserinfo-to-get-all-theinformation-we-have-about-a-user-including-the-fields-we-deduce-from-their-jwt-and-those-thatyou-have-already-set-through-our-api-you-can-call-v1usersusercurrentupdate-vehiclereference0updateuservehicle-toupdate-the-vehicle-thats-associated-with-a-users-account-
  version: 1.0.0
host: api.coord.co
basePath: /v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /location/{system_id}/{location_id}:
    get:
      summary: Get detailed information on a bike location, as a GeoJSON Feature.
      description: |-
        A bike location may be a single bike station (which can have multiple docked bikes) or a
        single dockless bike itself. All working docks are returned, but only free and rentable
        dockless bikes are returned.

        ### Example

        #### Request:
        `curl -G "https://api.coord.co/v1/bike/location/CitiBike/482?access_key="`

        #### Response:
        ```
        {
          "geometry": {
            "coordinates": [
              -73.99931783,
              40.73935542
            ],
            "type": "Point"
          },
          "id": "CitiBike-482",
          "properties": {
            "is_renting": true,
            "is_returning": true,
            "last_reported": "2018-05-17T15:41:06.000Z",
            "lat": 40.73935542,
            "location_id": "482",
            "location_type": "bike_station_dock",
            "lon": -73.99931783,
            "name": "W 15 St & 7 Ave",
            "num_bikes_available": 19,
            "num_docks_available": 19,
            "region_id": "71",
            "system_id": "CitiBike"
          },
          "type": "Feature"
        }
        ```
      operationId: get_bike_location
      x-api-path-slug: locationsystem-idlocation-id-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Detailed
      - Information
      - "On"
      - Bike
      - Location
      - ""
      - As
      - GeoJSON
      - Feature
  /system/{system_id}:
    get:
      summary: Get detailed information on a bike system, as a GeoJSON feature.
      description: |-
        Bike systems are individual bike share systems, often per-region.

        Information is returned as a GeoJSON Feature. The geometry of the GeoJSON Feature is
        a MultiPolygon that defines the system's operational area. All bike systems have an
        operational area, in which bikes may be found and parked.
        For systems that require bikes be docked, this area is somewhat arbitrary, as bikes are
        only found at stations. In this case, the operational area is roughly the city or
        jurisdiction that the system covers.
        For semi-dockless and dockless systems that allow bikes to be parked anywhere, the
        operational area is very important and strictly defined. Often there are extra fees for
        parking outside of the operational area (also known as a "catchment area"), and almost all
        bikes should be within the area.

        These bike system types are reflected in the `station_type` property.
        * `dock` - All bikes must be taken from and returned to a dock.
        * `dockless` - All bikes are only dockless.
        * `dockless_with_hub` - Bikes may be dockless, or taken from or returned to a hub.
        A hub can be an area rather than a discrete station, where a bike can be returned and
        locked but not explicitly docked. The total price of a rental may change based on whether
        a bike is returned to a hub or not.

        Areas are returned as a GeoJSON MultiPolygon since areas may be discontiguous or have
        holes.

        ### Example

        #### Request:
        `curl -G "https://api.coord.co/v1/bike/system/CitiBike?access_key="`

        #### Response:
        ```
        {
          "type": "Feature",
          "geometry": {
              "type": "MultiPolygon",
              "coordinates": [
                [
                  [ [-74.00, 40.70], [-74.00, 40.80], [-73.90, 40.80], ..., [-74.00, 40.70] ]
                ],
                ...,
                [
                  [ [-73.00, 41.70], [-73.00, 41.80], [-72.90, 41.80], ..., [-73.00, 41.70] ],
                  [ [-72.98, 41.75], [-72.98, 41.78], [-72.95, 41.78], ..., [-72.98, 41.75] ]
                ]
              ]
            },
          "id": "CitiBike",
          "properties": {
            "email": "support@coord.co",
            "phone_number": "+6789998212",
            "station_type": "dock",
            "is_transactable": "false"
          }
        }
        ```
      operationId: get_bike_system
      x-api-path-slug: systemsystem-id-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Detailed
      - Information
      - "On"
      - Bike
      - System
      - ""
      - As
      - GeoJSON
      - Feature
  /location:
    get:
      summary: Get bike locations in the requested search area, as a GeoJSON FeatureCollection.
      description: |-
        Get a list of locations given the input parameters. Specify a search area by radius around
        a latitude and longitude, as well as any filter for specific systems. Each location will
        be a GeoJSON Feature, and aggregated into a GeoJSON FeatureCollection.

        ### Example

        #### Request:
        `curl -G "https://api.coord.co/v1/bike/location?latitude=40.742868&longitude=-73.989186&radius_km=0.25&access_key="`

        #### Response:
        ```
        {
          "features": [
            {
              "geometry": {
                "coordinates": [
                  -73.98918628692627,
                  40.74286877312112
                ],
                "type": "Point"
              },
              "id": "CitiBike-3641",
              "properties": {
                "is_renting": true,
                "is_returning": true,
                "last_reported": "2018-05-17T15:39:24.000Z",
                "lat": 40.74286877312112,
                "location_id": "3641",
                "location_type": "bike_station_dock",
                "lon": -73.98918628692627,
                "name": "Broadway & W 25 St",
                "num_bikes_available": 53,
                "num_docks_available": 1,
                "region_id": "71",
                "system_id": "CitiBike"
              },
              "type": "Feature"
            },
            {
              "geometry": {
                "coordinates": [
                  -73.99144871,
                  40.74395411
                ],
                "type": "Point"
              },
              "id": "CitiBike-466",
              "properties": {
                "is_renting": true,
                "is_returning": true,
                "last_reported": "2018-05-17T15:32:40.000Z",
                "lat": 40.74395411,
                "location_id": "466",
                "location_type": "bike_station_dock",
                "lon": -73.99144871,
                "name": "W 25 St & 6 Ave",
                "num_bikes_available": 35,
                "region_id": "71",
                "system_id": "CitiBike"
              },
              "type": "Feature"
            }
          ],
          "type": "FeatureCollection"
        }
        ```
      operationId: search_locations
      x-api-path-slug: location-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: latitude
        description: Latitude to return results for
      - in: query
        name: longitude
        description: Longitude to return results for
      - in: query
        name: radius_km
        description: Distance, in kilometers, from (latitude, longitude) we will return
          results for
      - in: query
        name: system_ids
        description: Comma separated list of the bike system IDs to include in the
          search
      responses:
        200:
          description: OK
      tags:
      - Bike
      - Locations
      - In
      - Requested
      - Search
      - Area
      - ""
      - As
      - GeoJSON
      - FeatureCollection
  /system:
    get:
      summary: Get information on all bike systems in an area, as a GeoJSON FeatureCollection.
      description: |-
        Bike systems are individual bike share systems, often per-region.

        Information about each system is returned as a GeoJSON Feature, within a single GeoJSON
        FeatureCollection.

        See the [/system/{system_id}](#reference/0/get-information-for-a-bike-system) call for more
        details on the individual system Features.

        ### Example

        #### Request:
        `curl -G "https://api.coord.co/v1/bike/system?latitude=40.74286877312112&longitude=-73.98918628692627&radius_km=0.5&access_key="`

        #### Response:
        ```
        {
          "features": [
            {
              "geometry": {
                "coordinates": [
                  [
                    [
                      [
                        -74.055701,
                        40.707838
                      ],
                      [
                        -74.083639,
                        40.714807
                      ],
                      ...,
                      [
                        -74.055701,
                        40.707838
                      ]
                    ]
                  ]
                ],
                "type": "MultiPolygon"
              },
              "id": "CitiBike",
              "properties": {
                "is_transactable": true,
                "station_type": "dock"
              },
              "type": "Feature"
            }
          ],
          "type": "FeatureCollection"
        }
        ```
      operationId: search_bike_systems
      x-api-path-slug: system-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: latitude
        description: Latitude to return results for
      - in: query
        name: longitude
        description: Longitude to return results for
      - in: query
        name: radius_km
        description: Distance, in kilometers, from (latitude, longitude) we will return
          results for
      responses:
        200:
          description: OK
      tags:
      - Information
      - "On"
      - ""
      - Bike
      - Systems
      - In
      - Area
      - ""
      - As
      - GeoJSON
      - FeatureCollection
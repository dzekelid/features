---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Featured Users Featured User
  description: Retrieves a FeaturedUser by id.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /homepages/pickers/{featured_listing_picker_id}:
    get:
      summary: Get Homepages Pickers Featured Listing Picker
      description: Retrieves a FeaturedListingPicker by id.
      operationId: getHomepagesPickersFeaturedListingPicker
      x-api-path-slug: homepagespickersfeatured-listing-picker-id-get
      parameters:
      - in: path
        name: featured_listing_picker_id
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
  /homepages/pickers/{featured_listing_picker_id}/featured:
    get:
      summary: Get Homepages Pickers Featured Listing Picker Featured
      description: Retrieves a set of FeaturedListing objects associated to a FeaturedListingPicker.
      operationId: getHomepagesPickersFeaturedListingPickerFeatured
      x-api-path-slug: homepagespickersfeatured-listing-picker-idfeatured-get
      parameters:
      - in: path
        name: featured_listing_picker_id
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
      - Featured
  /homepages/pickers/{featured_listing_picker_id}/listings:
    get:
      summary: Get Homepages Pickers Featured Listing Picker Listings
      description: Retrieves a set of Listing objects associated to a FeaturedListingPicker.
      operationId: getHomepagesPickersFeaturedListingPickerListings
      x-api-path-slug: homepagespickersfeatured-listing-picker-idlistings-get
      parameters:
      - in: path
        name: featured_listing_picker_id
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
      - Listings
  /homepages/pickers/{featured_listing_picker_id}/listings/active:
    get:
      summary: Get Homepages Pickers Featured Listing Picker Listings Active
      description: Retrieves a set of Listing objects associated to a FeaturedListingPicker
        in scope active.
      operationId: getHomepagesPickersFeaturedListingPickerListingsActive
      x-api-path-slug: homepagespickersfeatured-listing-picker-idlistingsactive-get
      parameters:
      - in: path
        name: featured_listing_picker_id
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
      - Listings
      - Active
  /homepages/listings/{featured_listing_id}:
    get:
      summary: Get Homepages Listings Featured Listing
      description: Retrieves a FeaturedListing by id.
      operationId: getHomepagesListingsFeaturedListing
      x-api-path-slug: homepageslistingsfeatured-listing-id-get
      parameters:
      - in: path
        name: featured_listing_id
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
      - Featured
      - Listing
  /homepages/listings/{featured_listing_id}/picker:
    get:
      summary: Get Homepages Listings Featured Listing Picker
      description: Retrieves a set of FeaturedListingPicker objects associated to
        a FeaturedListing.
      operationId: getHomepagesListingsFeaturedListingPicker
      x-api-path-slug: homepageslistingsfeatured-listing-idpicker-get
      parameters:
      - in: path
        name: featured_listing_id
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
      - Featured
      - Listing
      - Picker
  /homepages/listings/{featured_listing_id}/listing:
    get:
      summary: Get Homepages Listings Featured Listing Listing
      description: Retrieves a set of Listing objects associated to a FeaturedListing.
      operationId: getHomepagesListingsFeaturedListingListing
      x-api-path-slug: homepageslistingsfeatured-listing-idlisting-get
      parameters:
      - in: path
        name: featured_listing_id
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
      - Featured
      - Listing
      - Listing
  /shops/{shop_id}/listings/featured:
    get:
      summary: Get Shops Shop Listings Featured
      description: Retrieves Listings associated to a Shop that are featured
      operationId: getShopsShopListingsFeatured
      x-api-path-slug: shopsshop-idlistingsfeatured-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: shop_id
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Listings
      - Featured
  /featured/users:
    get:
      summary: Get Featured Users
      description: Finds all FeaturedUser.
      operationId: getFeaturedUsers
      x-api-path-slug: featuredusers-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      responses:
        200:
          description: OK
      tags:
      - Featured
      - Users
  /featured/users/{featured_user_id}:
    get:
      summary: Get Featured Users Featured User
      description: Retrieves a FeaturedUser by id.
      operationId: getFeaturedUsersFeaturedUser
      x-api-path-slug: featuredusersfeatured-user-id-get
      parameters:
      - in: path
        name: featured_user_id
      responses:
        200:
          description: OK
      tags:
      - Featured
      - Users
      - Featured
      - User
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---
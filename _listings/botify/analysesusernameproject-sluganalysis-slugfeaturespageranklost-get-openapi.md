---
swagger: "2.0"
x-collection-name: Botify
x-complete: 0
info:
  title: Botify Get Analyses Username Project Slug Analysis Slug Features Pagerank
    Lost
  description: Get analyses username project slug analysis slug features pagerank
    lost.
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/features/ganalytics/orphan_urls/{medium}/{source}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Ganalytics
        Orphan Urls Medium Source
      description: 'Legacy    List of Orphan URLs. URLs which generated visits from
        the selected source according to Google Analytics data, but were not crawled
        with by the Botify crawler (either because no links to them were found on
        the website, or because the crawler was not allowed to follow these links
        according to the project settings).   For a search engine (medium: origanic;
        sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social
        network (medium: social; sources: all, facebook, google+, linkedin, pinterest,
        reddit, tumblr, twitter)'
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesGanalyticsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesganalyticsorphan-urlsmediumsource-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Ganalytics
      - Orphan
      - Urls
      - Medium
      - Source
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Ganalytics
        Orphan Urls Medium Source
      description: Parameters analyses username project slug analysis slug features
        ganalytics orphan urls medium source.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesGanalyticsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesganalyticsorphan-urlsmediumsource-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Ganalytics
      - Orphan
      - Urls
      - Medium
      - Source
  /analyses/{username}/{project_slug}/{analysis_slug}/features/links/percentiles:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Links Percentiles
      description: Get analyses username project slug analysis slug features links
        percentiles.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesLinksPercentiles
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeatureslinkspercentiles-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Links
      - Percentiles
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Links
        Percentiles
      description: Parameters analyses username project slug analysis slug features
        links percentiles.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesLinksPercentiles
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeatureslinkspercentiles-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Links
      - Percentiles
  /analyses/{username}/{project_slug}/{analysis_slug}/features/pagerank/lost:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Pagerank
        Lost
      description: Get analyses username project slug analysis slug features pagerank
        lost.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesPagerankLost
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturespageranklost-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Pagerank
      - Lost
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Pagerank
        Lost
      description: Parameters analyses username project slug analysis slug features
        pagerank lost.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesPagerankLost
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturespageranklost-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Pagerank
      - Lost
  /analyses/{username}/{project_slug}/{analysis_slug}/features/sitemaps/report:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Sitemaps
        Report
      description: Get global information of the sitemaps found (sitemaps indexes,
        invalid sitemaps urls, etc.)
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsReport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapsreport-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Report
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Sitemaps
        Report
      description: Parameters analyses username project slug analysis slug features
        sitemaps report.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsReport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapsreport-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Report
  /analyses/{username}/{project_slug}/{analysis_slug}/features/sitemaps/samples/out_of_config:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Out Of Config
      description: Sample list of URLs which were found in your sitemaps but outside
        of the crawl perimeter defined for the project, for instance domain/subdomain
        or protocol (HTTP/HTTPS) not allowed in the crawl settings.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesOutOfConfig
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplesout-of-config-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Out
      - Of
      - Config
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Out Of Config
      description: Parameters analyses username project slug analysis slug features
        sitemaps samples out of config.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesOutOfConfig
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplesout-of-config-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Out
      - Of
      - Config
  /analyses/{username}/{project_slug}/{analysis_slug}/features/sitemaps/samples/sitemap_only:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Sitemap Only
      description: Sample list of URLs which were found in your sitemaps, within the
        project allowed scope (allowed domains/subdomains/protocols), but not found
        by the Botify crawler.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesSitemapOnly
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplessitemap-only-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Sitemap
      - Only
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Sitemap Only
      description: Parameters analyses username project slug analysis slug features
        sitemaps samples sitemap only.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesSitemapOnly
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplessitemap-only-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Sitemap
      - Only
  /analyses/{username}/{project_slug}/{analysis_slug}/features/top_domains/domains:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Top Domains
        Domains
      description: Get analyses username project slug analysis slug features top domains
        domains.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsDomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainsdomains-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Domains
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Top
        Domains Domains
      description: Parameters analyses username project slug analysis slug features
        top domains domains.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsDomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainsdomains-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Domains
  /analyses/{username}/{project_slug}/{analysis_slug}/features/top_domains/subdomains:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Top Domains
        Subdomains
      description: Get analyses username project slug analysis slug features top domains
        subdomains.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsSubdomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainssubdomains-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Subdomains
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Top
        Domains Subdomains
      description: Parameters analyses username project slug analysis slug features
        top domains subdomains.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsSubdomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainssubdomains-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Subdomains
  /analyses/{username}/{project_slug}/{analysis_slug}/features/visits/orphan_urls/{medium}/{source}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Visits Orphan
        Urls Medium Source
      description: 'List of Orphan URLs. URLs which generated visits from the selected
        source according to Google Analytics data, but were not crawled with by the
        Botify crawler (either because no links to them were found on the website,
        or because the crawler was not allowed to follow these links according to
        the project settings).   For a search engine (medium: origanic; sources: all,
        aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium:
        social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr,
        twitter)'
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesVisitsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesvisitsorphan-urlsmediumsource-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Visits
      - Orphan
      - Urls
      - Medium
      - Source
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Visits
        Orphan Urls Medium Source
      description: Parameters analyses username project slug analysis slug features
        visits orphan urls medium source.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesVisitsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesvisitsorphan-urlsmediumsource-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Visits
      - Orphan
      - Urls
      - Medium
      - Source
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
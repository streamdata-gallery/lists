---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Money Markets List Swap Rates
  description: Returns swap rate currencies and tenors
  version: 1.0.0
host: www.xignite.com
basePath: xMoneyMarkets.json/XigniteMoneyMarkets
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListTradedSymbols:
    get:
      summary: List Traded Symbols
      description: Returns all symbols and names that are traded recently
      operationId: ListTradedSymbols
      x-api-path-slug: listtradedsymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Traded
      - Symbols
  /ListBondTypes:
    get:
      summary: List Bond Types
      description: ""
      operationId: ListBondTypes
      x-api-path-slug: listbondtypes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Bond
      - Types
  /ListSymbols:
    get:
      summary: List Symbols
      description: List available logos on market.
      operationId: postListsymbols
      x-api-path-slug: listsymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Symbols
  /ListCountryCodes:
    get:
      summary: List Country Codes
      description: Get all of the country codes available to query on.
      operationId: postListcountrycodes
      x-api-path-slug: listcountrycodes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Country
      - Codes
  /ListEventCodes:
    get:
      summary: List Event Codes
      description: Get all of the event codes available to query on.
      operationId: postListeventcodes
      x-api-path-slug: listeventcodes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Event
      - Codes
  /ListCurrencies:
    get:
      summary: List Currencies
      description: List currencies.
      operationId: ListCurrencies
      x-api-path-slug: listcurrencies-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Currencies
  /ListActiveCurrencies:
    get:
      summary: List Active Currencies
      description: List supported currencies.
      operationId: postListactivecurrencies
      x-api-path-slug: listactivecurrencies-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Active
      - Currencies
  /ListOfficialRates:
    get:
      summary: List Official Rates
      description: List supported official rates.
      operationId: postListofficialrates
      x-api-path-slug: listofficialrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Official
      - Rates
  /ListExchanges:
    get:
      summary: List Exchanges
      description: Post listexchanges
      operationId: ListExchanges
      x-api-path-slug: listexchanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Exchanges
  /ListCompanies:
    get:
      summary: List Companies
      description: List Symbols
      operationId: ListCompanies
      x-api-path-slug: listcompanies-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Companies
  /ListEstimates:
    get:
      summary: List Estimates
      description: List Estimates
      operationId: ListEstimates
      x-api-path-slug: listestimates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Estimates
  /ListFutureCategories:
    get:
      summary: List Future Categories
      description: List commmodities future categories.
      operationId: postListfuturecategories
      x-api-path-slug: listfuturecategories-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Future
      - Categories
  /ListSwaps:
    get:
      summary: List Swaps
      description: List all commodity swaps and the exchange on which they are traded.
      operationId: postListswaps
      x-api-path-slug: listswaps-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Swaps
  /ListFutures:
    get:
      summary: List Futures
      description: List all commodity futures and the exchange on which they are traded.
      operationId: postListfutures
      x-api-path-slug: listfutures-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Futures
  /ListFrontMonthContracts:
    get:
      summary: List Front Month Contracts
      description: List all commodity future Front Month Contracts.
      operationId: postListfrontmonthcontracts
      x-api-path-slug: listfrontmonthcontracts-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Front
      - Month
      - Contracts
  /ListFuturesByCategory:
    get:
      summary: List Futures By Category
      description: List futures information by byfuture category.
      operationId: postListfuturesbycategory
      x-api-path-slug: listfuturesbycategory-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Futures
      - By
      - Category
  /ListFuturesByExchange:
    get:
      summary: List Futures By Exchange
      description: List futures information by exchange.
      operationId: postListfuturesbyexchange
      x-api-path-slug: listfuturesbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Futures
      - By
      - Exchange
  /ListSwapsByExchange:
    get:
      summary: List Swaps By Exchange
      description: List swaps information by exchange.
      operationId: postListswapsbyexchange
      x-api-path-slug: listswapsbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Swaps
      - By
      - Exchange
  /ListFutureExchanges:
    get:
      summary: List Future Exchanges
      description: Returns a list of future exchanges
      operationId: ListFutureExchanges
      x-api-path-slug: listfutureexchanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Future
      - Exchanges
  /ListBaseFutures:
    get:
      summary: List Base Futures
      description: Returns a list of base future symbols
      operationId: ListBaseFutures
      x-api-path-slug: listbasefutures-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Base
      - Futures
  /ListFutureChain:
    get:
      summary: List Future Chain
      description: Returns a list of future contracts on a base future symbol
      operationId: ListFutureChain
      x-api-path-slug: listfuturechain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Future
      - Chain
  /ListOptionChain:
    get:
      summary: List Option Chain
      description: Returns a list of options on a future contract
      operationId: ListOptionChain
      x-api-path-slug: listoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Option
      - Chain
  /ListFinancialCenters:
    get:
      summary: List Financial Centers
      description: List financial centers.
      operationId: ListFinancialCenters
      x-api-path-slug: listfinancialcenters-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Financial
      - Centers
  /ListHolidays:
    get:
      summary: List Holidays
      description: List holidays.
      operationId: ListHolidays
      x-api-path-slug: listholidays-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Holidays
  /ListIndexGroups:
    get:
      summary: List Index Groups
      description: List index groups.
      operationId: ListIndexGroups
      x-api-path-slug: listindexgroups-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Index
      - Groups
  /ListIndicesByIndexGroup:
    get:
      summary: List Indices By Index Group
      description: List indices by index group.
      operationId: ListIndicesByIndexGroup
      x-api-path-slug: listindicesbyindexgroup-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Indices
      - Index
      - Group
  /ListIndustries:
    get:
      summary: List Industries
      description: Get the possible industries.
      operationId: ListIndustries
      x-api-path-slug: listindustries-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Industries
  /ListInstrumentClasses:
    get:
      summary: List Instrument Classes
      description: Get the possible instrument classes.
      operationId: ListInstrumentClasses
      x-api-path-slug: listinstrumentclasses-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Instrument
      - Classes
  /ListSectors:
    get:
      summary: List Sectors
      description: Provides a list of all available values for a given sector.
      operationId: ListSectors
      x-api-path-slug: listsectors-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Sectors
  /ListGlobalIndustries:
    get:
      summary: List Global Industries
      description: Get the possible industries.
      operationId: ListGlobalIndustries
      x-api-path-slug: listglobalindustries-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Global
      - Industries
  /ListGlobalSectors:
    get:
      summary: List Global Sectors
      description: Get the possible sectors.
      operationId: ListGlobalSectors
      x-api-path-slug: listglobalsectors-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Global
      - Sectors
  /ListMICToLegacyExchange:
    get:
      summary: List MIC To Legacy Exchange
      description: Get the legacy exchanges.
      operationId: ListMICToLegacyExchange
      x-api-path-slug: listmictolegacyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - MIC
      - Legacy
      - Exchange
  /ListMICToLegacySuffix:
    get:
      summary: List MIC To Legacy Suffix
      description: Get the legacy exchange suffix.
      operationId: ListMICToLegacySuffix
      x-api-path-slug: listmictolegacysuffix-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - MIC
      - Legacy
      - Suffix
  /ListIdentifiersByExchange:
    get:
      summary: List Identifiers By Exchange
      description: Returns all the Indetifiers and names for securities listed on
        an exchange.
      operationId: ListIdentifiersByExchange
      x-api-path-slug: listidentifiersbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Identifiers
      - Exchange
  /ListSymbolChanges:
    get:
      summary: List Symbol Changes
      description: This operation returns symbols changed in this exchange.
      operationId: ListSymbolChanges
      x-api-path-slug: listsymbolchanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Symbol
      - Changes
  /ListMetals:
    get:
      summary: List Metals
      description: List all Metals.
      operationId: ListMetals
      x-api-path-slug: listmetals-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Metals
  /ListRates:
    get:
      summary: List Rates
      description: List supported interest rates.
      operationId: postListrates
      x-api-path-slug: listrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Rates
  /GetIPOList:
    get:
      summary: Get IPO List
      description: Post getipolist
      operationId: GetIPOList
      x-api-path-slug: getipolist-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - IPO
      - List
  /GetLogosList:
    get:
      summary: Get Logos List
      description: Get all symbols which have available logos.
      operationId: postGetlogoslist
      x-api-path-slug: getlogoslist-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Logos
      - List
  /ListMarkets:
    get:
      summary: List Markets
      description: List markets which have avalilable logos.
      operationId: postListmarkets
      x-api-path-slug: listmarkets-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Markets
  /ListSwapRates:
    get:
      summary: List Swap Rates
      description: Returns swap rate currencies and tenors
      operationId: postListswaprates
      x-api-path-slug: listswaprates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Swap
      - Rates
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
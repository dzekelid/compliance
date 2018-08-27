---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Detailed Facility
    Report (DFR) Detailed Facility Report CWA CSV Compliance Service
  description: This procedure obtains data for the CWA Compliance Schedule Violations
    section of the DFR.
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dfr_rest_services.get_sdwis_compliance:
    get:
      summary: Detailed Facility Report SDWIS Compliance Service
      description: This procedure obtains data for the SDWA Compliance section of
        the DFR.
      operationId: this-procedure-obtains-data-for-the-sdwa-compliance-section-of-the-dfr-
      x-api-path-slug: dfr-rest-services-get-sdwis-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - SDWIS
      - Compliance
      - Service
  /dfr_rest_services.get_rcra_compliance:
    get:
      summary: Detailed Facility Report RCRA Compliance Service
      description: This procedure obtains data for the RCRA Compliance section of
        the DFR.
      operationId: this-procedure-obtains-data-for-the-rcra-compliance-section-of-the-dfr-
      x-api-path-slug: dfr-rest-services-get-rcra-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - RCRA
      - Compliance
      - Service
  /dfr_rest_services.get_cwa_se_compliance:
    get:
      summary: Detailed Facility Report CWA SEV Compliance Service
      description: This procedure obtains data for the CWA Single Event Violations
        section of the DFR.
      operationId: this-procedure-obtains-data-for-the-cwa-single-event-violations-section-of-the-dfr-
      x-api-path-slug: dfr-rest-services-get-cwa-se-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - CWA
      - SEV
      - Compliance
      - Service
  /dfr_rest_services.get_cwa_rnc_compliance:
    get:
      summary: Detailed Facility Report CWA RNC Compliance Service
      description: |-
        This procedure obtains data for the CWA SNC/RNC History section located in the Three Year ompliance Status by Quarter portion of the DFR. Valid Compliance Statuses are as follows.
        > S = SNC/Category I - an enforcement action has been issued, and the facility is not meeting its compliance schedule
        > E = SNC/Category I - effluent violations of monthly average limits (Technical Review Criteria and chronic)
        > X = SNC/Category I - effluent violations of non-monthly average limits (Technical Review Criteria and chronic)
        > T = SNC/Category I - compliance schedule reporting violation
        > D = SNC/Category I - reporting violation - nonreceipt of DMR
        > N = RNC/Category II - reportable non-compliance
        > P = Resolved Pending - an enforcement action has been issued, and facility compliance with the action is pending final completion
        > R = Resolved - the facility has returned to compliance with its permit conditions, either with or without issuance of an enforcement action
        > C = Not considered in RNC/SNC based on manual review of data by state or EPA region. This manual override status is also indicated by a superscripted "m".
        > Blank = Not considered in RNC/SNC
        > N/A = EPA's data system is not able to determine the facility-level compliance status based upon the information available. This information may be available from a state database.
      operationId: this-procedure-obtains-data-for-the-cwa-sncrnc-history-section-located-in-the-three-year-ompliance-s
      x-api-path-slug: dfr-rest-services-get-cwa-rnc-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - CWA
      - RNC
      - Compliance
      - Service
  /dfr_rest_services.get_cwa_ps_compliance:
    get:
      summary: Detailed Facility Report CWA PSV Compliance Service
      description: This procedure obtains data for the CWA Permit Schedule Violations
        section of the DFR.
      operationId: this-procedure-obtains-data-for-the-cwa-permit-schedule-violations-section-of-the-dfr-
      x-api-path-slug: dfr-rest-services-get-cwa-ps-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - CWA
      - PSV
      - Compliance
      - Service
  /dfr_rest_services.get_cwa_eff_compliance:
    get:
      summary: Detailed Facility Report CWA Effluent Compliance Service
      description: This procedure obtains data for the CWA Effluent Compliance section
        on the DFR.
      operationId: this-procedure-obtains-data-for-the-cwa-effluent-compliance-section-on-the-dfr---
      x-api-path-slug: dfr-rest-services-get-cwa-eff-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - CWA
      - Effluent
      - Compliance
      - Service
  /dfr_rest_services.get_cwa_cs_compliance:
    get:
      summary: Detailed Facility Report CWA CSV Compliance Service
      description: This procedure obtains data for the CWA Compliance Schedule Violations
        section of the DFR.
      operationId: this-procedure-obtains-data-for-the-cwa-compliance-schedule-violations-section-of-the-dfr-
      x-api-path-slug: dfr-rest-services-get-cwa-cs-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - CWA
      - CSV
      - Compliance
      - Service
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
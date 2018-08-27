swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 1
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Safe Drinking
    Water Act
  description: enforcement-and-compliance-history-online-echo-is-a-tool-developed-and-maintained-by-epas-office-of-enforcement-and-compliance-assurance-for-public-use--echo-provides-integrated-compliance-and-enforcement-information-for-about-800000-regulated-facilities-nationwide-brbrsdw-rest-services-provides-multiple-service-endpoints-each-with-specific-capabilities-to-search-and-retrieve-data-on-public-water-systems-regulated-under-the-safe-drinking-water-act-sdwa--the-returned-results-reflect-data-drawn-from-epas-federal-safe-drinking-water-information-system-sdwis-database-brbrthe-get-systems-get-qid-and-get-download-end-points-are-meant-to-be-used-together-brbrthe-recommended-use-scenario-for-get-systems-get-qid-and-get-downoad-isbrbrb1bnbsp-use-get-systems-to-validate-passed-query-parameters-obtain-summary-statistics-and-to-obtain-a-query-id-qid---qids-are-time-sensitive-and-will-be-valid-for-approximately-30-minutes-brb2bnbsp-use-get-qid-with-the-returned-qid-to-paginate-through-arrays-of-water-system-results-brb3bnbsp-use-get-download-with-the-returned-qid-to-generate-a-comma-separated-value-csv-file-of-water-system-information-that-meets-the-qid-query-criteria-brbruse-the-qcolumns-parameter-to-customize-your-search-results---use-the-metdata-service-endpoint-for-a-list-of-available-output-objects-their-column-ids-and-their-definitions-to-help-you-build-your-customized-output--brbradditional-echo-resourcesnbspnbsp-a-hrefhttpsecho-epa-govtoolswebservicesweb-servicesa-a-hrefhttpsecho-epa-govresourcesechodataaboutthedataabout-echos-dataa-a-hrefhttpsecho-epa-govtoolsdatadownloadsdata-downloadsabr
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
  /dfr_rest_services.get_compliance_summary:
    get:
      summary: Detailed Facility Report Compliance Summary Service
      description: This procedure obtains data for Compliance Summary Data in the
        Enforcement and Compliance Section of the Detailed Facility report.
      operationId: this-procedure-obtains-data-for-compliance-summary-data-in-the-enforcement-and-compliance-section-of
      x-api-path-slug: dfr-rest-services-get-compliance-summary-get
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
      - Compliance
      - Summary
      - Service
  /dfr_rest_services.get_compliance_history:
    get:
      summary: Detailed Facility Report 5 Year Compliance Monitoring History Service
      description: This procedure obtains data for the Compliance Monitoring History
        (5 years) in the Enforcement and Compliance Section of the Detailed Facility
        report.
      operationId: this-procedure-obtains-data-for-the-compliance-monitoring-history-5-years-in-the-enforcement-and-com
      x-api-path-slug: dfr-rest-services-get-compliance-history-get
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
      - "5"
      - Year
      - Compliance
      - Monitoring
      - History
      - Service
  /dfr_rest_services.get_air_compliance:
    get:
      summary: Detailed Facility Report Air Compliance Report Service
      description: This procedure obtains data for Air Compliance in the Environmental
        Conditions Section of the DFR.
      operationId: this-procedure-obtains-data-for-air-compliance-in-the-environmental-conditions-section-of-the-dfr-
      x-api-path-slug: dfr-rest-services-get-air-compliance-get
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
      - Air
      - Compliance
      - Report
      - Service
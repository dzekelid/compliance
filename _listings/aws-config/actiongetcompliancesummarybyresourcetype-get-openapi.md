---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 0
info:
  title: AWS Config API Get Compliance Summary By Resource Type
  version: 1.0.0
  description: Returns the number of resources that are compliant and the number that
    are noncompliant.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeComplianceByConfigRule:
    get:
      summary: Describe Compliance By Config Rule
      description: Indicates whether the specified AWS Config rules are compliant.
      operationId: describeComplianceByConfigRule
      x-api-path-slug: actiondescribecompliancebyconfigrule-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: ConfigRuleNames
        description: Specify one or more AWS Config rule names to filter the results
          by rule
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=DescribeComplianceByResource:
    get:
      summary: Describe Compliance By Resource
      description: Indicates whether the specified AWS resources are compliant.
      operationId: describeComplianceByResource
      x-api-path-slug: actiondescribecompliancebyresource-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: Limit
        description: The maximum number of evaluation results returned on each page
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: ResourceId
        description: The ID of the AWS resource for which you want compliance information
        type: string
      - in: query
        name: ResourceType
        description: The types of AWS resources for which you want compliance information;for
          example, AWS::EC2::Instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetComplianceDetailsByConfigRule:
    get:
      summary: Get Compliance Details By Config Rule
      description: Returns the evaluation results for the specified AWS Config rule.
      operationId: getComplianceDetailsByConfigRule
      x-api-path-slug: actiongetcompliancedetailsbyconfigrule-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: ConfigRuleName
        description: The name of the AWS Config rule for which you want compliance
          information
        type: string
      - in: query
        name: Limit
        description: The maximum number of evaluation results returned on each page
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetComplianceDetailsByResource:
    get:
      summary: Get Compliance Details By Resource
      description: Returns the evaluation results for the specified AWS resource.
      operationId: getComplianceDetailsByResource
      x-api-path-slug: actiongetcompliancedetailsbyresource-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: ResourceId
        description: The ID of the AWS resource for which you want compliance information
        type: string
      - in: query
        name: ResourceType
        description: The type of the AWS resource for which you want compliance information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetComplianceSummaryByConfigRule:
    get:
      summary: Get Compliance Summary By Config Rule
      description: "Returns the number of AWS Config rules that are compliant and
        noncompliant, up to a\n\t\t\tmaximum of 25 for each."
      operationId: getComplianceSummaryByConfigRule
      x-api-path-slug: actiongetcompliancesummarybyconfigrule-get
      parameters:
      - in: query
        name: ComplianceSummary
        description: The number of AWS Config rules that are compliant and the number
          that arenoncompliant, up to a maximum of 25 for each
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetComplianceSummaryByResourceType:
    get:
      summary: Get Compliance Summary By Resource Type
      description: Returns the number of resources that are compliant and the number
        that are noncompliant.
      operationId: getComplianceSummaryByResourceType
      x-api-path-slug: actiongetcompliancesummarybyresourcetype-get
      parameters:
      - in: query
        name: ResourceTypes
        description: Specify one or more resource types to get the number of resources
          that are compliant and the number that are noncompliant for each resource
          type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
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
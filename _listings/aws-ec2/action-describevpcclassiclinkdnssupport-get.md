---
swagger: "2.0"
info:
  title: AWS EC2 API Describe Vpc Classic Link Dns Support
  version: 1.0.0
  description: Describes the ClassicLink DNS support status of one or more VPCs.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeVpcClassicLinkDnsSupport:
    get:
      summary: Describe Vpc Classic Link Dns Support
      description: Describes the ClassicLink DNS support status of one or more VPCs
      operationId: describevpcclassiclinkdnssupport
      parameters:
      - in: query
        name: DryRun
        description: "Checks whether you have the required permissions for the action,
          without actually making the request, \t    and provides an error response"
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance to unlink from the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC to which the instance is linked
        type: string
      responses:
        200:
          description: OK
      tags:
      - vpc dns
definitions: []
x-collection-name: AWS EC2
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
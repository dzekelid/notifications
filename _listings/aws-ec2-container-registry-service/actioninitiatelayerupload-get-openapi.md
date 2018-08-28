---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Initiate Layer Upload
  version: 1.0.0
  description: Notify Amazon ECR that you intend to upload an image layer.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=InitiateLayerUpload:
    get:
      summary: Initiate Layer Upload
      description: Notify Amazon ECR that you intend to upload an image layer.
      operationId: initiateLayerUpload
      x-api-path-slug: actioninitiatelayerupload-get
      responses:
        200:
          description: OK
      tags:
      - Layer Upload
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
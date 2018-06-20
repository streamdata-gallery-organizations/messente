---
swagger: "2.0"
x-collection-name: Messente
x-complete: 0
info:
  title: Messente SMS API Send SMS
  description: Sending SMS text messages
  termsOfService: https://messente.com/pages/terms
  version: v1
host: api2.messente.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  send_sms/:
    get:
      summary: Send SMS
      description: Sending SMS text messages
      operationId: sendSMS
      x-api-path-slug: send-sms-get
      parameters:
      - in: query
        name: autoconvert
        description: ontuse replacement settings from accounts API Auto Replace settings
          page fulltall non GSM 03
      - in: query
        name: charset
        description: Encoding of the text and from parameter value
      - in: query
        name: dlr-url
        description: URL where automatic Delivery Request is made
      - in: query
        name: from
        description: Optional parameter that sets Sender
      - in: query
        name: password
        description: API account security key (API key) from the Messentes web page
      - in: query
        name: text
        description: All characters (Unicode) and long messages are supported
      - in: query
        name: time_to_send
        description: Optional parameter for sending message at some specific time
          in the future
      - in: query
        name: to
        description: Receivers phone number with country code
      - in: query
        name: udh
        description: SMS User Data Header
      - in: query
        name: username
        description: API account user name from the Messentes web page
      responses:
        200:
          description: OK
      tags:
      - SMS
      - Messaging
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
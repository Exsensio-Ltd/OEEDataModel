Station
  - required:
    - id
    - type
    - name
    - productionBreakDuration
    - productionIdealDuration
  - type: "object"
    - allOf:
      - $ref: "https://github.com/ts-exsensio/DataModel/blob/master/common-schema.json#/definitions/EntityIdentifierType"
      - $ref: "https://github.com/ts-exsensio/DataModel/blob/master/common-schema.json#/definitions/TimeSpan"
  - description: >
      ## Description
      This entity contains station information used as a relationship to product measurements data and information like breack and ideal duration related to the station.
      ## Data model
  - properties:
    - name:
      - x-ngsi:
        - type: "Property"
        - model: "https://schema.org/Text"
      - type: "text"
      - description: >
            Name of the station.
    - productionBreakDuration:
      - x-ngsi:
        - type: "Property"
        - model: "https://schema.org/Text"
      - type: "text"
      - description: >
            Unproductive time where the process is scheduled not to run because the crew is scheduled to be away from the line. Breaks are typically excluded from OEE calculations.
    - productionIdealDuration
      - x-ngsi:
        - type: "Property"
        - model: "https://schema.org/Text"
      - type: "text"
      - description: >
            Theoretical minimum time to produce one part. The inverse of Ideal Run Rate. Used to calculate OEE Performance. A variation of the calculation uses Ideal Run Rate instead.
    - totalProductCount:
      - x-ngsi:
        - type: "Property"
        - model: "https://schema.org/Integer"
      - type: "integer"
      - description: >
            Number fo total products that must be executed.

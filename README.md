# OEE Data Model

![GitHub](https://img.shields.io/github/license/Exsensio-Ltd/OEEDataModel)

OEE Data Model is represent the data that can be used in [OEEMicroservice](https://github.com/Exsensio-Ltd/OEEMicroservice) that is directly communicate with Fiware context broker.

The each model is represent the data that stored in the Fiware context broker, used for calculation OEE metric and represented in the Grafana plugin.

## Contents

-   [Product](#product)
-   [Station](#station)
-   [OEE Metric](#oee-metric)
-   [License](#license)


## Product

This entity contains product information used as a relationship to product measurements data. More information [here](https://github.com/Exsensio-Ltd/OEEDataModel/blob/master/Product/doc/spec.md).

## Station

This entity contains station information used as a relationship to product measurements data and information like breack and ideal duration related to the station. More information [here](https://github.com/Exsensio-Ltd/OEEDataModel/blob/master/Station/doc/spec.md).

## OEE Metric

This entity contains several measurements used to calculate the [overall equipment effectiveness (OEE)](https://www.oee.com/). More information on OEE and how the calculation is performed can be found here. More information [here](https://github.com/Exsensio-Ltd/OEEDataModel/blob/master/OEEMetric/doc/spec.md).

## License

[Apache2.0](LICENSE) © Exsensio Ltd

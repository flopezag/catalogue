# Core Context Management

If you want your application to be “smart”, you have to first make it “aware”.
FIWARE provides you with means to produce, gather, publish and consume context
information at large scale and exploit it to transform your application into a
truly smart application.

Context information is represented through values assigned to attributes that
characterize those entities relevant to your application.

To learn more about Core Context Management Enablers, check out the
[documentation](https://fiwaretourguide.readthedocs.io/en/latest/core/introduction/)

## Orion

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/core.svg)](./README.md)
![License](https://img.shields.io/github/license/telefonicaid/fiware-orion.svg)
![](https://img.shields.io/github/release-date/telefonicaid/fiware-orion.svg)
![](https://img.shields.io/github/commits-since/telefonicaid/fiware-orion/latest.svg)

| :octocat: [Git Repository](https://github.com/telefonicaid/fiware-orion/) | :whale: [Docker Hub](https://hub.docker.com/r/fiware/orion/) | :books: [Documentation](https://fiware-orion.rtfd.io) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/core/orion) | :dart: [Roadmap](https://github.com/telefonicaid/fiware-orion/blob/master/doc/roadmap.md) |
| ------------------------------------------------------------------------- | ------------------------------------------------------------ | ----------------------------------------------------- | ------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------- |


### What is Orion?

The Orion Context Broker is an implementation of the Publish/Subscribe Context
Broker GE, providing the NGSI interfaces. Using these interfaces, clients can do
several operations:

-   Register context producer applications, e.g. a temperature sensor within a
    room
-   Update context information, e.g. send updates of temperature
-   Being notified when changes on context information take place (e.g. the
    temperature has changed) or with a given frequency (e.g. get the temperature
    each minute)
-   Query context information. The Orion Context Broker stores context
    information updated from applications, so queries are resolved based on that
    information.

### Why Use Orion?

If you are developing a Data/Context scenario, a broker like the Orion Context
Broker is a must. You would need a component in the architecture able to mediate
between consumer producers (e.g. sensors) and the context consumer applications
(e.g. an mobile phone applications taking advantage of the context information
provided by the sensors). The Orion Context Broker fulfils this functionality in
your architecture.

Orion is an implementation of the FIWARE Publish/Subscribe Context Broker
Generic Enabler. More specifically, Orion implements the following API and Open
Specification:

-   [NGSI v2](https://swagger.lab.fiware.org/?url=https://raw.githubusercontent.com/Fiware/specifications/master/OpenAPI/ngsiv2/ngsiv2-openapi.json)

For context data management, NGSI and the Orion context broker have been
accepted as standards or recommendations by a variety of independent standards
bodies, for example, GSMA recommends NSGI as a standard for relevant parts of
their
[IoT Big Data architecture](https://www.gsma.com/iot/wp-content/uploads/2016/11/CLP.25-v1.0.pdf)
and promotes the Orion Context Broker as the primary example of the standard and
NGSI specification has been selected by the European Commission as a
[CEF Building Block](https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITAL/Context+Broker)
for the implementation of new smart applications and Public Administration.

The use of the Orion context broker is mandatory for any
[platform](https://marketplace.fiware.org/pages/platforms) or
[solution](https://marketplace.fiware.org/pages/solutions) to be labelled as
“Powered by FIWARE” within the
[FIWARE marketplace](https://marketplace.fiware.org/)

### Quality Assurance

The **Orion** project is part of [FIWARE](https://fiware.org/) and has been
rated as follows:

-   **Version Tested:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Version&url=https://fiware.github.io/catalogue/json/orion.json&query=$.version&colorB=blue)
-   **Documentation:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Completeness&url=https://fiware.github.io/catalogue/json/orion.json&query=$.docCompleteness&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Usability&url=https://fiware.github.io/catalogue/json/orion.json&query=$.docSoundness&colorB=blue)
-   **Responsiveness:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Respond&url=https://fiware.github.io/catalogue/json/orion.json&query=$.timeToCharge&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Fix&url=https://fiware.github.io/catalogue/json/orion.json&query=$.timeToFix&colorB=blue)
-   **FIWARE Testing:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Tests%20Passed&url=https://fiware.github.io/catalogue/json/orion.json&query=$.failureRate&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Scalability&url=https://fiware.github.io/catalogue/json/orion.json&query=$.scalability&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Performance&url=https://fiware.github.io/catalogue/json/orion.json&query=$.performance&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Stability&url=https://fiware.github.io/catalogue/json/orion.json&query=$.stability&colorB=blue)

## Cygnus

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/core.svg)](./README.md)
![License](https://img.shields.io/github/license/telefonicaid/fiware-cygnus.svg)
![](https://img.shields.io/github/release-date/telefonicaid/fiware-cygnus.svg)
![](https://img.shields.io/github/commits-since/telefonicaid/fiware-cygnus/latest.svg)

| :octocat: [Git Repository](https://github.com/telefonicaid/fiware-cygnus/) | :whale: [Docker Hub](https://hub.docker.com/r/fiware/cygnus-ngsi/) | :books: [Documentation](https://fiware-cygnus.rtfd.io) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/core/cygnus) | :dart: [Roadmap](https://github.com/telefonicaid/fiware-cygnus/blob/master/doc/roadmap.md) |
| -------------------------------------------------------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |


### What is Cygnus?

Cygnus is a connector in charge of persisting context data sources into other
third-party databases and storage systems, creating a historical view of the
context. Internally, Cygnus is based on Apache Flume,
[Flume](https://flume.apache.org/) is a data flow system based on the concepts
of flow-based programming. It supports powerful and scalable directed graphs of
data routing, transformation, and system mediation logic. It was built to
automate the flow of data between systems. While the term 'dataflow' can be used
in a variety of contexts, we use it here to mean the automated and managed flow
of information between systems.

Each data persistence agent within Cygnus is composed of three parts - a
listener or source in charge of receiving the data, a channel where the source
puts the data once it has been transformed into a Flume event, and a sink, which
takes Flume events from the channel in order to persist the data within its body
into a third-party storage.

### Why Use Cygnus?

Persisting historical context data is useful for big data analysis - it can be
used to discover trends, or data can be sampled and aggregated to remove the
influence of outlying data measurements. However within each Smart Solution, the
significance of each entity type will differ and entities and attributes may
need to be sampled at different rates.

Since the business requirements for using context data differ from application
to application, there is no one standard use case for historical data
persistence. Therefore rather than overloading the context broker with the job
of historical context data persistence, this role has been separated out into a
separate, highly configurable component - Cygnus.

Cygnus plays the role of a connector between the Orion Context Broker (which is
an
[NGSI](https://swagger.lab.fiware.org/?url=https://raw.githubusercontent.com/Fiware/specifications/master/OpenAPI/ngsiv2/ngsiv2-openapi.json)
source of data) and a wide range of external systems such as
[MySQL](https://www.mysql.com/), [MongoDB](https://www.mongodb.org/) etc. You
should use Cygnus if you need to process and persist context data so that you
can keep a historical record. Cygnus can also be used the filter and repost
context data back into Orion.

### Quality Assurance

The **Cygnus** project is part of [FIWARE](https://fiware.org/) and has been
rated as follows:

-   **Version Tested:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Version&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.version&colorB=blue)
-   **Documentation:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Completeness&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.docCompleteness&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Usability&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.docSoundness&colorB=blue)
-   **Responsiveness:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Respond&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.timeToCharge&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Fix&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.timeToFix&colorB=blue)
-   **FIWARE Testing:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Tests%20Passed&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.failureRate&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Scalability&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.scalability&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Performance&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.performance&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Stability&url=https://fiware.github.io/catalogue/json/cygnus.json&query=$.stability&colorB=blue)

## STH Comet

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/core.svg)](./README.md)
![License](https://img.shields.io/github/license/telefonicaid/fiware-sth-comet.svg)
![](https://img.shields.io/github/release-date/telefonicaid/fiware-sth-comet.svg)
![](https://img.shields.io/github/commits-since/telefonicaid/fiware-sth-comet/latest.svg)

| :octocat: [Git Repository](https://github.com/telefonicaid/fiware-sth-comet/) | :whale: [Docker Hub](https://hub.docker.com/r/fiware/sth-comet/) | :books: [Documentation](https://fiware-sth-comet.rtfd.io) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/core/sth-comet) | :dart: [Roadmap](https://github.com/telefonicaid/fiware-sth-comet/blob/master/doc/roadmap.md) |
| ----------------------------------------------------------------------------- | ---------------------------------------------------------------- | --------------------------------------------------------- | ---------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |


### What is STH Comet?

Short Time Historic (STH) - Comet is a component of the FIWARE ecosystem in
charge of managing (storing and retrieving) historical raw and aggregated time
series context information about the evolution in time of context data (i.e.,
entity attribute values) registered in an Orion Context Broker instance.

### Why use STH Comet?

The creation and analysis of trend data is a common requirement of
context-driven systems - therefore the FIWARE platform offers a generic enabler
(STH-Comet) specifically to deal with the issue of persisting and interpreting
time series data.

Within the FIWARE platform, historical context data can be persisted to a
database - this results in a series of data points. Each time-stamped data point
represents the state of context entities at a given moment in time. The
individual data points are relatively meaningless on their own, it is only
through combining a series data points that meaningful statistics such as
maxima, minima and trends can be observed.

### Quality Assurance

The **STH-Comet** project is part of [FIWARE](https://fiware.org/) and has been
rated as follows:

-   **Version Tested:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Version&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.version&colorB=blue)
-   **Documentation:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Completeness&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.docCompleteness&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Usability&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.docSoundness&colorB=blue)
-   **Responsiveness:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Respond&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.timeToCharge&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Fix&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.timeToFix&colorB=blue)
-   **FIWARE Testing:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Tests%20Passed&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.failureRate&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Scalability&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.scalability&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Performance&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.performance&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Stability&url=https://fiware.github.io/catalogue/json/sth_comet.json&query=$.stability&colorB=blue)

---

## :seedling: QuantumLeap (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/core.svg)](./README.md)
![License](https://img.shields.io/github/license/smartsdk/ngsi-timeseries-api.svg)
![](https://img.shields.io/github/last-commit/smartsdk/ngsi-timeseries-api.svg)
![](https://img.shields.io/github/tag/smartsdk/ngsi-timeseries-api.svg)

| :octocat: [Git Repository](https://github.com/smartsdk/ngsi-timeseries-api/) | :whale: [Docker Hub](https://hub.docker.com/r/smartsdk/quantumleap/) | :books: [Documentation](https://quantumleap.rtfd.io/) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/core/quantum-leap) | :dart: [Roadmap](https://github.com/smartsdk/ngsi-timeseries-api/blob/master/docs/roadmap.md) |
| ---------------------------------------------------------------------------- | -------------------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |


### What is QuantumLeap?

The QuantumLeap Generic Enabler focuses on persisting historical context data
into [time-series databases](https://en.wikipedia.org/wiki/Time_series_database)
such as [CrateDB](https://crate.io/) with reference to maintaining a scalable
architecture and compatibility with visualization tools such as
[Grafana](http://www.grafana.com/)

### Why use QuantumLeap?

The appropriate use of time series data analysis will depend on your use case
and the reliability of the data measurements you receive. Time series data
analysis can be used to answer questions such as:

-   What was the maximum measurement of a device within a given time period?
-   What was the average measurement of a device within a given time period?
-   What was the sum of the measurements sent by a device within a given time
    period?

QuantumLeap offers great flexibility in measuring and monitoring time-series
data and leverages existing time-series-based databases to be able to support
complex queries such as cross-entity queries (e.g. an average of averages)

The **QuantumLeap** project is part of [FIWARE](https://fiware.org/) and will be
rated as part of the next release.

## :seedling: Draco (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/core.svg)](./README.md)
![License](https://img.shields.io/github/license/ging/fiware-draco.svg)
![](https://img.shields.io/github/release-date/ging/fiware-draco.svg)
![](https://img.shields.io/github/commits-since/ging/fiware-draco/latest.svg)

| :octocat: [Git Repository](https://github.com/ging/fiware-draco) | :whale: [Docker Hub](https://hub.docker.com/r/ging/fiware-draco) | :books: [Documentation](https://fiware-draco.rtfd.io) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/core/draco) | :dart: [Roadmap](https://github.com/ging/fiware-draco/blob/master/docs/roadmap.md) |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------- |


### What is Draco?

Draco is a connector in charge of persisting context data sources into other
third-party databases and storage systems, creating a historical view of the
context. Internally, Draco is based on Apache NiFi.
[NiFi](https://nifi.apache.org) is a popular framework for data management and
processing from multiple sources.

Draco plays the role of a connector between the Orion Context Broker (which is
an
[NGSI](https://swagger.lab.fiware.org/?url=https://raw.githubusercontent.com/Fiware/specifications/master/OpenAPI/ngsiv2/ngsiv2-openapi.json)
source of data) source of data) and a wide range of external systems such as
MySQL, MongoDB etc. You can use Draco if you need to process and persist context
data so that you can keep a historical record. Draco can also be used to filter
and repost context data back into Orion.

### Why Use Draco?

Persisting historical context data is useful for big data analysis - it can be
used to discover trends, or data can be sampled and aggregated to remove the
influence of outlying data measurements. However within each Smart Solution, the
significance of each entity type will differ and entities and attributes may
need to be sampled at different rates.

Since the business requirements for using context data differ from application
to application, there is no one standard use case for historical data
persistence. Therefore rather than overloading the context broker with the job
of historical context data persistence, this role has been separated out into
another enabler. Amongst the advantages of the component, Draco offers a
flexible graphical interface so it is possible to amend your data flows
according to your current business needs.

### Quality Assurance

The **Draco** project is part of [FIWARE](https://fiware.org/) and has been
rated as follows:

-   **Version Tested:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Version&url=https://fiware.github.io/catalogue/json/draco.json&query=$.version&colorB=blue)
-   **Documentation:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Completeness&url=https://fiware.github.io/catalogue/json/draco.json&query=$.docCompleteness&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Usability&url=https://fiware.github.io/catalogue/json/draco.json&query=$.docSoundness&colorB=blue)
-   **Responsiveness:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Respond&url=https://fiware.github.io/catalogue/json/draco.json&query=$.timeToCharge&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Time%20to%20Fix&url=https://fiware.github.io/catalogue/json/draco.json&query=$.timeToFix&colorB=blue)
-   **FIWARE Testing:**
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Tests%20Passed&url=https://fiware.github.io/catalogue/json/draco.json&query=$.failureRate&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Scalability&url=https://fiware.github.io/catalogue/json/draco.json&query=$.scalability&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Performance&url=https://fiware.github.io/catalogue/json/draco.json&query=$.performance&colorB=blue)
    ![](https://img.shields.io/badge/dynamic/json.svg?label=Stability&url=https://fiware.github.io/catalogue/json/draco.json&query=$.stability&colorB=blue)

# Functional Capabilities

<mark style="color:orange;">\<Lead-in from Overview></mark>

<mark style="color:orange;">Key Capabilities:</mark>

<mark style="color:orange;">**Observe What Matters**</mark><mark style="color:orange;">: Derive insights to understand user behaviour and preferences, improve products, etc. by capturing user interaction & system data according to flexible specifications defined by you.</mark>

<mark style="color:orange;">**Seamless Data Transfer**</mark><mark style="color:orange;">: Stream and store the telemetry data efficiently using an out-of-the-box design that decouples data generation systems from the data processing systems.</mark>

<mark style="color:orange;">**Scalable Data Processing:**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">Perform real-time data processing i.e. cleaning & transforming according to reporting needs, with addition of metadata of various entities such as user, device and content.</mark>&#x20;

<mark style="color:orange;">**Readymade Key Metrics**</mark><mark style="color:orange;">: Derive insights quickly, from pre-defined summary metrics such as time spent in a session, time spent on a content etc.</mark>

<mark style="color:orange;">**Easy Reporting and Querying**</mark><mark style="color:orange;">: perform advanced analytics & reporting in near real-time by running queries on both the telemetry data and summarized data that is loaded into an analytics data store.</mark>

<mark style="color:orange;"></mark>

<mark style="color:green;">The following are the details of the functional capabilities enabled using Sunbird Obsrv:</mark>

<mark style="color:green;">**Flexible Data Model Specification:**</mark> <mark style="color:green;"></mark><mark style="color:green;">The Telemetry data model is designed to instrument telemetry data (interactions, metrics and logs) for any domain.</mark>&#x20;

The domain of an application determines to a vast extent the design of the data model for understanding various interactions and metrics from the application. Sunbird Obsrv is flexible  to allows the application to decide on the data model for the Telemetry and it is designed intelligently to keep the data structure for the event data as flexible as possible while enforcing to capture some common characteristics to ascertain the component details of the source system that generates the Telemetry.&#x20;

<mark style="color:green;">**Data collection at scale:**</mark> <mark style="color:green;"></mark><mark style="color:green;">Perform seamless telemetry data collection from client apps using horizontally scalable api.</mark> Ability to seamlessly scale the telemetry data collection is very important as it enables the client applications to sync the data without any data loss and also determines the rate at which . The data collection api in Sunbird Obsrv can be horizontally scaled by adding more instances of the collector both in containerized and virtual machine based environments. The data collector also provides options for configurable data sink such as Apache Kafka, Apache Cassandra or local hard disks. The data sinks, in turn, can be scaled horizontally which helps transferring telemetry data at very high transfer rates along with consistent and durable storage.

<mark style="color:green;">**Easy integration with Cloud providers:**</mark> <mark style="color:green;"></mark><mark style="color:green;">The analytics platform is cloud agnostic and can be easily deployed onto any of the popular cloud platforms such as AWS, Azure or Google Cloud Platform.</mark> The analytics platform has various plugable components and all of the components provide configurations to support deployments onto the popular cloud platforms. Furthermore, most of the components are deployed onto Kubernetes, the most popular tool for container orchestration.&#x20;

<mark style="color:green;">**Streaming/Batch data processing:**</mark> <mark style="color:green;"></mark><mark style="color:green;">The analytics platform provides an ability to process both real-time streaming data and batch data to derive insights.</mark>&#x20;

The analytics platform is built using lambda architecture principles. Lambda architecture is designed to provide the capability to process both real-time streaming data and batch data. The analytics platform has both a batch layer and a stream layer storage which helps in fault-tolerant and scalable architecture for data processing. The stream layer ensures that insights are derived in near real time to take immediate actions on the data arriving and the batch layer ensures that reporting requirements over a specific time period are addressed. Fault tolerance is built into the pipeline which ensures that there will be no data loss. Lambda architecture also provides the capability to replay or reload data for data processing with idempotency.

<mark style="color:green;">**Build fast, scalable data analytics:**</mark> <mark style="color:green;"></mark><mark style="color:green;">The analytics platform is designed to build ad-hoc analytics or recurring reports in a fast, scalable manner.</mark>&#x20;

Any analytics platform should allow ad-hoc user queries to be served with low latency response times and should provide an immutable data storage to obtain a snapshot of the historical data. Sunbird Obsrv's analytics platform uses different data stores to address the ability to query data with low latency. It uses the distributed cloud storage for batch processing of data to generate reports and it uses an Online Analytical Processing (OLAP) data store to address real-time adhoc user queries. Both these layers provide the ability to build fast and scalable analytics and reporting systems on top of large amounts (terabytes) of data with efficient infrastructure. The access of the data from the polyglot data stores is always using APIs which can horizontally scale according to the latency requirements.

<mark style="color:green;">**Downloadable data:**</mark> <mark style="color:green;"></mark><mark style="color:green;">The analytics platform provides an ability to download both the raw data and aggregated data through the reporting api also with an ability to schedule recurring reporting requirements.</mark>

Apart from the ability to build a querying layer on top of the data, a data analytics platform should provide the ability to download the data from the system so that the client applications can build their own insights on top of the data. Sunbird Obsrv's analytics platform is designed with this capability in mind. Cloud data stores in general store objects that are private and only the object owner has permissions to access them. The analytics platform provides APIs with access control to download data. The APIs generate urls which are pre-signed with security credentials of the object owner to grant time-bound permissions to download the data. This capability opens up a lot of possibilities for the client applications to create a visualization without overloading the data platform.

_<mark style="color:blue;"></mark>_

_<mark style="color:blue;"></mark>_

Some additional possibiities that can be visualised using Sunbird Obsrv include:

* Allowing for `capture of telemetry` as per chosen specifications from an agricultural monitoring system, and `processing and analysis of the resulting data` to optimise output
* Aggregation of anonymised health data from across platforms, and its `analysis` to arrive at health indicators and patterns at population scale.&#x20;
* Analysis of `streams of weather data` from satellites to better `predict` weather patterns.

****

****

_Obsrv_ allows for extensive configurability so as to enable creation of various custom workflows. Refer to the pages for different components listed in the Product & developer guide page to see details of what configurations are available for each.


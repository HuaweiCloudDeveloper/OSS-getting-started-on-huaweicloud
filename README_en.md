<p align="center">
    <h1 align="center">huaweicloud-oss-quickstart</h1>
  <p align="center">
    <strong>English</strong> | <a href="README.md"><strong>简体中文</strong></a>
</p>


This project collects information about **open-source projects adapted for Huawei Cloud**, including supported software, versions, adaptation components, and usage guides. It helps users quickly deploy, integrate, and use mainstream open-source ecosystems on Huawei Cloud.

> ***If this project helps you, please click the `Star` button in the upper right to support us!***

> ***Contribute: If you find an open-source project that has not yet been adapted for Huawei Cloud, feel free to [submit an ISSUE](https://github.com/HuaweiCloudDeveloper/huaweicloud-oss-quickstart/issues).  
Please provide the open-source software name, version, and adaptation needs or issues. We will enhance the ecosystem support based on your feedback.***

## Overview of Huawei Cloud Open-Source Ecosystem Adaptation Projects

| Category         | Language | Open-Source Project                                                                                | Adaptation Scenario                        | Huawei Cloud Services / Components                         | Version Info                       | Guide |
|:-----------------|:---------|:---------------------------------------------------------------------------------------------------|:-------------------------------------------|:------------------------------------------------------------|:------------------------------------|:------|
| Container Mgmt   | Go       | [Cluster API](https://github.com/HuaweiCloudDeveloper/cluster-api-provider-huawei)                | Kubernetes cluster lifecycle management     | CCE, ELB                                                    | Cluster API v1.9 / Huawei v0.1.0   |       |
| Container Mgmt   | Go       | [OpenKruiseGame](https://github.com/HuaweiCloudDeveloper/openkruisegame)                          | Game server orchestration & scheduling      | CCE                                                         | v0.10.0                            |       |
| Certificate Mgmt | Go       | [cert-manager](https://github.com/HuaweiCloudDeveloper/cert-manager-webhook-huawei)               | Automated certificate issuance              | CCE, DNS                                                    | v1.14                              |       |
| DNS Mgmt         | Go       | [external-dns](https://github.com/setoru/external-dns-webhook-huaweicloud)                        | Dynamic DNS auto-resolution                 | DNS, CCE                                                    | v0.14                              |       |
| Image Registry   | Go       | [Harbor](https://github.com/goharbor/harbor)                                                      | Enterprise-grade image registry mgmt        | CCE, OBS                                                    | v2.11                              |       |
| Monitoring/Store | Go       | [Thanos](https://github.com/thanos-io/thanos)                                                     | Distributed monitoring & multi-cluster data | CCE, ECS, OBS                                               | v0.36                              |       |
| CI/CD            | Go       | [Drone](https://github.com/harness/drone)                                                         | Container-based CI                          | OBS                                                         | v2.22                              |       |
| Image Build      | Go       | [Kaniko](https://github.com/GoogleContainerTools/kaniko)                                          | Build images without Docker daemon          | OBS                                                         | v1.23                              |       |
| Database         | Go       | [CockroachDB](https://github.com/cockroachdb/cockroach)                                           | Distributed SQL database                    | OBS                                                         | v24.1                              |       |
| Database         | Go       | [Vitess](https://github.com/vitessio/vitess)                                                      | MySQL horizontal scaling framework          | OBS                                                         | v20.0                              |       |
| Database         | Go       | [Weaviate](https://github.com/weaviate/weaviate)                                                  | Vector DB & knowledge search engine         | OBS                                                         | v1.27                              |       |
| O&M Monitoring   | Go       | [Velero](https://github.com/vmware-tanzu/velero)                                                  | Kubernetes backup & restore                 | OBS                                                         | v1.14                              |       |
| O&M Monitoring   | Go       | [Prometheus](https://github.com/prometheus/prometheus)                                            | Cloud & container monitoring                | ECS                                                         | v3.0                               |       |
| General App      | Go       | [Vault](https://github.com/hashicorp/vault)                                                       | Secrets & credential management             | OBS, IAM                                                    | v1.17                              |       |
| General App      | Go       | [JuiceFS](https://github.com/juicedata/juicefs)                                                   | Distributed file system                     | OBS                                                         | v1.2                               |       |
| Data Workflow    | Python   | [Apache Airflow](https://github.com/apache/airflow)                                               | ETL & task scheduling                       | CCE, OBS, DWS, DLI, DataArts, SMN, Modelarts, MRS           | v2.5                               |       |
| Data Visualization | Python | [Apache Superset](https://github.com/apache/superset)                                             | BI & data visualization                      | DWS, CCE, ECS                                               | v4.0                               |       |
| Scheduling        | Python | [Prefect](https://github.com/PrefectHQ/prefect)                                                   | Dataflow & task orchestration                | OBS                                                         | v3.1                               |       |
| Scheduling        | Python | [Dagster](https://github.com/dagster-io/dagster)                                                  | Data pipelines & orchestration               | OBS                                                         | v1.8                               |       |
| CI/CD             | Python | [StackStorm](https://github.com/StackStorm/st2)                                                   | Automation workflows & CI control            | OBS                                                         | v3.8                               |       |
| Automation/Config | Python | [Ansible](https://github.com/ansible/ansible)                                                     | Automated deployment & configuration mgmt    | CCE, ECS, VPC, EVS                                          | v10.3                              |       |
| General App       | Python | [Airbyte](https://github.com/airbytehq/airbyte)                                                   | Data sync & integration                      | OBS, DWS                                                    | v0.68                              |       |
| General App       | Python | [Chaos Genius](https://github.com/chaos-genius/chaos_genius)                                      | Anomaly detection & analytics                | DWS (PostgreSQL)                                             | v0.6                               |       |
| General App       | Python | [Pandas](https://github.com/pandas-dev/pandas)                                                    | Data analysis & processing                   | OBS                                                         | v2.2                               |       |
| General App       | Python | [MLflow](https://github.com/mlflow/mlflow)                                                        | Model mgmt & experiment tracking             | OBS                                                         | v2.18                              |       |
| Database          | C++    | [Milvus](https://github.com/milvus-io/milvus)                                                     | Vector database                              | OBS                                                         | v2.5                               |       |
| Database          | C++    | [Doris](https://github.com/apache/doris)                                                          | MPP analytical database                       | MRS                                                         | v3.0                               |       |
| Database          | C++    | [ClickHouse](https://github.com/ClickHouse/ClickHouse)                                            | High-performance columnar DB                 | OBS                                                         | v24.10                             |       |
| General App       | Java   | [StreamSets](https://github.com/streamsets/datacollector-oss)                                     | Data pipeline ingestion                       | OBS                                                         | v5.11                              |       |
| General App       | Java   | [DataX](https://github.com/alibaba/DataX)                                                         | Heterogeneous data sync                       | OBS                                                         | v4.0                               |       |
| Data Flow         | Java   | [Apache NiFi](https://github.com/apache/nifi)                                                     | Dataflow orchestration & visual integration   | CCE, ECS, OBS, SMN                                           | v1.27                              |       |
| Database          | Java   | [CrateDB](https://github.com/crate/crate)                                                         | Distributed time-series DB                   | OBS                                                         | v5.9                               |       |
| API Gateway       | Java   | [Apache ShenYu](https://github.com/apache/shenyu)                                                 | High-performance API gateway                  | EulerOS, LTS                                                | v2.6                               |       |
| Scheduling        | Java   | [Alluxio](https://github.com/Alluxio/alluxio)                                                     | Data caching & distributed storage orchestration | OBS                                                      | v3.1                               |       |
| CI/CD             | Java   | [Jenkins](https://github.com/jenkinsci/jenkins)                                                   | CI/CD automation build & release              | CodeArts Pipeline, CodeArts Check, VSS, OBS, SMN            | v2.479                             |       |
| O&M Monitoring    | Java   | [HertzBeat](https://github.com/dromara/hertzbeat)                                                 | Cloud-native monitoring platform              | EulerOS, SMN                                                | v2.1                               |       |
| O&M Monitoring    | Java   | [Jpom](https://github.com/dromara/Jpom)                                                           | Project deployment & monitoring               | ECS                                                         | v2.10                              |       |
| Stream/Message    | Java   | [Apache Flink](https://github.com/apache/flink)                                                   | Real-time stream processing                   | OBS                                                         | v1.20                              |       |
| Stream/Message    | Java   | [Apache Pulsar](https://github.com/apache/pulsar)                                                 | Distributed messaging system                  | OBS                                                         | v3.3                               |       |
| Stream/Message    | Java   | [Apache Heron](https://github.com/apache/incubator-heron)                                         | Real-time streaming engine                    | OBS                                                         | v0.24                              |       |
| Stream/Message    | Java   | [Logstash](https://github.com/elastic/logstash)                                                   | Log collection & data pipeline                | OBS                                                         | v8.15                              |       |
| Stream/Message    | Java   | [Siddhi](https://github.com/siddhi-io/siddhi)                                                     | Stream event processing engine                | OBS                                                         | v6.0                               |       |
| General App       | Java   | [Apache Hadoop](https://github.com/apache/hadoop)                                                 | Big-data distributed storage & compute         | OBS                                                         | v3.4                               |       |
| General App       | Java   | [Apache Flume](https://github.com/apache/flume)                                                   | Data ingestion & transport                    | OBS                                                         | v1.11                              |       |
| General App       | Java   | [Apache Hive](https://github.com/apache/hive)                                                     | Data warehouse query engine                   | OBS                                                         | v4.0                               |       |
| General App       | Java   | [Apache Druid](https://github.com/apache/druid)                                                   | Real-time analytical DB                       | OBS                                                         | v31.0                             |       |
| General App       | Java   | [Apache Hudi](https://github.com/apache/hudi)                                                     | Incremental data lake                         | OBS, DIS                                                    | v1.1                               |       |
| General App       | Java   | [Apache Drill](https://github.com/apache/drill)                                                   | SQL query engine                              | OBS                                                         | v2.1                               |       |
| General App       | Java   | [Pentaho Kettle](https://github.com/pentaho/pdi-ce)                                               | ETL data integration                          | OBS                                                         | v9.4                               |       |
| General App       | Java   | [Seatunnel](https://github.com/apache/seatunnel)                                                  | Data integration & synchronization            | OBS                                                         | v2.3                               |       |
| General App       | Java   | [DeepStream](https://github.com/NVIDIA-AI-IOT/deepstream_reference_apps)                          | Video stream analytics framework              | OBS                                                         | v7.1                               |       |
| General App       | Java   | [zyplayer-doc](https://github.com/zyplayer/zyplayer-doc)                                          | API documentation & knowledge center          | OBS                                                         | v3.3                               |       |
| General App       | Java   | [Apache Iceberg](https://github.com/apache/iceberg)                                               | Table-format data lake                        | OBS                                                         | v1.7                               |       |
| General App       | Java   | [Hop](https://github.com/apache/hop)                                                              | Data integration & orchestration              | OBS                                                         | v2.9                               |       |
| General App       | Java   | [Rainbond](https://github.com/goodrain/rainbond)                                                  | Cloud-native application management platform  | CCE                                                         | v7.4                               |       |
| General App       | Scala  | [Apache Spark](https://github.com/apache/spark)                                                   | Distributed in-memory computing               | OBS                                                         | v3.5                               |       |

---

## Usage Notes

- All projects are adapted and tested on Huawei Cloud based on **upstream open-source community versions**.
- Detailed **deployment examples**, **configuration instructions**, and **Huawei Cloud usage notes** are provided in the guide directory.

---

## Contributing

We welcome community developers and enterprise users to join the ecosystem adaptation effort:

1. Fork this repository and submit a Pull Request;
2. Or submit adaptation requests via the [Issues section](https://github.com/HuaweiCloudDeveloper/huaweicloud-oss-quickstart/issues);
3. Please include the open-source project name, version, and adaptation scenario details.

---

*This project is maintained by the Huawei Cloud Developer Ecosystem Team to promote best practices of mainstream open-source projects on Huawei Cloud.*

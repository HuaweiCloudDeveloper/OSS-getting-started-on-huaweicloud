<p align="center">
    <h1 align="center">OSS-getting-started-on-huaweicloud</h1>
  <p align="center">
    <a href="README_en.md"><strong>English</strong></a> | <strong>简体中文</strong>
</p>

本项目收集 **华为云适配的开源项目** 信息，包括适配的开源软件、版本、适配组件及使用指南等内容，帮助用户快速在华为云上部署、集成和使用主流开源生态。

> ***如果本项目对您有帮助，请点击右上角 `Star` 支持我们！***

> ***
*参与共建：如果您发现某个开源项目在华为云上还未适配，欢迎[提交 ISSUE](https://github.com/HuaweiCloudDeveloper/oss-getting-started-on-huaweicloud/issues)
。请提供开源软件名称、版本、适配需求或问题，我们将结合您的反馈完善生态适配支持。***

# 华为云开源生态适配项目总览

| 类别      | 语言     | 开源项目                                                                                | 适配场景                | 华为云组件 / 服务                                   | 版本信息                             | 使用指南 |
|:--------|:-------|:------------------------------------------------------------------------------------|:--------------------|:---------------------------------------------|:---------------------------------|:-----|
| 容器管理    | Go     | [Cluster API](https://github.com/HuaweiCloudDeveloper/cluster-api-provider-huawei)  | Kubernetes 集群生命周期管理 | CCE、ELB                                      | Cluster API v1.9 / Huawei v0.1.0 |      |
| 容器管理    | Go     | [OpenKruiseGame](https://github.com/HuaweiCloudDeveloper/openkruisegame)            | 游戏服务器编排与调度          | CCE                                          | v0.10.0                          |      |
| 证书管理    | Go     | [cert-manager](https://github.com/HuaweiCloudDeveloper/cert-manager-webhook-huawei) | 证书自动化签发             | CCE、DNS                                      | v1.14                            |      |
| DNS 管理  | Go     | [external-dns](https://github.com/setoru/external-dns-webhook-huaweicloud)          | 动态域名自动解析            | DNS、CCE                                      | v0.14                            |      |
| 容器镜像仓库  | Go     | [Harbor](https://github.com/goharbor/harbor)                                        | 企业级容器镜像仓库管理         | CCE、OBS                                      | v2.11                            |      |
| 监控存储扩展  | Go     | [Thanos](https://github.com/thanos-io/thanos)                                       | 分布式监控与多集群指标存储       | CCE、ECS、OBS                                  | v0.36                            |      |
| 持续集成交付  | Go     | [Drone](https://github.com/harness/drone)                                           | 容器化持续集成             | OBS                                          | v2.22                            |      |
| 镜像构建与管理 | Go     | [Kaniko](https://github.com/GoogleContainerTools/kaniko)                            | 无需Docker守护进程的镜像构建   | OBS                                          | v1.23                            |      |
| 数据库     | Go     | [CockroachDB](https://github.com/cockroachdb/cockroach)                             | 分布式关系型数据库           | OBS                                          | v24.1                            |      |
| 数据库     | Go     | [Vitess](https://github.com/vitessio/vitess)                                        | MySQL 水平扩展框架        | OBS                                          | v20.0                            |      |
| 数据库     | Go     | [Weaviate](https://github.com/weaviate/weaviate)                                    | 向量数据库与知识检索引擎        | OBS                                          | v1.27                            |      |
| 运维监控    | Go     | [Velero](https://github.com/vmware-tanzu/velero)                                    | Kubernetes 集群备份与恢复  | OBS                                          | v1.14                            |      |
| 运维监控    | Go     | [Prometheus](https://github.com/prometheus/prometheus)                              | 云服务与容器监控            | ECS                                          | v3.0                             |      |
| 通用应用    | Go     | [Vault](https://github.com/hashicorp/vault)                                         | 密钥与凭证管理             | OBS、IAM                                      | v1.17                            |      |
| 通用应用    | Go     | [JuiceFS](https://github.com/juicedata/juicefs)                                     | 分布式文件系统             | OBS                                          | v1.2                             |      |
| 数据工作流   | Python | [Apache Airflow](https://github.com/apache/airflow)                                 | ETL 与任务调度           | CCE、OBS、DWS、DLI、DataArts、SMN、Modelarts、MRS   | v2.5                             |      |
| 数据可视化   | Python | [Apache Superset](https://github.com/apache/superset)                               | 数据可视化与 BI 报表        | DWS、CCE、ECS                                  | v4.0                             |      |
| 调度与编排   | Python | [Prefect](https://github.com/PrefectHQ/prefect)                                     | 数据流与任务编排            | OBS                                          | v3.1                             |      |
| 调度与编排   | Python | [Dagster](https://github.com/dagster-io/dagster)                                    | 数据管道与调度编排框架         | OBS                                          | v1.8                             |      |
| 持续集成交付  | Python | [StackStorm](https://github.com/StackStorm/st2)                                     | 自动化工作流与CI管控         | OBS                                          | v3.8                             |      |
| 自动化与配置  | Python | [Ansible](https://github.com/ansible/ansible)                                       | 自动化部署与配置管理          | CCE、ECS、VPC、EVS                              | v10.3                            |      |
| 通用应用    | Python | [Airbyte](https://github.com/airbytehq/airbyte)                                     | 数据同步与整合             | OBS、DWS                                      | v0.68                            |      |
| 通用应用    | Python | [Chaos Genius](https://github.com/chaos-genius/chaos_genius)                        | 异常检测与分析             | DWS（PostgreSQL）                              | v0.6                             |      |
| 通用应用    | Python | [Pandas](https://github.com/pandas-dev/pandas)                                      | 数据分析与处理             | OBS                                          | v2.2                             |      |
| 通用应用    | Python | [MLflow](https://github.com/mlflow/mlflow)                                          | 模型管理与实验追踪           | OBS                                          | v2.18                            |      |
| 数据库     | C++    | [Milvus](https://github.com/milvus-io/milvus)                                       | 向量数据库               | OBS                                          | v2.5                             |      |
| 数据库     | C++    | [Doris](https://github.com/apache/doris)                                            | MPP 分析型数据库          | MRS                                          | v3.0                             |      |
| 数据库     | C++    | [ClickHouse](https://github.com/ClickHouse/ClickHouse)                              | 高性能列式数据库            | OBS                                          | v24.10                           |      |
| 通用应用    | Java   | [StreamSets](https://github.com/streamsets/datacollector-oss)                       | 数据流采集平台             | OBS                                          | v5.11                            |      |
| 通用应用    | Java   | [DataX](https://github.com/alibaba/DataX)                                           | 异构数据同步工具            | OBS                                          | v4.0                             |      |
| 数据流处理   | Java   | [Apache NiFi](https://github.com/apache/nifi)                                       | 数据流编排与可视化集成         | CCE、ECS、OBS、SMN                              | v1.27                            |      |
| 数据库     | Java   | [CrateDB](https://github.com/crate/crate)                                           | 分布式时序数据库            | OBS                                          | v5.9                             |      |
| API 网关  | Java   | [Apache ShenYu](https://github.com/apache/shenyu)                                   | 高性能 API 网关          | EulerOS、LTS                                  | v2.6                             |      |
| 调度与编排   | Java   | [Alluxio](https://github.com/Alluxio/alluxio)                                       | 数据缓存与分布式存储调度        | OBS                                          | v3.1                             |      |
| 持续集成交付  | Java   | [Jenkins](https://github.com/jenkinsci/jenkins)                                     | CI/CD 自动化构建与发布      | CodeArts Pipeline、CodeArts Check、VSS、OBS、SMN | v2.479                           |      |
| 运维监控    | Java   | [HertzBeat](https://github.com/dromara/hertzbeat)                                   | 云原生监控平台             | EulerOS、SMN                                  | v2.1                             |      |
| 运维监控    | Java   | [Jpom](https://github.com/dromara/Jpom)                                             | 项目部署与监控             | ECS                                          | v2.10                            |      |
| 流与消息    | Java   | [Apache Flink](https://github.com/apache/flink)                                     | 实时流计算与消息处理          | OBS                                          | v1.20                            |      |
| 流与消息    | Java   | [Apache Pulsar](https://github.com/apache/pulsar)                                   | 分布式消息系统             | OBS                                          | v3.3                             |      |
| 流与消息    | Java   | [Apache Heron](https://github.com/apache/incubator-heron)                           | 实时流式计算引擎            | OBS                                          | v0.24                            |      |
| 流与消息    | Java   | [Logstash](https://github.com/elastic/logstash)                                     | 日志收集与数据流处理          | OBS                                          | v8.15                            |      |
| 流与消息    | Java   | [Siddhi](https://github.com/siddhi-io/siddhi)                                       | 流事件处理引擎             | OBS                                          | v6.0                             |      |
| 通用应用    | Java   | [Apache Hadoop](https://github.com/apache/hadoop)                                   | 大数据分布式存储与计算         | OBS                                          | v3.4                             |      |
| 通用应用    | Java   | [Apache Flume](https://github.com/apache/flume)                                     | 数据采集与传输             | OBS                                          | v1.11                            |      |
| 通用应用    | Java   | [Apache Hive](https://github.com/apache/hive)                                       | 数据仓库查询引擎            | OBS                                          | v4.0                             |      |
| 通用应用    | Java   | [Apache Druid](https://github.com/apache/druid)                                     | 实时分析型数据库            | OBS                                          | v31.0                            |      |
| 通用应用    | Java   | [Apache Hudi](https://github.com/apache/hudi)                                       | 增量数据湖               | OBS、DIS                                      | v1.1                             |      |
| 通用应用    | Java   | [Apache Drill](https://github.com/apache/drill)                                     | SQL 查询引擎            | OBS                                          | v2.1                             |      |
| 通用应用    | Java   | [Pentaho Kettle](https://github.com/pentaho/pdi-ce)                                 | ETL 数据集成            | OBS                                          | v9.4                             |      |
| 通用应用    | Java   | [Seatunnel](https://github.com/apache/seatunnel)                                    | 数据集成与同步             | OBS                                          | v2.3                             |      |
| 通用应用    | Java   | [DeepStream](https://github.com/NVIDIA-AI-IOT/deepstream_reference_apps)            | 视频流分析框架             | OBS                                          | v7.1                             |      |
| 通用应用    | Java   | [zyplayer-doc](https://github.com/zyplayer/zyplayer-doc)                            | API 文档与知识中心         | OBS                                          | v3.3                             |      |
| 通用应用    | Java   | [Apache Iceberg](https://github.com/apache/iceberg)                                 | 表格式数据湖              | OBS                                          | v1.7                             |      |
| 通用应用    | Java   | [Hop](https://github.com/apache/hop)                                                | 数据集成与编排             | OBS                                          | v2.9                             |      |
| 通用应用    | Java   | [Rainbond](https://github.com/goodrain/rainbond)                                    | 云原生应用管理平台           | CCE                                          | v7.4                             |      |
| 通用应用    | Scala  | [Apache Spark](https://github.com/apache/spark)                                     | 分布式内存计算框架           | OBS                                          | v3.5                             |      |

---

## 使用说明

- 所有项目均基于 **开源社区版本** 进行华为云平台适配与测试。
- 使用指南目录中提供了 **详细的部署示例**、**配置说明**、以及 **在华为云上运行的注意事项**。

---

## 参与共建

欢迎社区开发者与企业用户参与生态适配项目的共建：

1. Fork 本仓库并提交 Pull Request；
2. 或通过 [Issue 区](https://github.com/HuaweiCloudDeveloper/oss-getting-started-on-huaweicloud/issues) 提交适配需求；
3. 提交时请附带开源项目名称、版本、适配场景说明等信息。

---

*本项目由华为云开发者生态团队维护，旨在推动主流开源项目在华为云平台的最佳实践落地。*

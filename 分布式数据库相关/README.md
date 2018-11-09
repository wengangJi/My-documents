Wayne
==========

loggo

**wayne**: 总体介绍，概略性描述.

[![GitHub stars]github start地址
[![Twitter Follow] twitter 开源follow
wayne 其他对外开放地址摘取



# 架构
**wayne** is an open source APM system, including monitoring, tracing, diagnosing capabilities for distributed system
in Cloud Native architecture. 
The core features are following.

- Service, service instance, endpoint metrics analysis
- Root cause analysis
- Service topology map analysis
- Service, service instance and endpoint dependency analysis
- Slow services and endpoints detected
- Performance optimization
- Distributed tracing and context propagation
- Alarm


架构图

SkyWalking supports to collect telemetry (traces and metrics) data from multiple sources
and multiple formats, 
including 
1. Java, .NET Core and NodeJS auto-instrument agents in SkyWalking format
1. Istio telemetry format
1. Zipkin v1/v2 formats


# Document
- [6.x Documents](docs/README.md). 

```
5.x is still supported by SkyWalking community, and the agent-backend protocol is compatible with 6.x.
You can go to 5.x branch. At there, you have everything you need.
```

- Go to [5.x pages](https://github.com/apache/incubator-skywalking/tree/5.x). Also 5.x document is [here](https://github.com/apache/incubator-skywalking/blob/5.x/docs/README.md).


# Downloads
Please head to the [releases page](http://skywalking.apache.org/downloads/) to download a release of Apache SkyWalking.


# Code of conduct
This project adheres to the Contributor Covenant [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. 
Please report unacceptable behavior to dev@skywalking.apache.org .

# Live Demo
- Host in Beijing. [goto](http://106.75.237.45:8080/)
  - Username: admin
  - Password: admin

# Screenshot
<table>
  <tr>
    <td width="50%" align="center"><b>Under javaagent observing</b></td>
    <td width="50%" align="center"><b>Observe on Istio</b></td>
  </tr>
  <tr>
    <td><img src="https://skywalkingtest.github.io/page-resources/6.0.0-alpha/Topology.png"/>
</td>
    <td><img src="https://skywalkingtest.github.io/page-resources/6.0.0-alpha/Istio/Topology.png"/>
</td>
   <tr>
     <td align="center"><a href="docs/Screenshots.md#agent">More screenshots</a></td>
     <td align="center"><a href="docs/Screenshots.md#istio">More screenshots</a></td>
  </tr>
</table>

# Compiling project
Follow this [document](docs/en/guides/How-to-build.md).

# Contact Us
* Submit an [issue](https://github.com/apache/incubator-skywalking/issues)
* Mail list: dev@skywalking.apache.org
* [Gitter](https://gitter.im/openskywalking/Lobby)
* QQ Group: 392443393

# Who Uses SkyWalking?
A wide variety of companies and organizations use SkyWalking for research, production and commercial product.
Here is the **User Wall** of SkyWalking.

<img src="https://skywalkingtest.github.io/page-resources/users/users-2018-11-02.png"/>

Users are encouraged to add themselves to the [PoweredBy](docs/powered-by.md) page.

<p align="center">
<a href="https://openapm.io"><img src="https://openapm.io/static/media/openapm_logo.svg" width="100"/></a> 
  <br/>Our project enriches the <a href="https://openapm.io">OpenAPM Landscape!</a>
</p>

# License
[Apache 2.0 License.](/LICENSE)

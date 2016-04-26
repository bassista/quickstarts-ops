# JBoss Fuse Quickstarts for Ops

A collection of sample configurations and scripts to showcase some of the typical JBoss Fuse configuration in Enterprise environments.

The example will verge mainly on the Operational aspects of JBoss Fuse, while [Quickstarts](https://github.com/jboss-fuse/fuse/tree/master/quickstarts) focus on the development aspects.

The aim of this initiative is to collect a set of scenarios that can be used by:

- Customers
- Consultants
- GSS
- QE
- Docs Team

to quickly provision and configure typical use cases.


Some of these information is *already covered by the official documentation*. What we are trying to do here is to turn that information in a quick step by step tutorial, adding when possible *re-usable scripts*.


## Scenarios

1. JBoss Fuse

   1. [HTTP Proxies](#http_proxies)
   2. [Corporate Maven Proxies](#maven_proxies)
   3. [LDAP integration](#ldap)
   4. [NO_INTERNET environments](#no_internet)
   5. [RBAC examples ](#rbac)
   6. [Hawtio restricted users](#hawtio)
   7. [External ZK Configuration](#zk)
   8. [External GIT repository](#git)
   9. [Change default ports](#ports)
   10. [SSL Configuration](#ssl)
   11. [Monitoring with Jolokia](#monitoring)
   12. [`resolver` configuration with multiple NICs](#resolvers)
   13. [Zookeeper HA](#zk_ha)
   14. [Loadbalancing](#loadbalancing)
   15. [Logging & Metrics](#logging_metrics)
   16. [Supervisor](#supervisor)
   17. [Security Policy](#external_security)
   18. [Authentication Examples](#authentication)
   19. [JVM Options and environment variables](#jvmopts_env_variables)

2. JBoss AMQ

   1. [persistente storage on a SAN](#amq_san)
   2. [LevelDB configuration](#amq_level)
   3. [External ZK Configuration](#amq_zk)
   4. [Websockets](#amq_websockets)


## 1. JBoss Fuse

### 1.1 HTTP Proxies <a id="http_proxies">&nbsp;</a>
- using Squid

### 1.2 Corporate Maven Proxies <a id="maven_proxies">&nbsp;</a>
[Details](02_maven_proxies/README.MD)

### 1.3 LDAP integration <a id="ldap">&nbsp;</a>
[Details](03_ldap/README.MD)

### 1.4 NO_INTERNET environments <a id="no_internet">&nbsp;</a>
[Details](04_no_internet/README.MD)
- edit maven proxies
- checking `iptables` possible issues

### 1.5 RBAC examples <a id="rbac">&nbsp;</a>
- a user that can just read logs?

### 1.6 Hawtio restricted users <a id="hawtio">&nbsp;</a>
- tweak non-admin users permissions

### 1.7 External ZK Configuration <a id="zk">&nbsp;</a>

### 1.8 External GIT repository <a id="git">&nbsp;</a>
[Details](08_external_git/README.MD)
- using either github or a plain `sshd` server

### 1.9 Change default ports <a id="ports">&nbsp;</a>
[Details](09_ports/README.MD)
- `minPort`, `maxPort`
- http port
- sshd port
- rmi port


### 1.10 SSL Configuration <a id="ssl">&nbsp;</a>
[Details](10_ssl/README.MD)
* Setup HTTPS/SSL for Jetty/Hawtio WebConsole
* Setup SSL transport for ActiveMQ broker
* Setup HTTPS/SSL for Camel and CXF endpoints


### 1.11 Monitoring with Jolokia <a id="monitoring">&nbsp;</a>
[Details](11_jolokia/README.MD)

### 1.12 `resolver` configuration with multiple NICs <a id="resolvers">&nbsp;</a>
[Details](12_resolvers/README.MD)
- complex network topologies
- AWS real use case

### 1.13 Zookeeper HA <a id="zk_ha">&nbsp;</a>
- Setup ensemble with 3, 5 Zk servers

### 1.14 Loadbalancing <a id="loadbalancing">&nbsp;</a>
- Integration with Big IP5, HTTP Mod_proxy loadbalancer

### 1.15 Logging & Metrics <a id="logging_metrics">&nbsp;</a>
- Insight topology (core & nodes)
- External elasticsearch
- Insight log
- Insight metrics
- Business monitoring

### 1.16 Supervisor <a id="supervisor">&nbsp;</a>
[Details](16_supervisor/README.MD)
- Integration with JON platform

### 1.17 Security Policy <a id="external_security">&nbsp;</a>
- Secure endpoints using ApiMan & Keycloak
- Export Fabric endpoints to Apiman (??)

### 1.18 Authentication Examples<a id="authentication">&nbsp;</a>
[Details](18_authentication/README.MD)

### 1.19 JVM Options and Environment Variables<a id="jvmopts_env_variables">&nbsp;</a>
[Details](19_jvmopts_env_variables/README.MD)

## 2. JBoss AMQ

### 2.1 persistent storage on a SAN <a id="amq_san">&nbsp;</a>

### 2.2 LevelDB configuration <a id="amq_level">&nbsp;</a>

### 2.3 External ZK Configuration <a id="amq_zk">&nbsp;</a>

### 2.4 Websockets  <a id="amq_websockets">&nbsp;</a>
- https://github.com/valdar/activemq-websocket-example

- 👋 Hi, I’m @MarioneMabilangan
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me Murion#6910

<!---
MarioneMabilangan/MarioneMabilangan is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
org.springframework.context.ApplicationContextException: Failed to start bean 'webServerStartStop'; nested exception is org.springframework.boot.web.server.WebServerException: Unable to start embedded Tomcat server
	at org.springframework.context.support.DefaultLifecycleProcessor.doStart(DefaultLifecycleProcessor.java:181) ~[spring-context-5.3.23.jar:5.3.23]
	at org.springframework.context.support.DefaultLifecycleProcessor.access$200(DefaultLifecycleProcessor.java:54) ~[spring-context-5.3.23.jar:5.3.23]
	at org.springframework.context.support.DefaultLifecycleProcessor$LifecycleGroup.start(DefaultLifecycleProcessor.java:356) ~[spring-context-5.3.23.jar:5.3.23]
	at java.base/java.lang.Iterable.forEach(Iterable.java:75) ~[na:na]
	at org.springframework.context.support.DefaultLifecycleProcessor.startBeans(DefaultLifecycleProcessor.java:155) ~[spring-context-5.3.23.jar:5.3.23]
	at org.springframework.context.support.DefaultLifecycleProcessor.onRefresh(DefaultLifecycleProcessor.java:123) ~[spring-context-5.3.23.jar:5.3.23]
	at org.springframework.context.support.AbstractApplicationContext.finishRefresh(AbstractApplicationContext.java:935) ~[spring-context-5.3.23.jar:5.3.23]
	at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:586) ~[spring-context-5.3.23.jar:5.3.23]
	at org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.refresh(ServletWebServerApplicationContext.java:147) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.boot.SpringApplication.refresh(SpringApplication.java:734) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.boot.SpringApplication.refreshContext(SpringApplication.java:408) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.boot.SpringApplication.run(SpringApplication.java:308) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.boot.SpringApplication.run(SpringApplication.java:1306) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.boot.SpringApplication.run(SpringApplication.java:1295) ~[spring-boot-2.7.5.jar:2.7.5]
	at com.m13.reprojecteFinal.GrupBProjecteFinalApplication.main(GrupBProjecteFinalApplication.java:10) ~[classes/:na]
Caused by: org.springframework.boot.web.server.WebServerException: Unable to start embedded Tomcat server
	at org.springframework.boot.web.embedded.tomcat.TomcatWebServer.start(TomcatWebServer.java:229) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.boot.web.servlet.context.WebServerStartStopLifecycle.start(WebServerStartStopLifecycle.java:43) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.context.support.DefaultLifecycleProcessor.doStart(DefaultLifecycleProcessor.java:178) ~[spring-context-5.3.23.jar:5.3.23]
	... 14 common frames omitted
Caused by: java.lang.IllegalArgumentException: standardService.connector.startFailed
	at org.apache.catalina.core.StandardService.addConnector(StandardService.java:238) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.springframework.boot.web.embedded.tomcat.TomcatWebServer.addPreviouslyRemovedConnectors(TomcatWebServer.java:282) ~[spring-boot-2.7.5.jar:2.7.5]
	at org.springframework.boot.web.embedded.tomcat.TomcatWebServer.start(TomcatWebServer.java:213) ~[spring-boot-2.7.5.jar:2.7.5]
	... 16 common frames omitted
Caused by: org.apache.catalina.LifecycleException: Protocol handler start failed
	at org.apache.catalina.connector.Connector.startInternal(Connector.java:1077) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.apache.catalina.util.LifecycleBase.start(LifecycleBase.java:183) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.apache.catalina.core.StandardService.addConnector(StandardService.java:234) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	... 18 common frames omitted
Caused by: java.net.BindException: L’adreça ja és en ús
	at java.base/sun.nio.ch.Net.bind0(Native Method) ~[na:na]
	at java.base/sun.nio.ch.Net.bind(Net.java:555) ~[na:na]
	at java.base/sun.nio.ch.ServerSocketChannelImpl.netBind(ServerSocketChannelImpl.java:337) ~[na:na]
	at java.base/sun.nio.ch.ServerSocketChannelImpl.bind(ServerSocketChannelImpl.java:294) ~[na:na]
	at org.apache.tomcat.util.net.NioEndpoint.initServerSocket(NioEndpoint.java:275) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.apache.tomcat.util.net.NioEndpoint.bind(NioEndpoint.java:230) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.apache.tomcat.util.net.AbstractEndpoint.bindWithCleanup(AbstractEndpoint.java:1227) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.apache.tomcat.util.net.AbstractEndpoint.start(AbstractEndpoint.java:1313) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.apache.coyote.AbstractProtocol.start(AbstractProtocol.java:617) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	at org.apache.catalina.connector.Connector.startInternal(Connector.java:1074) ~[tomcat-embed-core-9.0.68.jar:9.0.68]
	... 20 common frames omitted


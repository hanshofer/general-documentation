# TOMCAT 

### Add webapp (server.xml)

**Eclise plugin (add and remove...)**
```xml
<Host appBase="webapps" autoDeploy="true" name="localhost" unpackWARs="true">
   <Valve className="org.apache.catalina.valves.AccessLogValve" directory="logs" 
          pattern="%h %l %u %t &quot;%r&quot; %s %b" prefix="localhost_access_log." suffix=".txt"/>
   <Context docBase="service-endpoint" path="/service-endpoint" reloadable="true" 
	    source="org.eclipse.jst.jee.server:service-endpoint"/>
</Host>
```

**WAR application**
```xml
<Host appBase="webapps" autoDeploy="true" name="localhost" unpackWARs="true">
   <Valve className="org.apache.catalina.valves.AccessLogValve" directory="logs" 
          pattern="%h %l %u %t &quot;%r&quot; %s %b" prefix="localhost_access_log." suffix=".txt"/>
   <Context docBase="c:/data/workspaces/service-endpoint.war" path="/service-endpoint" reloadable="true"/>
</Host>
```

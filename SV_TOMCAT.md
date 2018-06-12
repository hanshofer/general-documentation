### Add webapp

**Eclise plugin (add and remove...)**
```xml
<Host appBase="webapps" autoDeploy="true" name="localhost" unpackWARs="true">
	<Valve className="org.apache.catalina.valves.AccessLogValve" directory="logs" pattern="%h %l %u %t &quot;%r&quot; %s %b" prefix="localhost_access_log." suffix=".txt"/>
	<Context docBase="c:/Data/workspaces/TEMP/activity-webservice/activity-service-endpoint/target/activity-service-endpoint-6.5.9.0.3-DCK-FTR-SNAPSHOT.war" path="/activity-service-endpoint" reloadable="true"/>
</Host>
```

**WAR application**
```xml
<Host appBase="webapps" autoDeploy="true" name="localhost" unpackWARs="true">
	<Valve className="org.apache.catalina.valves.AccessLogValve" directory="logs" pattern="%h %l %u %t &quot;%r&quot; %s %b" prefix="localhost_access_log." suffix=".txt"/>
	<Context docBase="c:/Data/workspaces/TEMP/activity-webservice/activity-service-endpoint/target/activity-service-endpoint-6.5.9.0.3-DCK-FTR-SNAPSHOT.war" path="/activity-service-endpoint" reloadable="true"/>
</Host>
```

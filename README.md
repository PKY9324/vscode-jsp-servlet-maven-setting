#vscode use jsp, servlet, maven
#install -> mvn compile -> mvn package

#how index page change localhost:port/
#open server setting (server.xml)

```xml
<Host name="localhost" appBase="webapps" unpackWARs="true" autoDeploy="true">
    <Context path="" docBase="yourAPP\target\yourAPP" reloadable="true"></Context>
    <Valve className="org.apache.catalina.valves.AccessLogValve" directory="logs" prefix="localhost_access_log" suffix=".txt" pattern="%h %l %u %t &quot;%r&quot; %s %b"/>
</Host>
```

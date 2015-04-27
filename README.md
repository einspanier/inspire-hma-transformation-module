# inspire-hma-transformation-module
Java Servlet-based transformation of HMA collection metadata to INSPIRE metadata and vice versa

## Build
1. Modify build.properties
* target.inspire.url: URL of an INSPIRE DS that has to be wrapped by a CIM EP facade
* target.cim.url: URL of a CIM EP service that has to be wrapped by an INSPIRE facade
* proxy.host: proxy to be used (if no proxy leave empty)
* proxy.port: port of proxy to be used (if no proxy leave empty)

2. Modify the capabilities document(s) inspireCapabilities and/or cimepCapabilities as desired

3. Modify log4j.xml as desired (optional).

4. Build via ant with build.xml (see http://ant.apache.org/).

## Deployment
Deploy in Servlet container (e.g. copy the generated war file from target folder to <tomcat>/webapps). Supported containers are Tomcat 6 and 7.
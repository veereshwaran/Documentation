# Tomcat
## Global
### Installation Type:
It defines the installation type to be use.
 * Repository Package: It is default OS repository package.
 * Binary Tarball: It is custom build from source build.
### Tomcat Installation Directory:
This mentions the where tomcat is installed. The default location is /opt.
### Binary distribution mirrors:
It defines the Apache Distribution compliant mirrors t be used.If it is not defined will use cloud apache mirror service.
### Version:
It defines the apache tomcat version.
### Build Version:
It defines the tomcat minor Version number.
### Webapps Directory:
This directory contains all web application files. Tomcat lookup this directory and run the application what are all in the webapps directory.
## Server
### User:
Specify the username for maintaining the tomcat process. If it is blank default OS specific username will be taken.
### Group:
Specify the group name for maintaining the tomcat process. If it is blank default OS specific group name will be taken.
### Sets the protocol to handle incoming traffic for Connector:
It is used to set connector type to handle the incoming connections.
 * **HTTP/1.1** - This Connector supports all of the required features of the HTTP/1.1 protocol, as described in RFC 2616, including persistent connections, pipelining, expectations and chunked encoding.
 * **Blocking Java Connector** -  The Java BIO connector will continue to wait for additional requests on the existing connector -- for keepalive HTTP requests.
 * **Non blocking java connector** - In this connector, the thread will go back into the thread pool immediately after the response is sent and it won't waste a thread on keepalive requests that may never arrive.
 * **APR/native connector** - When APR/native is enabled, the HTTPS connector will use a socket poller for keep-alive, increasing scalability of the server.
### Enable HTTP Connector:
It enables the HTTP connector. If it is not clicked the tomcat use SSL connector.
### Additional Attributes:
It is used to configure additional attributes for connector. There are more attributes are available.  
**Ex**
* **Timeout Period** - The number of milliseconds this Connector will wait, after accepting a connection, for the request URI line to be presented.
* **maxConnections** - The maximum connections that server will accept and process any given time.
### HTTP Port:
If tomcat uses HTTP connections then tomcat listens the incoming HTTP request on this port.
### SSL Port:
If tomcat uses SSL connections then tomcat listens incoming request on this port.
### Server Port:
This port is used for tomcat management server port.
### AJP Port:
This is port used by AJP connection.
### Environment Variables:
This environment variables are used by tomcat applications.
### Log Files Path:
This path is used to store the tomcat log files.
### Enable autoDelpoy:
If this option selected, during starting or restarting of tomcat all applications in tomcat automatically deployed.
### Add Context:
In Tomcat, the Context Container represents a single web application running within a given instance of Tomcat. Once a Context has been defined, Catalina will attempt to match incoming HTTP requests to its context path.
### Advanced Security Options:
When we click this option it will shows advanced security options for tomcat.  
**Ex.**
* Enable GET HTTP method: If it not chosen, tomcat do not accept the get request.
## Executor:
### Name:
This name represent the thread Pool in tomcat.
### Max Threads:
It means the maximum number of active threads in pool.
### Min Spare Threads:
It means the minimum number of threads in poll always keep alive.
### Java Options:
It is used to set the CATALINA_OPTS environment variable.
### System Properties:
It is used to set the -D argument to the JVM.
### Startup Parameter:
This Parameters are used when starting the tomcat.
### Max Heap Size:
It defines the maximum heap size.
### Start Heap Size:
It defines the heap size when tomcat is started.
### Specify the time limit to Shutdown the server:
It Specify the time the server should active.
## Security:
### User Security Manager:
It defines security manager. If it chose the user security is applied.
### Policy:
It defines the what are all the policies used in tomcat.
## Access Log
### Specify the directory in which access log files will be created:
This path mentioned the where the log files are stored. The generated log files are stored in that path.
### Log File Prefix:
This defines the log file name.
### Date format to place in log file name:
The mentioned time formats are used in log file.
### The suffix to be added to log file filenames:
This defines the log file types.
### Access log Formatting layout:
It is used to specify the log file pattern.
## Advanced
### Command to be executed before tomcat shutdown is invoked:
Command to be executed before catalina stop is invoked.
### Time(in seconds) to wait after the pre shut down is executed:
It will wait before catalina stop is executed after execution of pre shut down.
### Script to be executed after tomcat has been started:
The mentioned command is executed after tomcat has been. If it return 0 for successful execution. If it return 1 for failure which will cause tomcat startup to fail.
### Time(in seconds) to wait before executing post start up command:
This will controll at what frequency the post startup script will be executed.
### Max. Number of retries for executing post startup command:
The post startup script will be retried for max number of retries, executing the post startup script as per polling frequency.
# Dependencies
## Java
Tomcat 7 and 8 can run in Java 7 or later JRE.
Tomcat 6 can run in Java 5 or later JRE.
## logstash
## security group

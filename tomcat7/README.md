# Tomcat 7
This Docker image contains the Tomcat 7 servlet container. It is based off the
dsw88-java7 image.

# Using this image
To use this image, just add your WAR file to the /tomcat/webapps directory. Here's an
example of using this image

```
FROM dsw88/tomcat7

ADD path/to/your.war /tomcat/webapps
```

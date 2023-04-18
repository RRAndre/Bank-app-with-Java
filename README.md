# Bank-app-with-Java
There are 3 requirements to run this project on your machine:

1. To run this app please install Apache Tomcat 9 on your computer. If you have Apache version number 7 already installed, you just need to change the plugin on the pom file from 

\<plugin>
                \<groupId>org.apache.tomcat.maven\</groupId>
                \<artifactId>tomcat9-maven-plugin\</artifactId>
                \<version>4.0.0\</version>
                \<configuration>
                    \<url>http://localhost:8080/manager/text \</url>
                    \<server>tomcat\</server>
                    \<path>/javabank5\</path>
                \</configuration>
            \</plugin>

to 

\<plugin>
                \<groupId>org.apache.tomcat.maven\</groupId>
                \<artifactId>tomcat7-maven-plugin\</artifactId>
                \<version>2.2\</version>
                \<configuration>
                    \<url>http://localhost:8080/manager/text \</url>
                    \<server>tomcat\</server>
                    \<path>/javabank5\</path>
                \</configuration>
            \</plugin>". 

Please note the versions might be different and the plugin version might need to be updated. 

2. This is running on my side on the Apache Netbeans IDE 17 and no further configurations were required from the moment it was installed apart from adding the apache tomcat server to the list of available servers on Netbeans. 

3. Go to the javabank.properties file and change "dev.h2.location" to the path on your machine where you want to save the database file;


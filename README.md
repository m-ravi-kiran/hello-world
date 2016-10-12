API-AUTOMATION
==============

#About
+ API Testing script done using TestNG.

#Getting Started

To run tests you require maven, TestNG in Eclipse.

To generate a TestNG report you should perform following steps:
```bash
git clone -b auto https://github.com/delhivery/api-autommation.git
mvn clean compile
mvn package
java -jar target/ClientTest-0.0.1-SNAPSHOT-fat.jar -f=file_name.xml -config=config_name/config_name.config
```
To see a report open `/test-output/index.html` in your browser.

##Configurating files

###TestNG '.xml' file
`/suites/file_name.xml` <br />
Configure the xml file of TestNG by specifying the groups and classes in the suite tag. This will invoke the testing according to the details in file_name.xml file.

###Application Configuration Settings file 
`/config/config_name/config_name.config` <br />
Configure the .config file to suit a service. Specify the endpoint and the details of the Data Base being used.

###Initializing the Data Base


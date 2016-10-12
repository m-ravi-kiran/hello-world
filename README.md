API-AUTOMATION
==============

#About<br />
API Testing script done using TestNG.

#Getting Started

##Tools & Libraries
The test automation framework is comprised of following tools and libraries: <br />
JAVA: - Programming language  
TestNg: - TestNg Java testing framework  
Maven: - Build tool <br />
Github : - Git repository hosted server  
Eclipse: - Integrated Development Environment 

To generate a TestNG report you should perform following steps:
```bash
git clone -b auto https://github.com/delhivery/api-autommation.git
mvn clean install
mvn compile
mvn package
java -jar target/ClientTest-0.0.1-SNAPSHOT-fat.jar -f=file_name.xml -config=config_name/config_name.config
```
To see a TestNG report open `/test-output/index.html` in your browser.

##Configurating files

###TestNG '.xml' file
`/suites/file_name.xml` <br />
Configure the xml file (eg: file_name.xml) of TestNG by specifying the groups and classes in the suite tag. This will invoke the testing according to the details in file_name.xml file.

###Application Configuration Settings file 
`/config/config_name/config_name.config` <br />
Configure the .config file (eg: config_name/config_name.config) to suit a service. Specify the endpoint and the details of the Data Base being used.

###Initializing the Database
Add a table in Postgresql Database with the test data.
?? should include the keys required ??

###Test Cases
Write you TestNG test cases in the file .java with the @Test annotation.
```bash
@Test(groups = {"group_name"})
  public void testFunction() throws Exception {
  /*
  *Test Code here
  */
  }
```


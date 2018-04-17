---
published: true
---
## Project Object Model

1. POM is used for adding project dependencies. It comes as part of the Maven project setup.
2. SRC is the source folder. SRC Test java folder will contain only test cases. SRC main java folder will contain utilities,page classes,libraries etc.

3. Create individual package for each section(Example: Test data,Utilities,Base, config).

4. For reports, folder is created automatically.

5. Define common properties within the config package by creating a new file. Specifiy the URL,username and password and Browser details.

6. Inside the "Page" package, create all the pages.(Example: Login page,signup page,homepage)

## TestBase.java

Testbase.java file will be the base class for all the other java class files.This class will contain the details of the configuration file, code related to window maximization and code related to launching the URL.

![TestBase.png]({{site.baseurl}}/images/TestBase.png)


## Loginpage.java

Loginpage.java class contains **Object repositories, Page object initialization**(Pagefactory.initelements(driver,this)),**Actions**(validations like title name check, CRM image check), **login page**(with user name and password details that return Homepage class object.

![Loginpage.png]({{site.baseurl}}/images/Loginpage.png)

## Loginpagetest.java

This is a test case which contains test steps and which calls initialization method along with the super() which refers to base class constructor.

![loginpagetest]({{site.baseurl}}/images/Loginpagetest.png)

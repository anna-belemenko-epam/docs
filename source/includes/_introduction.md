# Introduction
## Simple JDI examples
### 1. Create simple Login test
For the beginning I would like to show you how tipycal problems can be solved with JDI. Let's start from Login, most of the tests starts from this you need to login on site.
Java code example can be found here: https://github.com/jdi-examples/jdi-introduction

Test Scenario
------
1) Open test site (https://epam.github.io/JDI/index.html)
2) Login as user
* Enter 'epam' in login textfield
* Enter '1234' in password textfield
* Press 'Enter' button
3) Validate that HomePage id openned
```java 
@Test
public void fillContactFormTest() {
    homePage.open();
    userIcon.click();
    loginForm.loginAs(DEFAULT_USER);
    homePage.checkOpened();
}
```
So simple!
But this is not all, just Run this test in your IDE and what you will get?
1. Detailed log in Console output:
```
[22:17.102  STEP] : Open 'Home Page'(url=https://epam.github.io/JDI/index.html)
[22:23.617  STEP] : Click on 'User Icon'
[22:23.727  STEP] : Login as User(userName:epam; password:1234)
[22:24.516  STEP] : Check that 'Home Page' is opened (url CONTAINS '/index.html'; title EQUALS 'Home Page')
```
Nice! Isn't it?
2. Same log in log file (src/test/.logs/) if you would like to see test execution results remotely (require log4j2.xml in src/test/resources)
3. Nice Allure report of your test execution! (require Allure settings in pom.xml)
![Allure Report](/images/allure-report.png)
![Allure Log](/images/allure-report-log.png)

Just move allure-results folder in target folder adn run maven > Plugins > allure > allure:serve
![Allure Serve](/images/allure-serve.png)

## Start new project with JDI
## How to improve your Selenium project with new capabilities in few minutes
## Logging and Reporting

# Documentation
## Extended Selenium features
TBD

## Simple elements
TBD

## Complex elements
### Table
[Test examples](https://github.com/jdi-testing/jdi-light-csharp/blob/master/JDI.Light/JDI.Light.Tests/Tests/Composite/TableTests.cs)
```java 
TBD
```
```csharp 
PerformancePage.UsersTable.AssertThat().HasRowWithValues(
                ContainsValue("Meyer", InColumn("Name")),
                ContainsValue("co.uk", InColumn("Email")));
```
```csharp 
PerformancePage.UsersTable.AssertThat().HasRowWithValues(
                ContainsValue("Meyer", InColumn(1)),
                ContainsValue("co.uk", InColumn(3)));
```
```csharp 
PerformancePage.UsersTable.AssertThat().HasRowWithValues(
                HasValue("Brian Meyer", InColumn("Name")),
                HasValue("mollis.nec@seddictumeleifend.co.uk", InColumn("Email")));
```
```csharp 
PerformancePage.UsersTable.AssertThat().HasRowWithValues(
                HasValue("Brian Meyer", InColumn(1)),
                HasValue("mollis.nec@seddictumeleifend.co.uk", InColumn(3)));
```
## Composite elements
TBD

## UI Objects
TBD

## JDI Locators
TBD

## Windows/Tabs manager
TBD

## Alerts
**Alert** –  a window with a message that displays on the screen and pauses the execution of the script until the user performs an action

<aside class="notice">
Note that you can make static import in order to simplify code Alerts.acceptAlert() > acceptAlert()
</aside>

Handle Window alerts/confirm/prompt dialogs desribed on <a href='https://developer.mozilla.org/en-US/docs/Web/API/Window' target="_blank">MDN</a>

```java 
alertButton.click();
acceptAlert();
```
```csharp 
AlertButton.Click();
AcceptAlert();
```
```java 
alertButton.click();
dismissAlert();
```
```csharp 
AlertButton.Click();
DismissAlert();
```

alert('Alert')
![Alert](/images/alert.png)

```java 
alertButton.click();
String text = getAlertText();
acceptAlert();
```
```csharp 
AlertButton.Click();
String text = GetAlertText();
AcceptAlert();
```
```java 
alertButton.click();
validateAlert(is("Red button"));
validateAlert(equalToIgnoringCase("red button"));
validateAlert(containsString("Red"));
```
```csharp 
TBD ValidateAlert
```

confirm()
![Confirmation dialog](/images/confirm.png)

```java 
alertButton.click();
inputAndAcceptAlert("Some Text");
```
```csharp 
TBD InputAndAcceptAlert
```

prompt('Alert', 'Default value')
![Prompt dialog](/images/prompt.png)


## Logs
TBD

## Reports
### Allure
TBD

### Report Portal
TBD

## JDI Settings
TBD

## Driver Settings
TBD

## Parallel tests run
TBD

## Remote test runs
TBD

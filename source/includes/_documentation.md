# Documentation
## Extended Selenium features
TBD

## Simple elements
TBD

## Complex elements
TBD

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
Handle Window alerts/confirm/prompt dialogs desribed on [MDN] https://developer.mozilla.org/en-US/docs/Web/API/Window_

alert('Alert')
![GitHub Logo](/images/alert.png)

### Methods
#### Accept Alert
```java 
alertButton.click();
acceptAlert();
```
confirm()
![GitHub Logo](/images/confirm.png)
#### Dismiss Alert
```java 
alertButton.click();
dismissAlert();
```
#### Get Alert Text
```java 
alertButton.click();
String text = getAlertText();
acceptAlert();
```
#### Validate Alert text
```java 
alertButton.click();
validateAlert(is("Red button"));
validateAlert(equalToIgnoringCase("red button"));
validateAlert(containsString("Red"));
```
prompt('Alert', 'Default value')
![GitHub Logo](/images/prompt.png)
#### Input and accept Alert
```java 
alertButton.click();
inputAndAcceptAlert("Some Text");
```

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

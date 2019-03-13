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
<aside class="notice">
This section is about working with alerts.
</aside>

**Alert** –  a window with a message that displays on the screen and pauses the execution of the script until the user performs an action.

Here is the list of available methods:

|Method | Description | Return Type
--- | --- | ---
**Ok()** |Accepts an alert  | void
**Cancel()** |Dismisses an alert  | void
**SendKeys()** |Sends key to the alert textbox  | void
**GetText()** |Returns the text displayed in the alert  | string

Action > Examples:

```csharp 
[Test]
public void CancelAlertExample() 
{
    MyPage.GetAlert().Cancel();
}

[Test]
public void GetAlertText() 
{
    Assert.AreEqual(MyPage.GetAlert().GetText(), "JDI Title");
}

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

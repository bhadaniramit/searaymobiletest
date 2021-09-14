Notes:
Appium Test - An Open source Tool for automating mobile application.
1. It helps in automating
* Web Bases Mobile application - Application on Mobile browser
* Native Mobile application - Calculator, Weather App, Searay App
* Hybrid Application - Application which can be both Native + Web Based
2. It supports Android, iOS, Windows based applications
3. Language supports: Python, Java, Php, JavaScript, Ruby, RobotFramework
4. Appium works as an client server architecture.
5. Appium is an HTTP Server written on Node.js platform
Appium Design:
WebDriver Script ---Webdriver Wire Protocol--->Appium HTTP Server---Native Automation Framework---> Mobile Device

Detailed design:
Appium script written in any language--->Webdriver JSON Wire Protocol---->
Appium Server Establish HTTP session with Client---->UIAutomation for iOS, UIAutomator2 for Android
--->Mobile Device(iOS/Android)

Native Automation Framework are:
UIAutomation for Apple
UIAutomator2 for Android
WinAppDriver for Microsoft

Desired Capabilities :
1. Set of Keys & Value pair sent to appium server to tell what kind of Automation Session user wanted
in starting up.
2. Desired Capabilities are sent with Apprium Script to Appium Server
3. Format of Desired Capabilities are in JSON
4. Desired Capabilities contains:
Platform Name: Name of Platform to automate
Platform Version : Version of platform to automate
Device Name: Device to automate
App: Path of App to automate(In case of Web Mobile Testing : BrowserName)
Automation Name: Name of driver to use (UIAutomation for iOS, UIAutomator2 for Android, WinAppDriver for Windows)

Sample of Desired Capabilities:
For Android:
{
“platformName”: “Android”,
“platformVersion”: “10.0”,
“deviceName”: “Samsung Galaxy Note10”,
“automationName”: “Appium”,
“app”: “path for the app under test”
}







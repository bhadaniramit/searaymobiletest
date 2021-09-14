Notes:
Appium Test - An Open source Tool for automating mobile application.
It helps in automating
1. Web Bases Mobile application - Application on Mobile browser
2. Native Mobile application - Calculator, Weather App, Searay App
3. Hybrid Application - Application which can be both Native + Web Based
It supports Android, iOS, Windows based
Appium Design:
WebDriver Script ---Webdriver Wire Protocol---> Appium HTTP Server -----Native Automation Framework----> Mobile Device

Detailed design:
Appium script written in any language--->Webdriver JSON Wire Protocol---->
Appium Server Establish HTTP session with Client---->UIAutomation for iOS, UIAutomator2 for Android
--->Mobile Device(iOS/Android)

Appium Support Native application via Framework
UIAutomation for Apple
UIAutomator2 for Android
WinAppDriver for Microsoft

Language supports: Python, Java, Php, JavaScript, Ruby, RobotFramework



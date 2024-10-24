This repository consists of Appium with Java Mobile Applications Automation Testing in OS's like Android & IOS and apps like Native, Hybrid, MobileWeb


Appium Intro

It uses Java library to write the code
it uses Android SDK to launch android virtual devices/emulators in Android Studio
It uses Node to communicate with the Appium Server

Appium Server Installation in Node 
open command prompt & run as administrator -> npm install -g appium
To start Appium Server -> appium (enter)(in cmd run as admin)
it says Welcome to Appium v2.5.4 .....
to install Appium server plugins -> appium plugin
Appium Server port --> 4723
Local Host --> 127.0.0.1
To list all Appium Drivers ->appium driver list
To install a driver -> appium driver install uiautomator2 //Android Apps Driver
appium driver install xcuitest //IOS Apps Driver

appium-inspector ---> A GUI inspector for mobile apps, it gives all the developer properties of selected elements like FindBy, Selector, accessibleId, xpath, Attributes & Values. scans all properties gives supported locators on the top

Configurations in Appium Inspector for Android
appium:app --> app location
appium:automationName --> UIAutomator2 (driver to automate Android Apps)
appium:deviceName --> RahulPhone
appium:eventTimings --> true
appium:platformName: android
Appium Server port --> 4723
Local Host --> 127.0.0.1
Start Appium Server
then start session in Appium-Inspector

Configurations in Appium Inspector for IOS
appium:app --> app location
appium:automationName --> XCUITest (driver to automate IOS Apps)
appium:deviceName --> iPhone 13 Pro
appium:platformName: IOS
appium:platformVersion: 15.5
Appium Server port --> 4723
Local Host --> 127.0.0.1
Start Appium Server
then start session in Appium-Inspector


OS ---> Android, IOS
apps---> apk, app package, app activity, app, bundle id
driver---> Android Driver, UIAutomator2, IOSDriver, XCUITest
apps---> native apps, hybrid apps, mobile web apps
app launch---> options.setApp(reinstalling for every test), launching app using app package & bundle id (No Reinstalling) or(Inbuilt Apps)
devices---> Virtual Devices(Android-->Emulator, IOS-->Simulator), Real Devices(Android & IOS)


Editor Tool Eclipse IDE - Install Appium, Selenium, TestNG
Set Java, SDK path, Node.js as Global Variables in Environment Variables
Appium Server - Install Appium Server using Node (npm install appium in cmd as admin, npm is set as global variable before step)
Driver - Install UIAutomator2 & XCUITest drivers in appium server (appium driver install in cmd) 
Virtual Devices - Android Studio-->Emulator, XCode-->Simulator (Windows only Android Studio, Mac both Android Studio & XCode)
Real Devices
Android - Settings>About Phone>Build Number(tap 7 times) it enables developer options and in developer options turn on USB Debugging
Go to cmd enter adb devices to see device connected or not. setDeviceName in Base Test
IOS - follow IOS Real Device Automation.docx
Locators - use Appium Inspector

Appium Code in Eclipse ----> Appium Server ----> Drivers(UIAutomator2 & XCUITest) ----> Perform Automation on Android or IOS Apps(Apps installed in Virtual or Real Devices)

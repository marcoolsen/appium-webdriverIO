# appium-webdriverIO

PoC using appium 2.x with WebDriverIO

## Features

 - Appium
 - WebDriverIO
 - Android
 - iOS
 - Page Object Model

## Run test
`npx wdio {config} --spec {filename}` run manually 

`npm run android` execute android tests

`npm run ios` execute ios tests

## Configuration

For the execution of the tests, I have created a shared configuration file using webdriverIO, so I can reuse various functions for both platforms. `wdio.shared.conf`

Android configuration is different from iOS so I have managed it in separate files. `wdio.android.conf` `wdio.ios.conf`

Also add a configuration file in case you need to add a cloud to run the tests in any device farm, such as BrowserStack, AWS, etc... `wdio.android.bs.conf`
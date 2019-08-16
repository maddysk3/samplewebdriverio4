WebDriverIO 4


First do npm init to create package .Jason file, enter the dependencies which you want to add to your project, for this project I added "selenium-standalone": "^6.16.0", "webdriverio": "^4.6.1” you can check the package.json file. 

Second npm install in the same folder

Third  start chrome driver and selenium server using following command

java -jar -Dwebdriver.chrome.driver=user/stack/drv/chromedriver selenium-server-standalone-3.141.59.jar

Check the path and selenium server version and do the changes and run this command in terminal. 

Once the server is up you can run your test 

IF YOU SEE BELOW ERROR 
{ Error: A new session could not be created.
    at end() - test.js:16:6
  details: undefined,
  message:
   'Unable to create new service: ChromeDriverService\nBuild info: version: \'3.14.0\', revision: \'aacccce0\', time: \'2018-08-02T20:13:22.693Z\'\nSystem info: host: \'Mireshs-MacBook-Pro.local\', ip: \'fe80:0:0:0:877:8320:bbbd:cbb8%en0\', os.name: \'Mac OS X\', os.arch: \'x86_64\', os.version: \'10.14.5\', java.version: \'1.8.0_131\'\nDriver info: driver.version: unknown',
  type: 'RuntimeError',
  seleniumStack:
   { type: 'SessionNotCreatedException',
     message: 'A new session could not be created.',
     orgStatusMessage:
      'Unable to create new service: ChromeDriverService\nBuild info: version: \'3.14.0\', revision: \'aacccce0\', time: \'2018-08-02T20:13:22.693Z\'\nSystem info: host: \'Mireshs-MacBook-Pro.local\', ip: \'fe80:0:0:0:877:8320:bbbd:cbb8%en0\', os.name: \'Mac OS X\', os.arch: \'x86_64\', os.version: \'10.14.5\', java.version: \'1.8.0_131\'\nDriver info: driver.version: unknown' } }

Just run Selenium standalone using command java -jar selenium-standalone 3.141.59.jar(you can use latest selenium standalone)
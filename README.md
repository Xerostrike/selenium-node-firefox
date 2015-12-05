# Selenium Grid Node - Firefox

Selenium Node configured to run Firefox

## Dockerfile

[Original Dockerfile](https://github.com/SeleniumHQ/docker-selenium/tree/master/NodeFirefox)

## With configuration of node

```
{
  "capabilities": [
    {
      "browserName": "firefox",
      "maxInstances": 10,
      "seleniumProtocol": "WebDriver"
    }
  ],
  "configuration": {
    "proxy": "org.openqa.grid.selenium.proxy.DefaultRemoteProxy",
    "maxSession": 10,
    "port": 5555,
    "register": true,
    "registerCycle": 5000,
    "timeout": 120,
    "browser": "firefox"
  }
}
```

## More information

[Grid parameters](https://code.google.com/p/selenium/source/browse/java/server/src/org/openqa/grid/common/defaults/GridParameters.properties)

[Default hub configuration](https://code.google.com/p/selenium/source/browse/java/server/src/org/openqa/grid/common/defaults/DefaultHub.json)

[Default node configuration](https://code.google.com/p/selenium/source/browse/java/server/src/org/openqa/grid/common/defaults/DefaultNode.json)
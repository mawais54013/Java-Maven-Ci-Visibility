## Ci-Visibility For Java-Gradle
 
## Compatibility 
JUnit >= 4.10 and >= 5.3<br/>
Also includes any test framework based on JUnit, such as Spock Framework and Cucumber-Junit
<br/>
<br/>
TestNG >= 6.4

# Prerequisites
 [Install the Datadog Agent to collect tests data](https://docs.datadoghq.com/continuous_integration/setup_tests/agent/?tab=azurepipelines)


[Install the Java tracer](https://github.com/DataDog/dd-trace-java) 


Command:
```
wget -O dd-java-agent.jar 'https://dtdg.co/latest-java-tracer'
```
<br/> 
Highly recommended to install Intellij to view java code:
https://www.jetbrains.com/idea/


## How to Use:
Run MVN command 
```
mvn compile 
```

Please refer to gif below for next steps:

<br/>
Run command below to run tests

```
DD_ENV=ci mvn clean verify -Pdd-civisibility
```

## Results:
Should be shown in datadog ci after a couple of minutes:
https://app.datadoghq.com/ci/test-runs?index=citest&start=1632627253983&end=1632630853983&paused=false

## Documentation
https://docs.datadoghq.com/continuous_integration/setup_tests/java/?tab=maven

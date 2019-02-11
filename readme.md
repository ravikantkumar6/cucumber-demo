# Cucumber 

### Setup

- Add gradle dependency in the gradle file.


	compile group: 'info.cukes', name: 'cucumber-spring', version: '1.2.5'
	compile group: 'info.cukes', name: 'cucumber-junit', version: '1.2.5'
- Create a class Cucumber runner.

```java
@RunWith(Cucumber.class)
@CucumberOptions(
        format = {"pretty","json:target/cucumber.json"},
        features = {"src/"}
)
public class CucumberRunner {
} 
```
- Create a feature file

```docker
Feature: Proof of concept to make cucmber framework integration

  Scenario: First Test case
    Given First step to add dependecy in gradle file
    When second step to create runner class
    Then create feature file
```

```Note :- check whether``` **```substeps intellij plug```** ```is installed or not if installed then remove it.```
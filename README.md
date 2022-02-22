# Introduction 
This Project will give you an overview of some new classes and helper methods we added that can help you write better test automation faster. We use Selenium/Appium (along with Java) for automating the test cases. 
The main purpose of Selenium/Appium is that it supports multiple browsers. Once a test case is automated, it can be run in any browser by changing the settings, so that the maintenance will be less. 
There are two different packages combined to in to Aurigo Masterworks Test Automation i.e., Aurigo Masterworks Test Framework, Aurigo Masterworks Tests. 
Each package has its own implementation for API, Mobile and Website for framework and tests. E.g. API has its own Base API Framework, which is inherited from Common Base Framework accessed by the other two modules.
 

# Getting Started
Installation process: Clone the specific repo from Git to your local workspace. Post that run the below maven goal, which would try to build the code.
    
     "mvn clean install" 
    
Software dependencies : Running the above command would download the required dependencies. In future if there is any change in the version of the dependency, please update the POM file accordingly.

# Build and Test
In order to run the tests, either run the specific TestNG xml files or run the below command (prior to that make sure the config files are updated as per the requirement) 

    "mvn test -DskipTests=false"
The above command on defaulted environment `qa` if no environment value is passed. In order to run tests on specific environment, pass the environment value as below:

`mvn test -DskipTest=false -Denvironment=qa`

Possible value for environment would be `qa` | `dev` : Accordingly the `config.<environment>'.properties` files needs to be updated.  
    
# Contribute
Before contributing, please make sure to go through the coding guidelines and act accordingly.

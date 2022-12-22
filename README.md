# Sonarqube to Swift proyect 2022


this repository is about how you can install Sonarqube in your machine and run the Unit test to Swift project and show the metrics


## Install SonarQube


1. Download 

Go to the folowind [link](https://www.sonarsource.com/products/sonarqube/downloads/) 
Remember, you need install Java JDK I recomend you Java11 

2. Run the server

open the terminal and run the following code

> `sh {your_directory}/sonarqube-xxx/bin/macosx-universal-64/sonar.sh start`

the server start in localhost:9000


## Install SonarScanner 

I prefer install sonar scanner by **BREW**. The command is

> `brew install sonar-scanner`

## All plugin Swfit 

In this repository you have a plugin to Sonarqube reads the iOS code 

	*backelite-sonar-swift-plugin-0.4.7*

Copy and page in the extension folder of Sonarqube. Restart the sonar server

## Run scan

To run the scanner 

`sonar-scanner \`
`  -Dsonar.projectKey=Sodexo \`
`  -Dsonar.sources=. \`
`  -Dsonar.host.url=http://localhost:9000 \`
`  -Dsonar.login=sqp_2b31e9f79c447e75a6a9a8b4f8d2fe563086bc2d \`
`  -X`
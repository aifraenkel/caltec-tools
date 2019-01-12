Scripts, tools and receipts that enable DevOps adoption
=======================================================

**Code Review - Continuous approach with Jenkins**

During the path to a continuous integration approach, automatic code review are key element to ensure code quality. SonarQuebe is an Open-source platform to do code reviews of different languages, enabling also to extend the AS-IS behaviour with plugins and custom rules generation. SonarQube has a client-server architecture where the client is the "sonar-runner" that runs a regression at client side and persist all the data in a sonar-qube server for analysis. Sonar-runner, the client, can be easily implemented with a jenkins-slave node. Jenkins-slave node will get the code for analysis, will run sonar-runner and then the analysis should be done in sonar-server. 

A continuous code revision approach can also be implemented, jenkins-slave jobs can be executed continuously with a plugin that understand when a sonar rule is an alert. This plugin can break a build and enable jenkins to take an action.



*How-To's*

SonarQube Plugins -> Para instalar los plugins es necesario compilar el plugin, copiarlo a la carpeta extensions de SonarQube y reiniciar el servicio.

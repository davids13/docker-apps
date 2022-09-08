## List of apps:
   - Jenkins
   - Nexus
   - Postgres
   - Sonarqube
   - Grafana & Prometheus


### Jenkins
**credentials:**
   - username: Admin 
   - password: the password can be found at: **/var/jenkins_home/secrets/initialAdminPassword**

___

### Nexus
**credentials:**
   - username: admin
   - password: the password can be found at: **/nexus-data/admin.password**
   
Nexus can be added in your java project and therefore it's possible to push an artifact into Nexus.<br>
**See:** https://www.baeldung.com/maven-deploy-nexus

___

### Sonarqube
**credentials:**
   - login: admin
   - password: admin

Sonarqube can be run locally in your java project.<br>
**Steps:**
   - Make sure you have a local instance up
   - The project must be already initialized by git
   - Add the dependency in plugin section: *https://mvnrepository.com/artifact/org.sonarsource.scanner.maven/sonar-maven-plugin*
   - Run the maven command in the root project: *mvn sonar:sonar -Dsonar.login=[your-sonar-token]*

___

Grafana
**credentials:**
   - login: admin
   - password: admin
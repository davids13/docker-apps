## List of apps:
   - Jenkins
   - Nexus
   - Postgres
   - Sonarqube

### Jenkins
**credentials:**
   - username: Admin 
   - password: the password can be found at: **/var/jenkins_home/secrets/initialAdminPassword**

### Nexus
**credentials:**
   - username: admin
   - password: the password can be found at: **/nexus-data/admin.password**

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

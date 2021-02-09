SonarQube Installation in Android Studio
1. First of all, download the latest version of SonarQube and unzip it.
2. After that open sonar qube directory folder \sonarqube-developer-7.9.1\sonarqube-7.9.1\bin\windows-x86-64 and run server on the shell by using StartSonar.bat file.  It'll take some time to run the server. 
3. Now, you can check server on the browser by using http://localhost:9000 path and you'll see following window.
https://1.bp.blogspot.com/-scjaiTmcVzs/XTwwR03zR1I/AAAAAAAAAxM/fxhJoyAyxgQjFOPjDNkww3184YEStJEZQCLcBGAs/s1600/sonar-dashboard.png
You can log in the admin panel by using admin/admin credential.

4. By default, sonar qube set some scan rule for our project. But we can customize it by using the Rules tab.
https://1.bp.blogspot.com/-lZtXVdjNngM/XTw8FsAMKfI/AAAAAAAAAxw/kvpDk9qx_BsQiuCzV1ZLOT9YvKJAb7LnACLcBGAs/s1600/sonar-qube-add-rules.png

Open terminal and type below command to execute sonarqube.gradle

gradlew sonarqube
After the task is success. Open browser and go to localhost:9000

Login with username/password.

In project dashboard you will be able to see the project with other details.

When will run gradlew sonarqube. it might throw below error
Execution failed for task ':app:sonarqube'.
> Unable to execute SonarQube

so to resolve make sure your local host (http://localhost:9000 ) is reachable.
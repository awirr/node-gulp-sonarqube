1. install docker
2. create sonarqube. run: docker run -d --name "name project" -p 9000:9000 sonarqube
3. install gulp. run: npm install --global gulp-cli
4. install projects node-gulp-sonarqube. run: npm install
5. to web browser run localhost:9000
6. to My Account -> Security -> Generate Tokens, copy token and keep token
7. update gulpfile.js
    - token: "",
    - options: {
        "sonar.projectBaseDir": "", Root project [C:/my-project]
        "sonar.working.directory": "", Root file sonar-scaner [C:/node-gulp-sonarqube/sonar-scaner]
      },
8. run: gulp default

Good luck


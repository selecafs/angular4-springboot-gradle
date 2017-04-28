# angular4-springboot-gradle

A tutorial for Angular4 + spring boot with gradle build

## The basic idea is
1. Create an angular project by using angular-cli.
2. 'ng build' to generate several bundle files.
3. Import the bundle files to spring boot project src/main/resources/public

## Tutorial
#### 1. Create an Angular2 project by using angular-cli
```bash
npm install -g @angular/cli
ng new PROJECT_NAME
cd PROJECT_NAME
ng serve
```

#### 2. Generate bundle files
```bash
ng build
```
bundle files are stored in dist/

#### 3. Import the bundle files to spring boot project
Copy files in dist/ folder to spring boot project src/main/resources/public folder.

If index.html is not used as the default entry point,
Move <app-root> and <script>bundle files from the generated index.html in dist/ to your spring project entry html file 


#### 4. upgrade angular2 to Angular4
Go to [upgrade guide](https://angular-update-guide.firebaseapp.com/),
select current angular version and desired angular version, and follow the instruction.

refers
http://angularjs.blogspot.com/2017/03/angular-400-now-available.html


#### 5. Build && run
```bash
Build: gradle build
Run: ./gradlew clean bootRun
```

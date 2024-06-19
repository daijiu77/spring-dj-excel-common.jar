First, Add references to your project that "spring-dj-excel-common.jar" itself depends on:<br>
[Click to see the references in the 'pom.xml'](/pom.xml)
<br>
download the package to your computer, and move the downloaded jar package to the specified directory of your project, assuming you put the jar in the lib directory of the root directory of the project, and add references to your Maven project pom.xml<br>
![dependency](https://github.com/daijiu77/spring-dj-excel-common.jar/assets/52983756/5c28dd41-46c0-4c85-ae62-72ce5b40a6d0)

And you need to modify the configuration of the 'build' tag to set 'includeSystemScope' to true

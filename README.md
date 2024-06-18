First, download the package to your computer, and move the downloaded jar package to the specified directory of your project, assuming you put the jar in the lib directory of the root directory of the project, and add references to your Maven project pom.xml<br>
  <dependency><br>
   <groupId>org.dj.excel</groupId><br>
   <artifactId>spring-dj-excel-common</artifactId><br>
   <version>0.0.1-SNAPSHOT</version><br>
   <scope>system</scope><br>
   <systemPath>${basedir}/lib/spring-dj-excel-common-0.0.1-SNAPSHOT.jar</systemPath><br>
 </dependency><br>
<br>
And you need to modify the configuration of the 'build' tag to set 'includeSystemScope' to true<br>
    <build><br>
        <plugins><br>
            <plugin><br>
                <groupId>org.springframework.boot</groupId><br>
                <artifactId>spring-boot-maven-plugin</artifactId><br>
                <configuration><br>
                    <includeSystemScope>true</includeSystemScope><br>
                </configuration><br>
            </plugin><br>
        </plugins><br>
    </build><br>

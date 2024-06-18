First, download the package to your computer, and move the downloaded jar package to the specified directory of your project, assuming you put the jar in the lib directory of the root directory of the project, and add references to your Maven project pom.xml
        <dependency>
            <groupId>org.dj.excel</groupId>
            <artifactId>spring-dj-excel-common</artifactId>
            <version>0.0.1-SNAPSHOT</version>
            <scope>system</scope>
            <systemPath>${basedir}/lib/spring-dj-excel-common-0.0.1-SNAPSHOT.jar</systemPath>
        </dependency>

And you need to modify the configuration of the 'build' tag to set 'includeSystemScope' to Tru
    <build>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
                <configuration>
                    <includeSystemScope>true</includeSystemScope>
                </configuration>
            </plugin>
        </plugins>
    </build>

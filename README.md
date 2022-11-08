# internship-checkstyle

## How To

1) Скопировать checkstyle.xml в корень проекта
2) Добавить в pom.xml конфигурацию:
```xml

<project>
    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-checkstyle-plugin</artifactId>
                <configuration>
                    <failsOnError>true</failsOnError>
                    <configLocation>checkstyle.xml</configLocation>
                    <consoleOutput>true</consoleOutput>
                </configuration>
            </plugin>
        </plugins>
    </build>
</project>
```
3) Запустить `mvn clean install` или `mvn checkstyle:checkstyle`.
4) Исправить ошибки
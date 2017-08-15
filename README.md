# maven-tiles

The [maven tiles](https://github.com/repaint-io/maven-tiles) used in SprintHive's projects. 

Each tile has a tile.xml and the contents can be merged into the pom of a given project by adding the tiles-maven-plugin to the project's pom with a reference to the wanted tile. For example, to add the code-quality tile:

```
<build>
    <plugins>
        ...
        <plugin>
            <groupId>io.repaint.maven</groupId>
            <artifactId>tiles-maven-plugin</artifactId>
            <version>2.10</version>
            <extensions>true</extensions>
            <configuration>
                <tiles>
                    <tile>com.sprinthive.tiles:code-quality:0.1</tile>
                </tiles>
            </configuration>
        </plugin>
    </plugins>
</build>
```

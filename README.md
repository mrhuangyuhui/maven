# Maven Manual

https://maven.apache.org/

http://search.maven.org/

https://mvnrepository.com/

## Examples

### [archetype:generate](https://maven.apache.org/archetype/maven-archetype-plugin/generate-mojo.html)
```bash
mvn archetype:generate
```

Filtering to reduce archetype list
```
# With a mojo parameter:
mvn archetype:generate -Dfilter=org.apache:struts

# Through the prompt:
mvn archetype:generate
Choose a number or apply filter (format: [groupId:]artifactId, case sensitive contains): org.apache:struts
```

Generate project in batch mode
```bash
mvn archetype:generate -B \
-DarchetypeGroupId=org.apache.maven.archetypes \
-DarchetypeArtifactId=maven-archetype-quickstart \
-DarchetypeVersion=1.1 \
-DgroupId=com.company \
-DartifactId=project \
-Dversion=1.0-SNAPSHOT \
-Dpackage=com.company.project
```

## Reference

[Plugins List](https://maven.apache.org/plugins/)

[POM Reference](https://maven.apache.org/ref/3.5.2/maven-model/maven.html)

[Lifecycle Reference](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html#Lifecycle_Reference)

[Built-in Lifecycle Bindings](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html#Built-in_Lifecycle_Bindings)

[Settings Reference](https://maven.apache.org/ref/3.5.2/maven-settings/settings.html)

[Maven Archetypes](https://maven.apache.org/archetypes/index.html)

[Standard Directory Layout](https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html)

[Maven Quick Reference Card](https://maven.apache.org/guides/MavenQuickReferenceCard.pdf)

## [Installation](https://maven.apache.org/install.html)

[Download](https://maven.apache.org/download.html) \
[Maven Releases History](https://maven.apache.org/docs/history.html)

### Linux

https://maven.apache.org/download.cgi

- #### [Binary](https://maven.apache.org/install.html)

[install-maven-bin.sh](https://github.com/mrhuangyuhui/maven/blob/master/install-maven-bin.sh)
```bash
sudo curl -L https://github.com/mrhuangyuhui/maven/raw/master/install-maven-bin.sh | sh
```

#### [SDKMAN](https://github.com/mrhuangyuhui/sdkman)
```bash
sdk list maven
sdk install maven 3.5.0
```

#### Package Manager
```bash
## APT ##
sudo apt update
apt show maven
sudo apt install maven -y
```

```bash
## YUM ##
yum info maven
sudo yum install maven -y
```

### Windows

https://maven.apache.org/download.cgi

Adding to `PATH`: Add the unpacked distribution’s bin directory to your user `PATH` environment variable by opening up the system properties (WinKey + Pause), selecting the “Advanced” tab, and the “Environment Variables” button, then adding or selecting the `PATH` variable in the user variables with the value `C:\Program Files\apache-maven-3.5.2\bin`. The same dialog can be used to set `JAVA_HOME` to the location of your JDK, e.g. `C:\Program Files\Java\jdk1.7.0_51`

```bash
mvn -v
```

## [Documentation](https://maven.apache.org/guides/)

### Getting Started with Maven

[Getting Started in 5 Minutes](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html)

[Getting Started in 30 Minutes](https://maven.apache.org/guides/getting-started/index.html)

### Introductions

[The Build Lifecycle](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html)

[The POM](https://maven.apache.org/guides/introduction/introduction-to-the-pom.html)

[Standard Directory Layout](https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html)

[The Dependency Mechanism](https://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html) 看到这里

### Guides

[Configuring Maven](https://maven.apache.org/guides/mini/guide-configuring-maven.html)

### References

## [Archetype](https://maven.apache.org/archetype/index.html)

```bash
mvn archetype:generate
```

```bash
mvn archetype:generate -Dfilter=org.apache:struts
```

```bash
mvn archetype:generate -B -DarchetypeGroupId=org.apache.maven.archetypes -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.1 -DgroupId=com.company -DartifactId=project -Dversion=1.0-SNAPSHOT -Dpackage=com.company.project
```

[Maven Archetype](https://maven.apache.org/archetype/index.html)

[Maven Archetype Plugin](https://maven.apache.org/archetype/maven-archetype-plugin/index.html)

[Project creation](https://maven.apache.org/archetype/maven-archetype-plugin/usage.html)

[archetype:generate](http://maven.apache.org/archetype/maven-archetype-plugin/generate-mojo.html)

[Generate project in batch mode](https://maven.apache.org/archetype/maven-archetype-plugin/examples/generate-batch.html)

[Generate project using an alternative catalog](https://maven.apache.org/archetype/maven-archetype-plugin/examples/generate-alternative-catalog.html)

[Maven Archetypes](https://maven.apache.org/archetypes/)

## Tutorials

[Maven Tutorial](https://www.tutorialspoint.com/maven/index.htm)





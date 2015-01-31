# missing-translation-checker-maven-plugin-usage
Example how to use the maven plugin to find missing translation

Look at the pom (https://github.com/samyBadjoudj/missing-translation-checker-maven-plugin-usage/blob/master/pom.xml)
to see how it is configured.

```
[WARNING] Can't find/open file /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/src/main/resources/MessagesBundle_de_US.properties

[WARNING] [Missing translations for /MessagesBundle_fr_FR.properties]
[WARNING] -> added.property

[WARNING] [Missing translations for MessagesBundle_de_DE.properties]
[WARNING] -> french.only.property
          -> added.property

```
```


samys-air:missing-translation-checker-maven-plugin-usage sbadjoudj$ mvn clean install
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building missing-translation-checker-maven-plugin-usage 1.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
Downloading: http://maven-repo.bugs3.com/com/samy/maven/plugin/missing-translation-checker-maven-plugin/1.0/missing-translation-checker-maven-plugin-1.0.pom
Downloaded: http://maven-repo.bugs3.com/com/samy/maven/plugin/missing-translation-checker-maven-plugin/1.0/missing-translation-checker-maven-plugin-1.0.pom (5 KB at 5.4 KB/sec)
Downloading: http://maven-repo.bugs3.com/com/samy/maven/plugin/missing-translation-checker-maven-plugin/1.0/missing-translation-checker-maven-plugin-1.0.jar
Downloaded: http://maven-repo.bugs3.com/com/samy/maven/plugin/missing-translation-checker-maven-plugin/1.0/missing-translation-checker-maven-plugin-1.0.jar (8 KB at 23.2 KB/sec)
[INFO]
[INFO] --- maven-clean-plugin:2.4.1:clean (default-clean) @ missing-translation-checker-maven-plugin-usage ---
[INFO]
[INFO] --- maven-resources-plugin:2.4.3:resources (default-resources) @ missing-translation-checker-maven-plugin-usage ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 4 resources
[INFO]
[INFO] --- maven-compiler-plugin:2.3.2:compile (default-compile) @ missing-translation-checker-maven-plugin-usage ---
[WARNING] File encoding has not been set, using platform encoding UTF-8, i.e. build is platform dependent!
[INFO] Compiling 1 source file to /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/target/classes
[INFO]
[INFO] --- missing-translation-checker-maven-plugin:1.0:check-translation (default) @ missing-translation-checker-maven-plugin-usage ---
[WARNING] Can't find/open file /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/src/main/resources/MessagesBundle_de_US.properties
[WARNING] [Missing translations for /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/src/main/resources/MessagesBundle_fr_FR.properties]
[WARNING] -> added.property

[WARNING] [Missing translations for /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/src/main/resources/MessagesBundle_de_DE.properties]
[WARNING] -> french.only.property
          -> added.property

[INFO]
[INFO] --- maven-resources-plugin:2.4.3:testResources (default-testResources) @ missing-translation-checker-maven-plugin-usage ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/src/test/resources
[INFO]
[INFO] --- maven-compiler-plugin:2.3.2:testCompile (default-testCompile) @ missing-translation-checker-maven-plugin-usage ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:2.7.2:test (default-test) @ missing-translation-checker-maven-plugin-usage ---
[INFO] No tests to run.
[INFO] Surefire report directory: /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/target/surefire-reports

-------------------------------------------------------
 T E S T S
-------------------------------------------------------
There are no tests to run.

Results :

Tests run: 0, Failures: 0, Errors: 0, Skipped: 0

[INFO]
[INFO] --- maven-jar-plugin:2.3.1:jar (default-jar) @ missing-translation-checker-maven-plugin-usage ---
[INFO] Building jar: /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/target/missing-translation-checker-maven-plugin-usage-1.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-install-plugin:2.3.1:install (default-install) @ missing-translation-checker-maven-plugin-usage ---
[INFO] Installing /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/target/missing-translation-checker-maven-plugin-usage-1.0-SNAPSHOT.jar to /Users/sbadjoudj/.m2/repository/com/samy/maven/plugin/missing-translation-checker-maven-plugin-usage/1.0-SNAPSHOT/missing-translation-checker-maven-plugin-usage-1.0-SNAPSHOT.jar
[INFO] Installing /Users/sbadjoudj/tp/missing-translation-checker-maven-plugin-usage/missing-translation-checker-maven-plugin-usage/pom.xml to /Users/sbadjoudj/.m2/repository/com/samy/maven/plugin/missing-translation-checker-maven-plugin-usage/1.0-SNAPSHOT/missing-translation-checker-maven-plugin-usage-1.0-SNAPSHOT.pom
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 4.376s
[INFO] Finished at: Sat Jan 31 18:14:47 CET 2015
[INFO] Final Memory: 12M/115M
[INFO] ------------------------------------------------------------------------
```

Samy Badjoudj

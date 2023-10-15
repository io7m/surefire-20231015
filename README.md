```
$ mvn package
[INFO] Scanning for projects...
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] surefire                                                           [pom]
[INFO] surefire.core                                                      [jar]
[INFO] surefire.tests                                                     [jar]
[INFO] 
[INFO] -----------------------< com.io7m.bugs:surefire >-----------------------
[INFO] Building surefire 20231015                                         [1/3]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.3.0:enforce (enforce-rules) @ surefire ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- buildnumber-maven-plugin:3.2.0:create (default) @ surefire ---
[INFO] Executing: /bin/sh -c cd '/home/rm/git/com.github/io7m/surefire-20231015' && 'git' 'rev-parse' '--verify' 'HEAD'
[INFO] Working directory: /home/rm/git/com.github/io7m/surefire-20231015
[INFO] Storing buildNumber: UNKNOWN at timestamp: 1697400527008
[INFO] Executing: /bin/sh -c cd '/home/rm/git/com.github/io7m/surefire-20231015' && 'git' 'symbolic-ref' 'HEAD'
[INFO] Working directory: /home/rm/git/com.github/io7m/surefire-20231015
[WARNING] Cannot get the branch information from the git repository: 
Detecting the current branch failed: fatal: not a git repository (or any of the parent directories): .git

[INFO] Executing: /bin/sh -c cd '/home/rm/git/com.github/io7m/surefire-20231015' && 'git' 'rev-parse' '--verify' 'HEAD'
[INFO] Working directory: /home/rm/git/com.github/io7m/surefire-20231015
[INFO] Storing scmBranch: UNKNOWN_BRANCH
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.10:prepare-agent (jacoco-agent) @ surefire ---
[INFO] argLine set to -javaagent:/home/rm/.m2/repository/org/jacoco/org.jacoco.agent/0.8.10/org.jacoco.agent-0.8.10-runtime.jar=destfile=/home/rm/git/com.github/io7m/surefire-20231015/target/jacoco.exec,append=true
[INFO] 
[INFO] --- build-helper-maven-plugin:3.4.0:parse-version (insert-version) @ surefire ---
[INFO] 
[INFO] --- maven-checkstyle-plugin:3.3.0:check (validate) @ surefire ---
[INFO] 
[INFO] --- bnd-maven-plugin:6.4.0:bnd-process (generate-osgi-manifest) @ surefire ---
[INFO] 
[INFO] --- maven-dependency-plugin:3.6.0:analyze-only (analyze) @ surefire ---
[INFO] Skipping plugin execution
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:jar-no-fork (default) @ surefire ---
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:test-jar-no-fork (default) @ surefire ---
[INFO] 
[INFO] --- reproducible-build-maven-plugin:0.16:strip-jar (reproducible-jar) @ surefire ---
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/target/surefire-20231015-javadoc.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/target/surefire-20231015-tests.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/target/surefire-20231015.jar
[INFO] 
[INFO] --- cyclonedx-maven-plugin:2.7.9:makeAggregateBom (default) @ surefire ---
[INFO] CycloneDX: Resolving Aggregated Dependencies
[INFO] CycloneDX: Creating BOM version 1.4 with 8 component(s)
[INFO] CycloneDX: Writing and validating BOM (XML): /home/rm/git/com.github/io7m/surefire-20231015/target/bom.xml
[INFO]            attaching as surefire-20231015-cyclonedx.xml
[INFO] 
[INFO] --------------------< com.io7m.bugs:surefire.core >---------------------
[INFO] Building surefire.core 20231015                                    [2/3]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.3.0:enforce (enforce-rules) @ surefire.core ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- buildnumber-maven-plugin:3.2.0:create (default) @ surefire.core ---
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.10:prepare-agent (jacoco-agent) @ surefire.core ---
[INFO] argLine set to -javaagent:/home/rm/.m2/repository/org/jacoco/org.jacoco.agent/0.8.10/org.jacoco.agent-0.8.10-runtime.jar=destfile=/home/rm/git/com.github/io7m/surefire-20231015/core/target/jacoco.exec,append=true
[INFO] 
[INFO] --- build-helper-maven-plugin:3.4.0:parse-version (insert-version) @ surefire.core ---
[INFO] 
[INFO] --- maven-checkstyle-plugin:3.3.0:check (validate) @ surefire.core ---
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:resources (default-resources) @ surefire.core ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/core/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:compile (default-compile) @ surefire.core ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- bnd-maven-plugin:6.4.0:bnd-process (generate-osgi-manifest) @ surefire.core ---
[INFO] 
[INFO] --- maven-dependency-plugin:3.6.0:analyze-only (analyze) @ surefire.core ---
[INFO] Skipping plugin execution
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:testResources (default-testResources) @ surefire.core ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/core/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:testCompile (default-testCompile) @ surefire.core ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.1.2:test (default-test) @ surefire.core ---
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:jar (default-jar) @ surefire.core ---
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015.jar
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:jar-no-fork (default) @ surefire.core ---
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:test-jar-no-fork (default) @ surefire.core ---
[INFO] No sources in project. Archive not created.
[INFO] 
[INFO] --- reproducible-build-maven-plugin:0.16:strip-jar (reproducible-jar) @ surefire.core ---
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-tests.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-sources.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-javadoc.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015.jar
[INFO] 
[INFO] --- cyclonedx-maven-plugin:2.7.9:makeAggregateBom (default) @ surefire.core ---
[INFO] CycloneDX: Resolving Dependencies
[INFO] CycloneDX: Creating BOM version 1.4 with 0 component(s)
[INFO] CycloneDX: Writing and validating BOM (XML): /home/rm/git/com.github/io7m/surefire-20231015/core/target/bom.xml
[INFO]            attaching as surefire.core-20231015-cyclonedx.xml
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:test-jar (test-jar) @ surefire.core ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-tests.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:jar (empty-javadoc-jar) @ surefire.core ---
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-javadoc.jar
[INFO] 
[INFO] --------------------< com.io7m.bugs:surefire.tests >--------------------
[INFO] Building surefire.tests 20231015                                   [3/3]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.3.0:enforce (enforce-rules) @ surefire.tests ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- buildnumber-maven-plugin:3.2.0:create (default) @ surefire.tests ---
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.10:prepare-agent (jacoco-agent) @ surefire.tests ---
[INFO] argLine set to -javaagent:/home/rm/.m2/repository/org/jacoco/org.jacoco.agent/0.8.10/org.jacoco.agent-0.8.10-runtime.jar=destfile=/home/rm/git/com.github/io7m/surefire-20231015/tests/target/jacoco.exec,append=true
[INFO] 
[INFO] --- build-helper-maven-plugin:3.4.0:parse-version (insert-version) @ surefire.tests ---
[INFO] 
[INFO] --- maven-checkstyle-plugin:3.3.0:check (validate) @ surefire.tests ---
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:resources (default-resources) @ surefire.tests ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/tests/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:compile (default-compile) @ surefire.tests ---
[INFO] Changes detected - recompiling the module! :dependency
[INFO] Compiling 2 source files with javac [debug release 20 module-path] to target/classes
[INFO] 
[INFO] --- bnd-maven-plugin:6.4.0:bnd-process (generate-osgi-manifest) @ surefire.tests ---
[INFO] 
[INFO] --- maven-dependency-plugin:3.6.0:analyze-only (analyze) @ surefire.tests ---
[INFO] Skipping plugin execution
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:testResources (default-testResources) @ surefire.tests ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/tests/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:testCompile (default-testCompile) @ surefire.tests ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.1.2:test (default-test) @ surefire.tests ---
[INFO] Using auto detected provider org.apache.maven.surefire.junitplatform.JUnitPlatformProvider
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.io7m.bugs.surefire.tests.ExampleTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.056 s -- in com.io7m.bugs.surefire.tests.ExampleTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:jar (default-jar) @ surefire.tests ---
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire.tests-20231015.jar
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:jar-no-fork (default) @ surefire.tests ---
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:test-jar-no-fork (default) @ surefire.tests ---
[INFO] No sources in project. Archive not created.
[INFO] 
[INFO] --- reproducible-build-maven-plugin:0.16:strip-jar (reproducible-jar) @ surefire.tests ---
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire.tests-20231015-sources.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire.tests-20231015-tests.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire.tests-20231015-javadoc.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire.tests-20231015.jar
[INFO] 
[INFO] --- cyclonedx-maven-plugin:2.7.9:makeAggregateBom (default) @ surefire.tests ---
[INFO] CycloneDX: Resolving Dependencies
[INFO] CycloneDX: Creating BOM version 1.4 with 7 component(s)
[INFO] CycloneDX: Writing and validating BOM (XML): /home/rm/git/com.github/io7m/surefire-20231015/tests/target/bom.xml
[INFO]            attaching as surefire.tests-20231015-cyclonedx.xml
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:test-jar (test-jar) @ surefire.tests ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire.tests-20231015-tests.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:jar (empty-javadoc-jar) @ surefire.tests ---
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire.tests-20231015-javadoc.jar
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary for surefire 20231015:
[INFO] 
[INFO] surefire ........................................... SUCCESS [  1.670 s]
[INFO] surefire.core ...................................... SUCCESS [  0.600 s]
[INFO] surefire.tests ..................................... SUCCESS [  1.123 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  3.475 s
[INFO] Finished at: 2023-10-15T20:08:49Z
[INFO] ------------------------------------------------------------------------
```

Then:


```
$ mvn -Dio7m.java.targetJavaVersion=21 package
[INFO] Scanning for projects...
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] surefire                                                           [pom]
[INFO] surefire.core                                                      [jar]
[INFO] surefire.tests                                                     [jar]
[INFO] 
[INFO] -----------------------< com.io7m.bugs:surefire >-----------------------
[INFO] Building surefire 20231015                                         [1/3]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.3.0:enforce (enforce-rules) @ surefire ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- buildnumber-maven-plugin:3.2.0:create (default) @ surefire ---
[INFO] Executing: /bin/sh -c cd '/home/rm/git/com.github/io7m/surefire-20231015' && 'git' 'rev-parse' '--verify' 'HEAD'
[INFO] Working directory: /home/rm/git/com.github/io7m/surefire-20231015
[INFO] Storing buildNumber: UNKNOWN at timestamp: 1697400614140
[INFO] Executing: /bin/sh -c cd '/home/rm/git/com.github/io7m/surefire-20231015' && 'git' 'symbolic-ref' 'HEAD'
[INFO] Working directory: /home/rm/git/com.github/io7m/surefire-20231015
[WARNING] Cannot get the branch information from the git repository: 
Detecting the current branch failed: fatal: not a git repository (or any of the parent directories): .git

[INFO] Executing: /bin/sh -c cd '/home/rm/git/com.github/io7m/surefire-20231015' && 'git' 'rev-parse' '--verify' 'HEAD'
[INFO] Working directory: /home/rm/git/com.github/io7m/surefire-20231015
[INFO] Storing scmBranch: UNKNOWN_BRANCH
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.10:prepare-agent (jacoco-agent) @ surefire ---
[INFO] argLine set to -javaagent:/home/rm/.m2/repository/org/jacoco/org.jacoco.agent/0.8.10/org.jacoco.agent-0.8.10-runtime.jar=destfile=/home/rm/git/com.github/io7m/surefire-20231015/target/jacoco.exec,append=true
[INFO] 
[INFO] --- build-helper-maven-plugin:3.4.0:parse-version (insert-version) @ surefire ---
[INFO] 
[INFO] --- maven-checkstyle-plugin:3.3.0:check (validate) @ surefire ---
[INFO] 
[INFO] --- bnd-maven-plugin:6.4.0:bnd-process (generate-osgi-manifest) @ surefire ---
[INFO] 
[INFO] --- maven-dependency-plugin:3.6.0:analyze-only (analyze) @ surefire ---
[INFO] Skipping plugin execution
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:jar-no-fork (default) @ surefire ---
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:test-jar-no-fork (default) @ surefire ---
[INFO] 
[INFO] --- reproducible-build-maven-plugin:0.16:strip-jar (reproducible-jar) @ surefire ---
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/target/surefire-20231015-javadoc.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/target/surefire-20231015-tests.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/target/surefire-20231015.jar
[INFO] 
[INFO] --- cyclonedx-maven-plugin:2.7.9:makeAggregateBom (default) @ surefire ---
[INFO] CycloneDX: Resolving Aggregated Dependencies
[INFO] CycloneDX: Creating BOM version 1.4 with 8 component(s)
[INFO] CycloneDX: Writing and validating BOM (XML): /home/rm/git/com.github/io7m/surefire-20231015/target/bom.xml
[INFO]            attaching as surefire-20231015-cyclonedx.xml
[INFO] 
[INFO] --------------------< com.io7m.bugs:surefire.core >---------------------
[INFO] Building surefire.core 20231015                                    [2/3]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.3.0:enforce (enforce-rules) @ surefire.core ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- buildnumber-maven-plugin:3.2.0:create (default) @ surefire.core ---
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.10:prepare-agent (jacoco-agent) @ surefire.core ---
[INFO] argLine set to -javaagent:/home/rm/.m2/repository/org/jacoco/org.jacoco.agent/0.8.10/org.jacoco.agent-0.8.10-runtime.jar=destfile=/home/rm/git/com.github/io7m/surefire-20231015/core/target/jacoco.exec,append=true
[INFO] 
[INFO] --- build-helper-maven-plugin:3.4.0:parse-version (insert-version) @ surefire.core ---
[INFO] 
[INFO] --- maven-checkstyle-plugin:3.3.0:check (validate) @ surefire.core ---
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:resources (default-resources) @ surefire.core ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/core/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:compile (default-compile) @ surefire.core ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- bnd-maven-plugin:6.4.0:bnd-process (generate-osgi-manifest) @ surefire.core ---
[INFO] 
[INFO] --- maven-dependency-plugin:3.6.0:analyze-only (analyze) @ surefire.core ---
[INFO] Skipping plugin execution
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:testResources (default-testResources) @ surefire.core ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/core/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:testCompile (default-testCompile) @ surefire.core ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.1.2:test (default-test) @ surefire.core ---
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:jar (default-jar) @ surefire.core ---
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015.jar
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:jar-no-fork (default) @ surefire.core ---
[INFO] 
[INFO] --- maven-source-plugin:3.3.0:test-jar-no-fork (default) @ surefire.core ---
[INFO] No sources in project. Archive not created.
[INFO] 
[INFO] --- reproducible-build-maven-plugin:0.16:strip-jar (reproducible-jar) @ surefire.core ---
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-tests.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-sources.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-javadoc.jar
[INFO] Stripping /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015.jar
[INFO] 
[INFO] --- cyclonedx-maven-plugin:2.7.9:makeAggregateBom (default) @ surefire.core ---
[INFO] CycloneDX: Resolving Dependencies
[INFO] CycloneDX: Creating BOM version 1.4 with 0 component(s)
[INFO] CycloneDX: Writing and validating BOM (XML): /home/rm/git/com.github/io7m/surefire-20231015/core/target/bom.xml
[INFO]            attaching as surefire.core-20231015-cyclonedx.xml
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:test-jar (test-jar) @ surefire.core ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-tests.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.3.0:jar (empty-javadoc-jar) @ surefire.core ---
[INFO] Building jar: /home/rm/git/com.github/io7m/surefire-20231015/core/target/surefire.core-20231015-javadoc.jar
[INFO] 
[INFO] --------------------< com.io7m.bugs:surefire.tests >--------------------
[INFO] Building surefire.tests 20231015                                   [3/3]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.3.0:enforce (enforce-rules) @ surefire.tests ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- buildnumber-maven-plugin:3.2.0:create (default) @ surefire.tests ---
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.10:prepare-agent (jacoco-agent) @ surefire.tests ---
[INFO] argLine set to -javaagent:/home/rm/.m2/repository/org/jacoco/org.jacoco.agent/0.8.10/org.jacoco.agent-0.8.10-runtime.jar=destfile=/home/rm/git/com.github/io7m/surefire-20231015/tests/target/jacoco.exec,append=true
[INFO] 
[INFO] --- build-helper-maven-plugin:3.4.0:parse-version (insert-version) @ surefire.tests ---
[INFO] 
[INFO] --- maven-checkstyle-plugin:3.3.0:check (validate) @ surefire.tests ---
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:resources (default-resources) @ surefire.tests ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/tests/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:compile (default-compile) @ surefire.tests ---
[INFO] Changes detected - recompiling the module! :dependency
[INFO] Compiling 2 source files with javac [debug release 21 module-path] to target/classes
[INFO] 
[INFO] --- bnd-maven-plugin:6.4.0:bnd-process (generate-osgi-manifest) @ surefire.tests ---
[INFO] 
[INFO] --- maven-dependency-plugin:3.6.0:analyze-only (analyze) @ surefire.tests ---
[INFO] Skipping plugin execution
[INFO] 
[INFO] --- maven-resources-plugin:3.3.1:testResources (default-testResources) @ surefire.tests ---
[INFO] skip non existing resourceDirectory /home/rm/git/com.github/io7m/surefire-20231015/tests/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.11.0:testCompile (default-testCompile) @ surefire.tests ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.1.2:test (default-test) @ surefire.tests ---
[INFO] Using auto detected provider org.apache.maven.surefire.junitplatform.JUnitPlatformProvider
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.io7m.bugs.surefire.tests.ExampleTest
[ERROR] Tests run: 1, Failures: 1, Errors: 0, Skipped: 0, Time elapsed: 0.061 s <<< FAILURE! -- in com.io7m.bugs.surefire.tests.ExampleTest
[ERROR] com.io7m.bugs.surefire.tests.ExampleTest.test -- Time elapsed: 0.041 s <<< FAILURE!
org.opentest4j.AssertionFailedError: expected: <3> but was: <0>
	at org.junit.jupiter.api.AssertionFailureBuilder.build(AssertionFailureBuilder.java:151)
	at org.junit.jupiter.api.AssertionFailureBuilder.buildAndThrow(AssertionFailureBuilder.java:132)
	at org.junit.jupiter.api.AssertEquals.failNotEqual(AssertEquals.java:197)
	at org.junit.jupiter.api.AssertEquals.assertEquals(AssertEquals.java:150)
	at org.junit.jupiter.api.AssertEquals.assertEquals(AssertEquals.java:145)
	at org.junit.jupiter.api.Assertions.assertEquals(Assertions.java:527)
	at com.io7m.bugs.surefire.tests.ExampleTest.test(ExampleTest.java:30)
	at java.base/java.lang.reflect.Method.invoke(Method.java:580)
	at java.base/java.util.ArrayList.forEach(ArrayList.java:1596)
	at java.base/java.util.ArrayList.forEach(ArrayList.java:1596)

[INFO] 
[INFO] Results:
[INFO] 
[ERROR] Failures: 
[ERROR]   ExampleTest.test:30 expected: <3> but was: <0>
[INFO] 
[ERROR] Tests run: 1, Failures: 1, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary for surefire 20231015:
[INFO] 
[INFO] surefire ........................................... SUCCESS [  1.589 s]
[INFO] surefire.core ...................................... SUCCESS [  0.624 s]
[INFO] surefire.tests ..................................... FAILURE [  0.975 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD FAILURE
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  3.285 s
[INFO] Finished at: 2023-10-15T20:10:16Z
[INFO] ------------------------------------------------------------------------
[ERROR] Failed to execute goal org.apache.maven.plugins:maven-surefire-plugin:3.1.2:test (default-test) on project surefire.tests: There are test failures.
[ERROR] 
[ERROR] Please refer to /home/rm/git/com.github/io7m/surefire-20231015/tests/target/surefire-reports for the individual test results.
[ERROR] Please refer to dump files (if any exist) [date].dump, [date]-jvmRun[N].dump and [date].dumpstream.
[ERROR] -> [Help 1]
[ERROR] 
[ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch.
[ERROR] Re-run Maven using the -X switch to enable full debug logging.
[ERROR] 
[ERROR] For more information about the errors and possible solutions, please read the following articles:
[ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/MojoFailureException
[ERROR] 
[ERROR] After correcting the problems, you can resume the build with the command
[ERROR]   mvn <args> -rf :surefire.tests
```

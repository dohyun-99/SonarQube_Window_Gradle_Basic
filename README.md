# SonarScanner for Gradle

This example demonstrates how to analyze a simple project built with [Gradle](https://gradle.org/). See [SonarScanner for Gradle](https://docs.sonarsource.com/sonarqube/latest/analyzing-source-code/scanners/sonarscanner-for-gradle/) for more information.

## Prerequisites
* A gradle wrapper is included that bundles gradle. All other required plugins will be pulled by gradle as needed.

## Coverage

To get the project [test coverage](https://community.sonarsource.com/t/coverage-test-data-importing-jacoco-coverage-report-in-xml-format) computed, add gradle task `jacocoTestReport` to your command line.

* On Windows:
  ```text
  gradlew.bat build jacocoTestReport -D"sonar.host.url=http://localhost:9000" -D"sonar.token=<발급한 sonarqube token>" sonar
  ```

## sonar-scanner.properties
해당 파일은 실제 sonar-scanner로 코드 분석을 실행할 때 사용하는 파일을 업로드 한 것 입니다.  
sonar-scanner 로컬 설치 후, cmd에서 해당 설치된 sonar-scanner폴더\bin 이동 후 아래 명령어로 실행하면 됩니다.
  ```bash
  sonar-scanner.bat
  ```

# webProject

The test automation project for [Hostegram website] https://hostegram.com/
<p align="center">
  <img src="images/screenshot/hostegramDashboard.JPG">
</p>


<p  align="center" p>

<code>
<img width="5%" title="Java" src="images/logo/Java_icon.png">
<img width="5%" title="Gradle" src="images/logo/Gradle_icon.svg">
<img width="5%" title="IntelliJ IDEA" src="images/logo/Intellij_icon.png">
<img width="5%" title="Selenide" src="images/logo/Selenide_icon.svg">
<img width="5%" title="Selenoid" src="images/logo/Selenoid_icon.svg">
<img width="5%" title="JUnit5" src="images/logo/JUnit5_icon.png">
<img width="5%" title="Github" src="images/logo/Github_icon.png">
<img width="5%" title="Jenkins" src="images/logo/Jenkins_icon.svg">
<img width="5%" title="Allure Report" src="images/logo/Allure_Report_icon.svg">
<img width="5%" title="Allure TestOps" src="images/logo/Allure_TestOps_icon.svg">
<img width="5%" title="Telegram" src="images/logo/Telegram_icon.png">
<img width="5%" title="Jira" src="images/logo/Jira_icon.png">
</code>
</p>

___

## Run tests from terminal locally

### Run tests with filled remote properties:

```bash
gradle clean test
```

### Run tests without filled remote properties:

```bash
gradle clean test

-Dbrowser=${BROWSER}
-DbrowserVersion=${BROWSER_VERSION}
-DbrowserSize=${BROWSER_SIZE}
```

### Serve report:

```bash
allure serve build/allure-results
```

___

## Results 

The test results can be found in:
+ [Jenkins](#jenkins)
+ [Allure Report](#allure-report)
+ [Allure TestOps](#allure-testOps)


### [Jenkins](https://jenkins.autotests.cloud/job/09-elenakomarova-itfinland-project-ui/build?delay=0sec)

For the running autotests in Jenkins, you can specify the parameters described
in :point_up:  [Run tests without filled remote properties](#run-tests-without-filled-remote-properties).


<p align="center">
  <img src="images/screenshot/jenkinsScreen.JPG">
</p>

Once the launch is finished you may watch statistics and open the `Allure Report` <img width="2%" title="Allure Report" src="images/logo/Allure_Report_icon.svg">

<p align="center">
  <img src="images/screenshot/jenkinsScreen1.JPG">
</p>

### Allure Report

Here are the examples of a report about test build with grouping by tags (:point_up: [The list of tests grouped by tag parameter](#the-list-of-tests-grouped-by-tag-parameter))

:arrow_right: [The launch with results for tag = main_page](https://jenkins.autotests.cloud/job/09-elenakomarova-itfinland-project-ui/93/allure/)

<p align="center">
  <img src="images/screenshot/allureReport/JPG">
</p>

:arrow_right: [The launch with results for tag = top_menu](https://jenkins.autotests.cloud/job/09-elenakomarova-itfinland-project-ui/94/allure/)

<p align="center">
  <img src="images/screenshot/allureReport1.JPG">
</p>

### Allure TestOps

Allure TestOps is used as a storage for all tests cases (automated and manual), launches, their results. You may watch statistic and reports by all launches and results

:arrow_right: Dashboards:

<p align="center">
  <img src="images/screenshot/allureTestOps.JPG">
</p>

<p align="center">
  <img src="images/screenshot/allureTestOps1.JPG">
</p>

___

## Example of video with test running in Allure Report

You may see the example of a video showing the test run in Allure report.

<p align="center">
  <img src="images/screenshot/telegramNotification.JPG">
</p>


___

## Notifications in Telegram channel

The project is configured to send notifications about the results of launches from Jenkins to Telegram channel

<p align="center">
  <img src="images/screens/Telegram_failed_notification.PNG">
</p>

<p align="center">
  <img src="images/screens/Telegram_passed_notification.PNG">
</p>


___

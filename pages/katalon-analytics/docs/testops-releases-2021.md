---
title: "Katalon TestOps 2021 Releases" 
sidebar: katalon_studio_docs_sidebar
permalink: /katalon-analytics/docs/testops-releases-2021.html
redirect from: 
    - "/katalon-studio/docs/docs/core-1.x.html"
    - "/katalon-analytics/docs/docs/core-1.x.html"
    - "/katalon-analytics/docs/core-1.0.html"
    - "/katalon-analytics/docs/advanced-0.1.x.html"
description:
---
 
## Latest Release - July 26th, 2021

### New Features

- Introduced Auto-distributed execution. Users can automatically distribute tasks to active and available Agents. Learn more: [Auto-Distributed Execution](https://docs.katalon.com/katalon-analytics/docs/auto-distributed-execution.html)

- Introduced Test Usage Validation. Users can view how many test runs remain until their subscription quota is capped. Learn more: [View Test Usage and Balance in the Usage Dashboard](docs.katalon.com/katalon-analytics/docs/test-usage-balance-usage-dashboard.html)

### Enhancements

- Added verification to attachments when uploading test cases
- Made access logs sortable by date range
- Enhanced component release summary
- Updated access log api exporting function to return csv file
- Enabled component to show test percentage in release readiness
- Applied feature flag for release readiness
- Enhanced wizard for framework integration
- Build visible under Configuration section for each Test Run

### Fixes

- Could not filter API log by timestamp.
- testRuns \(Number of test runs\) field could be manipulated into invalid values.
- Long pending messages in Retry function.
- Path Injection, Zip Slip vulnerabilities.
- Occurences where the app would break because of a missing LD config file.
- Uncommon error when creating thumbnail.
- User could fetch other organization's invoices from Payment Success screen.
- Week/day view of calendar would show wrong test runs when updating time zone.
- Manually uploading Katalon Reports in TestOps sometimes failed.
- Agent could not override Execution Mode of Test Suite Collection when executing with KRE 8.0 \ 8.0.5 versions.

- Removed: polling message prompts for certain errors.

## June 22nd

### New features

- Added Re-run Test Results to the Test Results summary. See: [View Re-run Test Results in TestOps](https://docs.katalon.com/katalon-analytics/docs/rerun-results.html).

### Enhancements

-Updated maintainer column in Flaky Test list.
-Updated UI for Integration function.
-Enhanced security when updating Git test projects.

### Fixes

- Fixed a bug where users could not:
  - migrate subscriptions.
  - send an invitation email.
  - calculate statistics for empty Test Runs.
  - download a large Test Run as .xsls file.
  - delete the execution.

- Fixed the missing profile name on the execution page.
- Fixed search field for execution that doesn't re-run.
- Clarified the message for adding Users to Teams successfully.

## May 26th

### Improvements

- Filter test runs by Build Name. [Learn more](https://docs.katalon.com/katalon-analytics/docs/filter-test-build-name.html)

- View Release Readiness in TestOps Dashboard. [Learn more](https://docs.katalon.com/katalon-analytics/docs/dashboard-overview.html)

## April 26

### New features

- Integration with Pytest. [Learn more](https://docs.katalon.com/katalon-analytics/docs/kt-upload-test-pytest.html)

- Integration with Kobiton. [Learn more](https://docs.katalon.com/katalon-analytics/docs/kt_kobiton_integration.html)

- Test Suite-based parallel execution. [Learn more](https://docs.katalon.com/katalon-analytics/docs/kt_run_parallel_agent.html)

### Improvements

- New release of Katalon agent version 1.7.

- Improve performance for Test Planning calendar view.

See [What's new in April Release?](https://docs.katalon.com/katalon-analytics/docs/kte-whats-new-in-april-release.html)

## March 8

### New features

- Introduce a new term — Build —  that is used in Katalon TestOps. Learn more about the definition of Build [here](/katalon-analytics/docs/testops-terminology.html).

- Create and manage Builds in Test Planning. [Learn more](/katalon-analytics/docs/kt-build.html)

- The "Task" feature has been removed.

### Improvements

- Introduce a new and improved Katalon TestOps User Interface.

See [What's new in March Release?](/katalon-analytics/docs/new-core-11.html)

## January 19

### New features

- Monitor Test Runs in a calendar view. [Learn more](https://docs.katalon.com/katalon-analytics/docs/create-plan.html#view-test-runs)

- Manage Test Runs with similar configurations with Test Run Types. [Learn more](https://docs.katalon.com/katalon-analytics/docs/create-plan.html#schedule-test-runs)

- View Release Readiness by Test Case status & Test Run history. [Learn more](https://docs.katalon.com/katalon-analytics/docs/kt-jira-release.html)

- Manage **Katalon Studio** Test Results (BDD and non-BDD). [Learn more](https://docs.katalon.com/katalon-analytics/docs/bdd-test-results.html)

- Automatically detect assertions in each Test Case for better quality evaluation & failure investigation. [Learn more](https://docs.katalon.com/katalon-analytics/docs/assertions.html)

- Balance loads between multiple Test Environments. [Learn more](https://docs.katalon.com/katalon-analytics/docs/load-balancing-agents.html)

- Support reports for Visual Testing. [Learn more](https://forum.katalon.com/t/visual-testing-image-comparison-with-katalon-studio-7-8-0-and-katalon-testops/45557)

- Create an Agent for Docker Environment. [Learn more](https://docs.katalon.com/katalon-analytics/docs/agents.html)

- Create a Kubernetes Environment. [Learn more](https://docs.katalon.com/katalon-analytics/docs/aws-eks.html)

- View reports of Web Services & Test Objects.

- View abnormal Web Services for faster failure detection. [Learn more](https://docs.katalon.com/katalon-analytics/docs/view-abnormal-web-services.html)

- View Requirement coverage heat map. [Learn more](https://docs.katalon.com/katalon-analytics/docs/requirement-coverage.html)

- Detect the flakiness of Test Cases. [Learn more](https://docs.katalon.com/katalon-analytics/docs/view-test-cases.html#active-test-cases)

### Improvements

- Simplify the Local Test Environment setup process.

- Enhance CI integrations.

- Enhance UI/UX

- Simplify the Local Test Environment setup process.

- Enhance navigation to recent projects and on-going Test Runs.

- Enhance Jira issue lists.

- Centralize Test Run data for better collaboration.

- [Visual Testing] Incorporate reports into Test Run results.

- [Visual Testing] Provide execution comparisons with visualization.

- View Test Sessions with logs submitted from Test Environments.

- Support sharing Test Run report via email.

- Provide shortcuts to access reports.

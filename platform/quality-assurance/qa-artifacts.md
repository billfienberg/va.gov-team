# Quality Assurance Artifacts

A list of expected deliverables and explanation of their contents is listed below. Please note that you will need access to [TestRail](https://dsvavsp.testrail.io/) in order to create these artifacts.

## Table of Contents

* [Quality Assurance Artifacts](qa-artifacts.md#quality-assurance-artifacts)
  * [Table of Contents](qa-artifacts.md#table-of-contents)
  * [Artifacts](qa-artifacts.md#artifacts)
    * [Regression Test Plan](qa-artifacts.md#regression-test-plan)
    * [Test Plan](qa-artifacts.md#test-plan)
    * [Test Cases](qa-artifacts.md#test-cases)
    * [Test Results](qa-artifacts.md#test-results)
    * [Reference Test Coverage Report](qa-artifacts.md#reference-test-coverage-report)
    * [Summary\(Defects\) Report](qa-artifacts.md#summarydefects-report)

## Artifacts

### Regression Test Plan

**Collab Cycle:**

* \(Draft\) delivered for [Usability Testing Prep](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#usability-testing-prep)
* \(Final\) delivered for [Staging Review](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#staging-review)

**Note: If you already have a regression test plan for your product's baseline in TestRail you can forego this step. However, as your changes are integrated you will need to continue to update your regression test plan to reflect the new baseline.**

Regression test plans should represent a basic suite of test scenarios that cover the baseline functionality of your product prior to changes from your current development effort.

* Example: [Regression Test Plan](https://dsvavsp.testrail.io/index.php?/suites/view/20&group_by=cases:title&group_order=asc)

### Test Plan

**Collab Cycle:**

* \(Draft\) delivered for [Usability Testing Prep](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#usability-testing-prep)
* \(Final\) delivered for [Staging Review](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#staging-review)

You will create a test plan within [TestRail](https://dsvavsp.testrail.io/). The test plan is a mapping of the functional changes being developed to test cases that verify those changes behave as expected per the user stories and acceptance criteria. A test plan may employ multiple testing techniques \(manual, automated end-to-end, and load tests\). If test cases do not exist for each change then they will need to be created.

* Example: [Test Plan](https://dsvavsp.testrail.io/index.php?/plans/view/30)

### Test Cases

**Collab Cycle:**

* \(Draft\) delivered for [Usability Testing Prep](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#usability-testing-prep)
* \(Final\) delivered for [Staging Review](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#staging-review)

Test cases describe in detail the actions taken within the product that verify the changes made during development achieve the acceptance criteria defined in their associated user stories. A link to your [TestRail](https://dsvavsp.testrail.io/) test cases or an export of your test cases including their steps.

* Example: [Test Cases](https://dsvavsp.testrail.io/index.php?/suites/view/2&group_by=cases:section_id&group_order=asc)

### Test Results

**Collab Cycle:** Delivered for [Staging Review](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#staging-review)

Test results include the outcome of the execution of the test cases. These results enable project participants to understand where successes and failures were achieved. A link to your [TestRail](https://dsvavsp.testrail.io/) test results or an export of your test execution logs.

* Example: [Test Results](https://dsvavsp.testrail.io/index.php?/runs/view/7&group_by=cases:section_id&group_order=asc)

### Reference Test Coverage Report

**Collab Cycle:** Delivered for [Staging Review](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#staging-review)

This report provides an overview of which user stories are covered by your test plan as well as what percentage of your test cases are linked to a user story. A link to your [TestRail](https://dsvavsp.testrail.io/) _Coverage for References_ report or an export of your coverage map.

* Example: [Coverage for References Report](https://dsvavsp.testrail.io/index.php?/reports/view/12)

### Summary\(Defects\) Report

**Collab Cycle:** Delivered for [Staging Review](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/vsp-collaboration-cycle/vsp-collaboration-cycle.md#staging-review)

This report provides a summary of the defects uncovered during test case execution as well as a percentage of defects that were resolved vs. unresolved. A link to your [TestRail](https://dsvavsp.testrail.io/) _Summary\(Defects\)_ report or an export of your issues discovered.

* Example: [Summary\(Defects\)](https://dsvavsp.testrail.io/index.php?/reports/view/14)


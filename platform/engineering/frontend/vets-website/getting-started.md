# Getting Started

To build a service on the Veteran-facing Services Platform, which can be anything from a digital form to a map-based facility locator, developers will create a Frontend experience in React on Vets-Website, and connect it to an Integration on Vets-API, which manages the data flow to and from VA systems.

* [Get started](getting-started.md#get-started)
* [Development](getting-started.md#development)
* [Get help](getting-started.md#get-help)

## Get started

1. Confirm that your team's Project Manager has added your name, email address, and Github username to the team spreadsheet and sent it to DSVA. You'll know when you can visit [this Github repo and see the content](https://github.com/department-of-veterans-affairs/va.gov-team).
2. Follow the steps to [create new SSH keys, configure, and test the SOCKS proxy](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/engineering/internal-tools.md#additional-onboarding-steps-for-developers).
3. Verify that you have
   * Have access to the [Veteran-facing Services Platform code repositories](getting-started.md#code-repositories)
   * Have credentials for the shared testing environments — [dev.va.gov](https://dev.va.gov) and [staging.va.gov](https://staging.va.gov).
   * Have access to [Internal Tools](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/engineering/internal-tools.md)
   * **Tip**: If you have a problem or can't get access, post in the _\#vfs-platform-support_ Slack channel or reach out to your DSVA contact.
4. Review all the content this folder — `DeveloperDocs`
5. Review the frontend documentation for [Vets-Website](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/platform/engineering/frontend/vets-website/vets-website/README.md).
6. Review the backend documentation for [Vets-API](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/platform/engineering/frontend/vets-website/vets-api/README.md).

## Development

### Code repositories

The Veteran-facing Services Platform is broken into three parts:

1. [Vets-Website](https://github.com/department-of-veterans-affairs/vets-website), which contains frontend applications and components users interact with
2. [Vets-API](https://github.com/department-of-veterans-affairs/vets-api), a JSON-based API used by the frontend to provide data to and from VA systems
3. [Vets-JSON-Schema](https://github.com/department-of-veterans-affairs/vets-json-schema), which contains shared resources used to structure and validate form data between Vets-Website and Vets-API.

### Local development environment setup

1. [How to setup your front end VA.gov local environment](https://department-of-veterans-affairs.github.io/veteran-facing-services-tools/getting-started)
2. [How to setup your back end VA.gov local environment](https://github.com/department-of-veterans-affairs/vets-api)
3. After you are setup and running both front-end and back-end servers, try logging in using a mock user. Information on how to login with a mock user can be found [here](https://github.com/department-of-veterans-affairs/va.gov-team-sensitive/blob/master/Administrative/accessing-staging.md).
4. [Mock test users](https://github.com/department-of-veterans-affairs/vets-api-mockdata/blob/master/mock_data_table.md)
5. Once you can seccessfully login you should be setup for developing on VA.gov.

### Internal Tools

To get access to metrics, build logs, deployment information and exception details, see [Internal Tools Access](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/platform/engineering/frontend/vets-website/internal-tools-access.md) documentation.

## Get help

DSVA engineering resources are available to provide guidance and support through the development effort.

If you encounter issues or have any questions, raise them in the _\#vfs-platform-support_ Slack channel, or reach out to your DSVA contact.

Next: [Environments](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/platform/engineering/frontend/vets-website/environments.md)

Back: [Developer Docs Introduction](./)


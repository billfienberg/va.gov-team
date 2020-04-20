# Release Phase

The release phase is a time to get your product fully tested and cleaned up in production and eventually launched to a live audience. This will likely include testing and monitoring it in production, making sure contact centers are ready to support it, preparing any marketing or publicity, and actually getting it live for real users -- all with a plan for how to track performance to inform future iterations.

**Below are ideas for things the team can do together to facilitate a solid Product Release. This is a guide, NOT a prescription. Work with your team to identify what your Release plan should look like, what methods and deliverables it should include, in order to get your product live.**

## Epic Issue Title

Release - \[product name - feature or initiative name if applicable\]

_Sample: Release - Login - SSO for other VA properties_

## Epic Issue Attributes

* convert to ZenHub Epic
* add labels:
  * team name
  * product name \(if known\)
* assign to PM, DSVA Team Lead, and DevOps lead
* add to Program Increment

## Epic Issue Description

### Problem Statement

_Copy problem statement_

### Product Outline

_Paste link to the product outline here_

### Acceptance Criteria

* [ ] Necessary ATO updates complete
* [ ] Security review with DevOps complete
* [ ] Production User Acceptance Testing complete
* [ ] 508 Office review complete
* [ ] All launch-blocking bugs fixed
* [ ] Contact Center preparations complete
* [ ] Web Communications strategy in place
* [ ] Go / No Go meeting complete
* [ ] Soft launch successful \(per defined soft launch criteria\)
* [ ] Supporting static content live
* [ ] Global site menus and other navigation elements live
* [ ] Launch announcement sent to stakeholders
* [ ] Hard launch successful, and monitoring works!
* [ ] Hardening epic present to capture ideas for future iteration

### Resources

* [Contact center product guide example](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/README.md)
* [Launch announcement example](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/README.md)
* [UAT sample how to](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/README.md)

### Suggested issues for consideration

**Product tasks**

* Determine UAT approach
* Recruit for UAT
* Conduct UAT
* Schedule 508 Office review
* Create Contact Center guide \(including screenshots of all possible error states\)
* Create product demo video
* Meet with Contact Center to go over the guide
* Meet with Web Comms lead to plan strategy
* Set up analytics dashboard to track product success
* Schedule go/no-go
* Check that analytics and monitoring are working as intended

**Engineering tasks**

* Fix bug 1
* Fix bug 2 \(etc\)
* Remove supporting static content pages from the ignore list
* Remove the production:false flag
* Remove password from production application
* Set up monitoring and logging:
* Configure any alerts around saturation, error rate, latency, availability


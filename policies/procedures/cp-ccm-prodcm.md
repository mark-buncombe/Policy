### Production Deploy / Code Promotion Processes

In order to promote changes into Production, a valid and approved Change Request
(CR) is required. It can be created in the [Change Management System/Portal][1]
which implements the Buncombe County Change Management workflow, using the
Production Change Management (PRODCM) github project to manage
changes and approvals.

[1]: https://buncombecounty.cherwellondemand.com/CherwellPortal

* At least two approvals are required for each PRODCM ticket.  By default, the
  approvers are

    - Security Lead and
    - Engineering Lead.

* Additional approver(s) may be added depending on the impacted component(s).
  For example,

    - the IT Manager is added as an approver for IT/network changes; and
    - the DevOps Lead is added as an approver for changes to `aws-Buncombe County-infra`
      account in AWS.

* Each PRODCM ticket requires the following information at a minimum:

    - Summary of the change
    - Component(s) impacted
    - Justification
    - Rollback plan

* Additional details are required for a code deploy, including:

    - Build job name
    - Build ID and/or number
    - Deploy action (e.g. plan, apply)
    - Deploy branch (e.g. master)
    - Target environment (e.g. `aws-Buncombe County-infra`, `aws-Buncombe County-prod-us`, `datacenter-hq`)
    - Links to pull requests and/or github issues
    - Security scan status and results
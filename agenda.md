## GitHub Working Group Meeting Agendas & Notes
Meeting notes inline in italics (starting with 2021-08-18 meeting)

### 2022-06-22

### 2022-06-08
- No meeting

### 2022-05-25
- No new GitHub topics today
- Jason and Dave gave some updates on UCB OpenShift work and roadmap
  - Looking at cluster redundancy across data centers
  - Initially using VMware and IPI, eventually hope to move to bare metal
  - VMware licensing very expensive and prohibitive to running OpenShift long-term
  - Some current challenges and improvements include:
    - backups including volumes using OADP operator
    - etcd performance alerts
    - customer workload requests and worker node resources
    - cost model using Red Hat operator
  - We see future container use expanding in production and for critical services

- Consider re-branding this group as more of a C3 DevOps/Automation/Containerization working group?
  - Would be good to check in with Orrie about this eventually

- UCCS updates from Ryan and Eric
  - Continuing to explore OpenShift
  - Using OpenShift install in AWS for now while academic licensing is still in the works
  - Have done some proof-of-concept work bringing up one or two existing "hosted" web applications in OpenShift
  - Experience has been very positive thus far
  - Trying to get ROSA trial going but running into some hurdles

### 2022-05-11
- Welcome new UCCS staff members Xiang Tan and Jonathan Douglas
- Chris Wilhelmsen
  - Lots of GitHub activity at CU Anschutz (Informatics, Health AI)
  - Suggested using organization "friendly name" conventions to designate which campuses own which orgs
  - Some discussion of billing that is tied to orgs and may occur monthly - all billing rolls up to the enterprise
  - If campuses beyond UCB start using per-org billed features we may need to navigate that with Todd Schaefer
- Ad hoc platform / devops discussion
  - Chris Wilhemsem
    - CU Denver / Anschutz looking at k8s in Oracle cloud; interest in Prometheus and Grafana
    - Chris W. also noted some contractor work taking place in Google Cloud and using GitHub for code and automation
  - Ryan LaRoy
    - VPN work
  - Eric Schneider
    - New UCCS staff
    - Ansible Tower licensed and in use
    - Continuing to work on OpenShift and Academic Licensing

### 2022-04-27
- No meeting today
### 2022-04-13
- Office Hours / Walk-on Topics

### 2022-03-30
- GitHub outage on 3/17 and [GitHub Status page](https://www.githubstatus.com/) awareness

### 2022-03-16
- Office Hours / Walk-on Topics

### 2022-03-02
- Office Hours / Walk-on Topics

### 2022-02-17
- Initial meeting of working group for 2022
- Office Hours / Walk-on Topics
  - _Billing_
    - _After billing the campuses in September for the initial 6 months of our GitHub Enterprise license, we won't be charged again until September 2022_
    - _There may be some desire to pull billing numbers in April (ahead of the fiscal year end) to allow campuses to include projected GitHub spending in the budget planning process_
    - _Still TBD based on discussion between Todd and UCB OIT Budget and Finance_
   - _Adoption across campuses_
     - _UIS still using GitLab_
     - _Todd to check in with them about potentially transitioning to GitHub_
     - _UIS has invested significant time and effort into GitLab and transition may be tricky_
   - _Miscellaneous discussion about security scanning, image registries, and build/deploy processes_
     - _In light of recent security issues like log4j, questions came up about taking advantage of security features in GitHub_
     - _Dependabot is currently being used by some teams_
     - _GitHub CodeQL was mentioned as another potential tool_
     - _GitHub Packages was also noted as a potential container image registry and supports other uses, as well_
     - _GitHub Packages may also introduce some opportunities for vulnerability scanning, dependency scanning, etc._
     - _UCB and perhaps others would benefit from formal guidance in terms of various CI/CD tools, including security and vulnerability measures_
       - _Possible some of this work will be undertaken by UCB Architecture Review Board_

### 2022 Meetings started again on 2/17

### 2021-12-22
- No meeting due to holidays

### 2021-12-08
- Quick GitHub LFS (Large File Storage) update
  - _UCB purchased "Data Packs" to alleviate default low quotas and avoid the need to "police" usage_
  - _UCB is currently the only org where repositories are using LFS_
- Office Hours

### 2021-11-24
- No meeting due to Thanksgiving week and holiday

### 2021-11-10
- Note about GitHub LFS (Large File Storage) quota
  - _Boulder looking at buying additional data packs for the enterprise_
- Office hours

### 2021-10-27
- GitHub Organization Moves
  - It's possible to move other existing organizations among CU
    departments into our GitHub enterprise account.
  - This is a "wholesale" move and retains permissions, history, etc.
  - UCB working with PhET (see [phet.colorado.edu](https://phet.colorado.edu))
    on moving their existing organization (with a GitHub "gold"
    contract) into our enterprise, which will let them access project
    features not currently available to them.
  - Some coordination needed for transition to SSO and making SSO a
    requirement.
  - GitHub will assist with actually moving the organization (this
    doesn't appear to be something we can do on our own).
- LFS Quota Issues
  - UCB noticed that our small 1Gb LFS quota is sitting at 96% used due
    to one UCB repository.
  - Need more visibility going forward (dashboard or scheduled
    reporting).
  - For now will need to reach out to the department to see if they can
    reduce the repo footprint and remove from commit history.
- Office Hours
  - _Billing Update from Todd_
    - _Todd received speedtypes from all campuses_
    - _This invoice was for the initial six month period between April
      and September and consisted of half of our annual license cost._
    - _UCB just paid the next full year of our license as of September
      20_
    - _Discussed next billing out to the campuses - looking at July 2022
      so campuses can make budget requests for the next fiscal year._
    - _Billing may evolve over time beyond our initial, simple "snapshot"
      usage model._
  - _UIS and GitHub / GitLab_
    - _UIS is still using an expensive GitLab license_
    - _Todd to check in with UIS about potential migration to GitHub_
    - _Still potential benefits to be had here with collaboration among
      UIS and campus development teams._

### 2021-10-13
- Repository Transfers
  - Keep in mind that owners of the "destination" organization receive
    an automated email notification from GitHub when a repository is
    transferred into an org.
  - No automated notifications are sent to the GitHub user initiating
    the transfer or the owners of the "originating" repository or
    organization.
  - UCB submitted a support case to GitHub about this and it was added
    as a feature request.
- Office hours

### 2021-09-29
- Billing updates
  - Actual billing for April - September expected soon (Todd Schaefer)
  - Kludge to get current data displayed locally via Matt Roush's dashboard Node.js app
  - Any time or interest among the group in contributing?
- Office Hours
  - _Not GitHub related, but some misc discussion of new developments with OpenShift education/research licensing._

### 2021-09-15
- Note about repository sizes, quotas, and GitHub large file storage (LFS) and billing implications.
  - _Documentation has been updated at https://university-of-colorado.github.io/_
  - _FAQ now has a section related to this._
- Office Hours

### 2021-09-01
- Reminder about Dave facilitating for any new attendees.
- Billing updates
  - _Matt gave a demo of his initial billing dashboard work._
  - _Matt's last day with CU is September 10._
  - _Billing dashboard code to be committed to GiitHub as part of Matt's transition._
  - _Goal is to bill all the campuses for the ,April - September period at the end of September_
  - _UCB to "own" billing functionality?_
  - _Chris Rose will be joining for now with Matt leaving_
- Office Hours

### 2021-08-18
- Transition to Dave as MC of these meetings, or does someone else wish to step up?
  - _Dave will facilitate from here._
- Billing program updates?
  - _Matt Roush wasn't in attendance today, so no updates._
  - _Expectation is that we'll have initial / basic billing processes in place by the end of August._
- Reduce the cadence of these meetings
  - _Sticking with every two weeks for now and we'll adjust as needed._
- Office Hours
  - _GitHub Projects, Project Boards, and Issues features_
    - _Chris Edmundson inquired about these capabilities as a possible alternate to Jira, for example._
    - _GitHub Projects offers Kanban type functionality._
    - _Boulder currently runs Jira Server but the future is a little uncertain with licensing and Jira Server, Jira Cloud, etc._
    - _More conversations about workflow and CI/CD tools are expected at the CU system (or "enterprise") level._
    - _Chris Wilhemsen has a lot of experience with Jira and other Atlassian tools and would love to be involved in any conversations in this area._
  - _New Opportunities / Changes_
    - _Erinn will be retiring from IT and leaving the University in mid-September._
    - _Chris Edmundson will be taking on a new IT Security role within UCD OIT in late August._

### 2021-08-04
- When can we expect the billing program to be available?
- Self service with Azure AD + SCIM, the good and the bad.
- Office hours

### 2021-07-21
- Office hours

### 2021-07-07
- Reduce meeting cadence
- Final moves (probably) for auth in Boulder's GitHub.
- Understanding Internal Repositories
- Office hours

### 2021-06-30
- On the ups and downs of Azure AD Team Sync (https://docs.github.com/en/organizations/managing-saml-single-sign-on-for-your-organization/managing-team-synchronization-for-your-organization)
- Office hours

### 2021-06-16
- Office hours (open forum for questions/concerns)

### 2021-06-07
- Status Updates
- Any work with billing?
- Questions?

#### Azure AD Self Service:
References for Azure AD self service:
- https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/github-tutorial
- https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/access-panel-manage-self-service-access

### 2021-05-24
- Enterprise admins? Anyone?
- Status Updates
- Questions?

### 2021-05-17
#### Is CU Boulder trying to control GitHub?
There seems to be some feelings floating around that CU Boulder is trying to arbitrarily control GitHub for other campuses/entities. This appears to be mostly based around miscommunication of why we are where we are. Time will be taken to explain the decisions about GitHub that have been made so far.

#### Arbitrary Organizations within the enterprise
As a first pass attempt, an organization per campus was set up, the hope was that campuses could use teams within organizations to effectively manage themselves.  With this structure tracking billing for campuses was simple, each campus only had one organization and the number of users per campus was the number of users in the organization. However, it is becoming increasingly clear that campuses want the ability to create an arbitrary number of organizations. Further there are a number of restrictions in GitHub around teams that make this a bit unpalatable. 
There are unfortunately a number of drawbacks to arbitrary organizaions in the enterprise and these mainly center around billing. This again is a continuation of the duscussion that occured on May 3rd, I will include the notes sent out for that meeting invite:

Do we need more organizations?

Organizations are a flat namespace. So, if two users wish to create repository 'foo' a conflict will ensue, and the second-place person will need to rename. This is not a particularly big deal (to me), but with our current design I expect hundreds if not thousands of repositories in at least, the Boulder organization. Do we need to have more organizations? Do we care if the CS department has a bunch of students doing projects in the same organization as OIT? If so, this would imply that we will need to have more campuses have enterprise admins in order to create organizations. It probably also implies using a centralized IDP because setting up SAML per organization right now appears to be a slightly heavyweight operation. 

As well, the billing model for GitHub as it currently stands (this is my understanding, billing is not my area) is weighted on the number of users a campus has. If we allow unlimited organizations to be created, tracking those users and campuses would become difficult if not impossible. This may imply that we move to an equal apportionment billing model. Each campus pays an equal amount for GitHub, and can create unlimited organizations, and can have unlimited users, etc. etc. 

#### Enterprise admins from each campus
This discussion happened in the last meeting we pulled together on May 3, but it will continue, I'll simply copy and paste my notes from the last meeting invite:

Should every campus have an enterprise owner or two or three?

This question came up, and I guess there was an expectation set in the past that each campus has a couple of folks who are enterprise admins? I don't personally remember that, but it could have certainly been the case. As GitHub is currently configured there are basically only two things an enterprise owner can do that an organization owner cannot, create more organizations, and have slightly (strong emphasis on slightly) better insight into which organizations are using resources like action minutes. That is all. As an organization owner, you have insight into how many action minutes your organization is consuming (amongst other metered resources) but you cannot see what other organizations are consuming, and as mentioned, you can't create other organizations. Is this a sufficient level of access? Does each campus feel they need to have that higher level of access into the enterprise?

#### The enterperise managed users beta
Some folks have felt that the way SSO is handled in GitHub is less than optimal. It appears GitHub is working to address that: https://github.com/github/roadmap/issues/132 we have asked to join the private beta and are on the wait list. 

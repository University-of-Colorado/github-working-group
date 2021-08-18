## GitHub Working Group Meeting Agendas & Notes
Meeting notes inline in italics (starting with 2021-08-18 meeting)

### 2021-09-01

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

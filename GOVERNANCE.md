# k0s Governance

This document defines governance policies for the [k0s and its sub-projects](https://github.com/k0sproject):

- [k0s Governance](#k0s-governance)
  - [Principles](#principles)
  - [Code of Conduct](#code-of-conduct)
  - [Vendor Neutrality](#vendor-neutrality)
  - [Meetings](#meetings)
  - [Project Roles \& Contributor ladder](#project-roles--contributor-ladder)
    - [Summary of Roles](#summary-of-roles)
      - [Contributors](#contributors)
        - [Checklist before becoming a Contributor](#checklist-before-becoming-a-contributor)
        - [Privileges of a Contributor](#privileges-of-a-contributor)
      - [Reviewers](#reviewers)
        - [Checklist before becoming a Reviewer](#checklist-before-becoming-a-reviewer)
        - [Privileges of a Reviewer](#privileges-of-a-reviewer)
      - [Maintainers](#maintainers)
      - [Mapping Project Roles to GitHub Roles](#mapping-project-roles-to-github-roles)
    - [Off-boarding Guidance](#off-boarding-guidance)
  - [Maintainer Areas](#maintainer-areas)
    - [k0s Projects](#k0s-projects)
  - [Conflict Resolutions](#conflict-resolutions)
  - [Changes](#changes)
  - [Credits](#credits)

## Principles

The k0s community adheres to the following principles:

- **Open**: The k0s community strives to be open, accessible and welcoming to everyone. Anyone may contribute, and contributions are available to all users according to open-source values and licenses.
- **Transparent and accessible**: Any changes to the k0s source code and collaborations on the project are publicly accessible (GitHub issues, PRs, and discussions).
- **Merit**: Ideas and contributions are accepted according to their technical merit and alignment with project objectives, scope, and design principles.

## Code of Conduct

k0s follows the [Code of Conduct](CODE_OF_CONDUCT.md).

## Vendor Neutrality

k0s follows the CNCF vendor neutrality guidelines documented at:

   https://contribute.cncf.io/maintainers/community/vendor-neutrality/

## Meetings

The k0s Project community meetings are scheduled via [LFX Calendar](https://zoom-lfx.platform.linuxfoundation.org/meetings/k0s?view=month). Meeting notes are kept in CNCF [notes](https://notes.cncf.io/s/_5FVgysYK) tool. Both of these require a Linux Foundation account to access.

The maintainers may also have closed meetings to discuss security reports or Code of Conduct violations. Such meetings should be scheduled by any maintainer on receipt of a security issue or CoC report. All current Maintainers must be invited to such closed meetings, except for any maintainer who is accused of a CoC violation.

## Project Roles & Contributor ladder

The k0s community welcomes all contributors and has well-defined roles detailed below. The progression between the roles defines the contributor ladder. The contributor ladder is a way to provide a path for contributors to grow and take on more responsibilities in the project. Community members generally start at the first levels of the ladder and advance up it as their involvement in the project grows.

This document highlights the roles and responsibilities for the k0s community members. It also outlines the requirements for anyone who is looking to take on leadership roles in the k0s project. The following governance applies to all k0s subprojects.

Each of the contributor roles below is organized into three types of lists:

Responsibilities: tasks that a contributor is expected to do at this level
Qualifications: requirements a person needs to meet to be at that level
Privileges: rights contributors on that level are entitled to

As the k0s project grows, the current roles may be broken out into new roles and/or teams and roles may no longer be needed.

All roles within the k0s project will need to adhere to CNCF [Code of Conduct](https://github.com/cncf/foundation/blob/master/code-of-conduct.md).

### Summary of Roles

The table below summarizes project roles and responsibilities. Details are provided in the sections following the table:

| Role         | Requirements                                                                                                                | Ongoing Responsibilities                                               | Defined by                                                                                                      |
|--------------|-----------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|
| Contributors | At least five (5) contributions to any sub-project.                                                                         | None                                                                   | CONTRIBUTORS.md, voted in by current maintainers of the given sub-project                                       |
| Reviewers    | An established contributor who regularly participates in the project via issues, PRs and discussions.                       | Review PRs and provide feedback to contributors.                       | Voted in by the k0s maintainers, listing in `MAINTAINERS.md`, GitHub organization member.                       |
| Maintainer   | At least ten (10) contributions to a sub-project + Highly experienced and active contributor + Voted in by k0s maintainers. | Monitor project growth, set direction and priorities for a subproject. | Voted in by the k0s maintainers, listing in `MAINTAINERS.md`, GitHub organization member, and repository owner. |

#### Contributors

Contributors are individuals who have made at least five (5) contributions to the project; by authoring PRs, commenting on issues and pull requests,
and participating in community discussions on Slack or the mailing list.
They are trusted to have their contributions to run CI without requiring maintainers' approval.

##### Checklist before becoming a Contributor

- Have at least five (5) PRs successfully merged for any repositories under the k0s organization in 6 month period
  - The five PRs must demonstrate good judgment and a meaningful understanding of the project’s codebase, design, and development practices. The number of PRs alone is not sufficient to meet this requirement
- Member of the k0s channel(s) on Kubernetes and/or CNCF Slack
- Attended one (1) Contributors Meeting as documented
- Check-in with maintainers to make yourself eligible to be voted in as a Contributor by the maintainers

##### Privileges of a Contributor

- Listed in the file in at least one (1) organization repository
- k0s contributor badge issued
- Their PRs will run CI without the maintainers approval

To join the k0s project as a Contributor create a Pull Request (PR) in the [k0s repository](https://github.com/k0sproject/k0s) with the following:

1. Changes to add yourself to the [CONTRIBUTORS.md](https://github.com/k0sproject/k0s/blob/main/CONTRIBUTORS.md) file.
2. Links to your prior contributions (at least five).
3. Links to slack discussions, issue comments, etc.

#### Reviewers

A Reviewer is an established contributor who regularly participates in the project via issues, PRs and discussions.
Reviewers are expected to review PRs, provide feedback to contributors, and help maintain the quality of the project.
Reviewers have privileges in the project repositories to give authoritative reviews and as such are trusted to act in the interests of the whole project.

##### Checklist before becoming a Reviewer

- Be an established contributor in repositories under the k0s organization
- Regularly participates in issues, pull requests, and community discussions
- Demonstrates high-quality and timely PR reviews with constructive feedback
- Attained a majority vote from current maintainers
- Added to `MAINTAINERS.md` as a Reviewer
- Granted GitHub organization membership with repository permissions appropriate for PR review

##### Privileges of a Reviewer

Reviewers have the privileges of a contributor, and in addition:

- Has the ability to review pull requests and provide feedback
- Provides feedback to contributors
- Helps maintain the quality of the project
- Reviewer approvals are considered authoritative and count toward required pull request approvals
  - Reviewer can give authoritative review for a maintainers PRs and their approvals are considered binding for the purpose of merging
  - A maintainer can override a reviewer's approval if necessary

#### Maintainers

Maintainers are individuals who have shown good technical judgement in feature design/development in the past. Maintainers have overall knowledge of the project and features in the project. They can read, clone, and push to the repository. They can also manage issues, pull requests, and some repository settings.

Maintainers are the technical authority for a subproject and are considered leaders for the organization as a whole. They must have demonstrated both good judgement and responsibility towards the health of the subproject. Maintainers must set technical direction and make or approve design decisions for their subproject, either directly or through delegation of these responsibilities. Unlike contributors, maintainers have the highest degree of responsibility and ownership for the project. Maintainer status may be subject to a vote and, if the minimum level of activity is not maintained, may be moved to an _emeritus_ status.

**Checklist before becoming a Maintainer:**

- Have at least ten (10) significant PRs successfully merged for any combination of repositories under the k0s organization
- Member of the `#k0s-users` and `#k0s-dev` channels on Kubernetes Slack workspace
- Regularly attends k0s [Maintainers and Community Meetings](https://docs.google.com/document/d/1K7kc4nARFsM60RpzWF7xREF9FHySDuWSu9_6dstkLlg/edit?tab=t.0#heading=h.s485wlw1do6e)
- Create a pull request to add self to `CODEOWNERS` file in at least one (1) repository
- Attained the super majority vote (66%) from maintainers
- Respond to reviews from maintainers on pull requests
- Proficient in GitHub, YAML, Markdown, and Git
- Exhibits strong attention to detail when reviewing commits and provides generous guidance and feedback
- Helps others achieve their goals with open-source and community contributions
- Understands the workflow of the Issues and Pull Requests
- Makes consistent contributions to the k0s project
- Consistently initiates and participates in [k0s discussions](https://slack.k8s.io/#k0s)
- Has knowledge and interest that aligns with the overall project goals, specifications, and design principles of the k0s project
- Makes contributions that are considered notable
- Demonstrates ability to help troubleshoot and resolve user issues
- Has achieved the k0s Certification or demonstrated an equivalent mastery of k0s
- Maintains a consistent level of activity with contributions to the project

**Responsibilities of a Maintainer**

- Tracks and ensures adequate health of the modules and subprojects they are in charge of
- Ensures adequate test coverage to confidently release new features and fixes
- Ensures that tests are passing reliably (i.e. not flaky) and are fixed when they fail
- Mentors and guides code owners, reviewers, and contributors
- Actively participates in the processes for discussion and decision making in the project
- Merges Pull Requests and helps prepare releases
- Makes and approves technical design decisions for the subproject
- Helps define milestones and releases
- Decides on when PRs are merged to control the release scope
- Works with other maintainers to maintain the project's overall health and success holistically

**Privileges of a Maintainer**

- Listed as an organization member
- Listed in `CODEOWNERS` in at least one (1) repository
- Member of the https://lists.cncf.io/g/cncf-k0s-maintainers mailing list
- Have issues assigned to them
- Have PRs assigned to them
- Receives a k0s Maintainer Badge
- Listed in `MAINTAINERS.md`

**On-boarding Criteria**

- Voted in by a majority of current maintainers, raised in a PR by the proposed member to add themselves to `MAINTAINERS.md`, during a voting period lasting at least three (3) working days

**Off-boarding Criteria**

An off-boarding vote may be called by any maintainer if any of the following criteria are met:

- A maintainer or contributor has become in-active, meaning they have not contributed or participated in project activities for an extended period.
  - Contributions will be tracked manually until having an active Devstats Dashboard for the project.
  - Other relevant data will be collected and evaluated to assess the maintainer's contributions. This includes their involvement in discussions, conversations on Slack, and any other relevant interactions.

The off-boarding process includes the following steps:

- The off-boarding process is initiated by any currently active maintainer who conducts a review of the maintainers list and proceeds to initialize the off-boarding process if the above criteria are met.
- The plans of off-boarding process is sent in a private Slack message or email to the candidate.
- If the candidate for removal states plans to continue participating, another 6 months will be granted to the candidate to make contributions and the new cycle starts. No action is taken and this process terminates.
- If the candidate fails to meet the criteria during the second attempt to make contributions, the off-boarding process continues.
- A pull request (PR) proposing movement of the candidate is sent, initiating the public voting phase.
- The vote passes if a majority of current maintainers vote yes during a voting period lasting five (5) working days.
- A positive vote will result in movement to an _emeritus_ status within `MAINTAINERS.md` and removal from organization membership.

#### Mapping Project Roles to GitHub Roles

The roles used in this document are custom roles mapped according to the [GitHub roles and responsibilities](https://docs.github.com/en/organizations/managing-access-to-your-organizations-repositories/repository-roles-for-an-organization).

| Project Role | GitHub Role                     |
|--------------|---------------------------------|
| Contributor  | Triage                          |
| Reviewer     | Triage + reviewers team mapping |
| Maintainer   | Maintain                        |

### Off-boarding Guidance

If any of the above roles hasn't contributed in any phases (including, but not limited to: code changes, doc updates, issue discussions) in 3 months, the administrator needs to inform the member and remove one's roles and GitHub permissions.

## Maintainer Areas

The k0s projects code base cover many areas and project maintainers are not required to know everything about a project.
For this reason, maintainers can be specific to one (or more) area of the code base, every area representing a specific aspect.

### k0s Projects

- [k0s](https://github.com/k0sproject/k0s)
- [k0smotron](https://github.com/k0sproject/k0smotron)
- [k0sctl](https://github.com/k0sproject/k0sctl)
- [k0sproject rig](https://github.com/k0sproject/rig)
- [k0s Community](https://github.com/k0sproject/community)
- [k0s Website](https://github.com/k0sproject/k0sproject.github.io)

## Conflict Resolutions

Typically, it is assumed that disputes will be resolved amicably by those involved. However, if the situation becomes more serious, conflicts will be resolved through a voting process. A supermajority of votes from project maintainers is required to make a decision, and the project lead has the final say in the ruling.

## Changes

This Project Governance is a living document. All key project changes including changes in project governance can be proposed by a GitHub PR and then reviewed and voted on by project maintainers.

## Credits

Sections of this document have been borrowed from the [CoreDNS](https://github.com/coredns/coredns/blob/master/GOVERNANCE.md) and [fluxcd](https://github.com/fluxcd/community/blob/main/GOVERNANCE.md) projects.

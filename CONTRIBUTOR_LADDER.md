# OpenEverest Contributor Ladder

This document describes the roles in the OpenEverest community, what each role is responsible for, and how people move between them. Roles are held by individuals, not companies. Contributors from any organization are welcome at every level.

| Role | Scope | GitHub permission | How to get there |
| ---- | ----- | ----------------- | ---------------- |
| [Contributor](#contributor) | Any repository | – | Contribute |
| [Reviewer](#reviewer) | One or more repositories | Triage | Nomination, lazy consensus |
| [Component Maintainer](#component-maintainer) | Specific repositories | Maintain on those repositories | Nomination, simple majority of Project Maintainers |
| [Project Maintainer](#project-maintainer) | Whole project | Maintain on all repositories | Nomination, ⅔ vote of Project Maintainers |

## Contributor

Anyone who contributes to the project: code, documentation, reviews, issues, testing, answering questions, talks or blog posts.

**Responsibilities**
- Follow the [Code of Conduct](CODE_OF_CONDUCT.md) and the [contributing guide](https://github.com/openeverest/openeverest/blob/main/CONTRIBUTING.md).
- Sign off commits ([DCO](https://developercertificate.org/)).

## Reviewer

Reviewers are trusted to review pull requests in one or more repositories. Their approval is a signal of quality to maintainers.

**Requirements**
- Several merged, non-trivial contributions to the repositories in scope.
- Has reviewed pull requests in those repositories.
- Familiar with the codebase and project conventions.

**Responsibilities**
- Review pull requests in a timely and constructive way.
- Help triage issues.

**Becoming a Reviewer:** any Component or Project Maintainer nominates the candidate in a public GitHub issue or discussion. The nomination is accepted by [lazy consensus](GOVERNANCE.md#lazy-consensus) of the maintainers of the repositories in scope, with no objections within one week.

## Component Maintainer

Component Maintainers own specific repositories, for example a provider or a plugin. This is the path for people who build and run a specific integration to take responsibility for it.

**Requirements**
- Significant, sustained contributions and reviews in the component, typically as a Reviewer for at least 3 months.
- Demonstrated good judgment on design, quality and compatibility.

**Responsibilities**
- Review and merge pull requests, triage issues, and keep CI healthy in their repositories.
- Release their components following the [release process](https://github.com/openeverest/openeverest/blob/main/RELEASE.md#providers-plugins-and-other-components).
- Respond to security reports affecting their components, together with the security response team.
- Keep compatibility with supported core versions.

**Becoming a Component Maintainer:** a Project Maintainer nominates the candidate in a public GitHub issue or discussion. Project Maintainers approve by **simple majority**. Component Maintainers are listed in [MAINTAINERS.md](MAINTAINERS.md).

## Project Maintainer

Project Maintainers are responsible for the project as a whole. See [GOVERNANCE.md](GOVERNANCE.md#maintainers).

**Requirements**
- Sustained contributions across more than one area of the project, typically as a Component Maintainer or Reviewer for at least 6 months.
- Shown leadership: design reviews, mentoring, community engagement.

**Responsibilities**
- Everything a Component Maintainer does, across the project.
- Project direction, governance, releases and the [security response](https://github.com/openeverest/openeverest/blob/main/SECURITY.md#security-response-team).
- Vote on governance and maintainer decisions.

**Becoming a Project Maintainer:** an existing Project Maintainer nominates the candidate. Project Maintainers approve by a **⅔ majority vote**, as described in [GOVERNANCE.md](GOVERNANCE.md#changes-in-leadership).

## Onboarding

When someone takes on a new role, a Project Maintainer:
1. updates [MAINTAINERS.md](MAINTAINERS.md) and, for Project Maintainers, [`.project/maintainers.yaml`](https://github.com/openeverest/.project/blob/main/maintainers.yaml);
2. grants the matching GitHub permissions and updates `CODEOWNERS`;
3. for Project Maintainers, adds them to the private maintainer channels and the security response team.

## Stepping Down and Emeritus

Anyone may step down from a role at any time by telling the Project Maintainers. Advance notice and help with handing over work are appreciated.

**Inactivity:** a Reviewer or maintainer with no reviews, commits or meeting participation for **6 months** is contacted by the Project Maintainers. If there is no reply, or they don't plan to return, within **30 days**, the Project Maintainers move them to emeritus by **simple majority**.

**Removal:** a person may be removed from a role for other reasons, such as a Code of Conduct violation, by a **⅔ majority vote** of Project Maintainers. The person concerned does not vote.

**Offboarding:** a Project Maintainer revokes the GitHub permissions and private-channel access, and moves the person to the **Emeritus** section of [MAINTAINERS.md](MAINTAINERS.md). Emeritus members are thanked for their work and may return to an active role through the normal nomination process.

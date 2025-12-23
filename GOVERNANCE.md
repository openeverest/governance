# OpenEverest Governance

This document defines governance policies for the OpenEverest project.

## Our Mission

> **"Simplifying database management. Everywhere."**

Managing stateful workloads remains a significant hurdle for many engineering teams, particularly when moving away from managed cloud services. Our vision is simple: enable 
teams to run databases anywhere—on-premise, hybrid, or multi-cloud—without sacrificing usability, security, or reliability.

While Kubernetes Operators exist to solve this, they often demand a steep learning curve and deep familiarity with specific Custom Resources (CRs). 
OpenEverest aims to standardize this experience, abstracting the complexity to provide a unified, user-friendly interface for database management across any infrastructure.

### Project Origins

OpenEverest evolved from **Percona Everest**, a tool originally developed by [Percona](https://percona.com). 
To foster a truly vendor-neutral ecosystem, the project has transitioned into a fully independent open-source initiative. 
OpenEverest is now driven by open governance and supported by a diverse, multi-vendor community.

## Core Values

Building database solutions for Kubernetes requires bridging the gap between the Cloud Native ecosystem and deep database internals. 
OpenEverest aims to lead innovation in the "Data on Kubernetes" space.

We prioritize an extensible architecture, allowing new databases and management tools to be integrated seamlessly via plugins. 
This flexibility drives our goal of becoming the most proficient platform for open-source database management.

We believe that a healthy open-source community is built on teamwork, trust, merit, and accountability. To that end, the OpenEverest project embraces the following values:

* **Technical Excellence:** We strive to provide the premier experience for running data on Kubernetes. 
This demands a commitment to high proficiency in both container orchestration and database technologies.

* **Security and Quality by Design:** We believe in "shifting left." Automated testing and security protocols are integrated directly into our development 
lifecycle to ensure reliability and safety, rather than treating them as afterthoughts or manual checks.

* **Community First:** The sustainability and growth of our ecosystem take precedence over release schedules or the goals of any single sponsoring organization. 
Every contributor participates in the project as an individual peer.

* **Fairness and Meritocracy:** All voices matter. Feedback and code contributions are evaluated strictly on their technical merit and value to the project, 
regardless of the contributor's background or employer.

* **Radical Transparency:** We operate with a "public by default" mindset. Decision-making, roadmaps, and discussions occur in open forums and repositories to ensure discoverability. 
We encourage constructive dissent and respectful debate as essential drivers of innovation.

## Maintainers

Maintainers are the stewards of the OpenEverest ecosystem, playing a pivotal role in the development and strategic direction of the project. 
Being a maintainer is a privilege that comes with significant responsibility; it is a role reserved for individuals who have demonstrated a deep commitment to the project's health and growth.

A Maintainer is more than just a contributor with write access. They are community leaders who have proven their ability to:
* Collaborate effectively with the wider team.
* Facilitate peer reviews by connecting code authors with the right subject matter experts.
* Uphold high standards for code quality and testing.
* Take ownership of issues, ensuring they are resolved thoroughly.

Ultimately, a maintainer acts as a model citizen of the OpenEverest community, dedicated to its long-term success. All current maintainers are listed in the [MAINTAINERS.md](MAINTAINERS.md) file.

### Changes in Leadership

The maintainer group is self-governing. New maintainers must be nominated by an existing maintainer. 
Both appointments and removals are decided by a **two-thirds (⅔) majority vote** of the current maintainers.

If a maintainer steps down or is removed via a vote, they are transitioned to **Emeritus** status to acknowledge their past contributions.

### GitHub Permissions and Administration

In terms of repository management:
* **Maintainers Team:** All active maintainers are added to the `maintainers` team on GitHub. 
This grants them the **Maintain** role across all OpenEverest repositories, allowing them to manage issues, review PRs, and merge code.
* **Admins Team:** Maintainers willing to take on additional administrative burdens (such as repository configuration and secret management) may be appointed to the `admins` team. 
This grants the **Admin** role across the organization.

## Meetings and Communication

### Public Engagement
Maintainers act as the public face of the project. Whenever time zones and schedules permit, Maintainers are expected to attend the public developer meetings 
(see ["OpenEverest Community Meetings" in the organization page](https://github.com/openeverest/#openeverest-community-meetings) for details).

### Closed Sessions
Maintainers also hold closed sessions specifically to address sensitive topics, such as unpatched security vulnerabilities or Code of Conduct (CoC) reports. 
Any Maintainer may call for a private meeting upon receiving such a report. All active Maintainers must be invited to these sessions, 
with the exception of any Maintainer who is the direct subject of a CoC investigation.

## Code of Conduct Enforcement

Protecting the safety of our community is paramount. Violations of the [Code of Conduct](CODE_OF_CONDUCT.md) by general community members will be reviewed and resolved 
via the private Maintainer mailing list.

**Handling Internal Violations**
If a Code of Conduct report is filed against an active Maintainer, a special protocol applies to ensure impartiality. 
The accused Maintainer is recused from the discussion. The remaining leadership will designate two Maintainers to oversee the resolution process, 
working with independent mediators or neutral third parties as necessary to resolve the issue fairly.

## Decision Making

### Lazy Consensus
OpenEverest operates primarily on "lazy consensus." This means that proposals and changes are assumed to be accepted unless an objection is raised within a reasonable timeframe. 
This keeps the project moving fast without unnecessary bureaucracy.

### Voting Protocol
Periodically, formal decisions or "hard" consensus is required. Any Maintainer has the right to demand a formal vote on a specific issue. Voting may occur in the following venues:
* **Public:** A dedicated GitHub Discussion under the "Maintainers" category.
* **Private:** The Maintainers' mailing list (reserved strictly for security or conduct matters).
* **Live:** During scheduled developer meetings.

### Voting Thresholds
* **Standard Actions:** Most operational votes require a **simple majority (>50%)** of all active Maintainers to pass.
* **Governance Changes:** Amendments to this Governance document require a **two-thirds (⅔) supermajority** of all active Maintainers.



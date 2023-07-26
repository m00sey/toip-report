# Analysis of ToIP GitHub Access and organizational recommendations.

The following report is an analysis of current GitHub resources, teams and repositories within the Trust Over IP GitHub organization and recommendations to create, normalize and remove resources.

## Membership

"Trust Over IP Members" (people that have gone through the Steering/General/Contributor sign-up) should be added to the GitHub Organization as "Members".

### Rational
It is nice to be a part of something!
Access to repositories should be managed through WG/TF groups in the structure provided below. 
We should not have any "floating" individuals associated we ownership of repositories.
To use the Team structure below, ToIP members need to be a part of the GitHub organization.

### Whois

@ToIPOperations is this an account we have access to/control over?

#### Concern
It is an Admin on everything.

## GitHub Teams

These recommendations provide either clean-up or consistency in naming and provide an archetype for new Working Groups and Task Forces moving forward.

### Recommendation
Create a GitHub team for each existing Working Group and a child team for the WG Task Forces. Initially using the chairs/co/vice chairs for assigning GitHub `Admin` access.

#### Rational
While not all Working Groups or Task Forces may provide deliverables via GitHub, maintaining a current hierarchy and subsequent Admins of those groups provide a consistent approach to accessing GitHub.

#### Proposal
Create the following Teams hierarchy:

* Governance Stack Working Group (gswg)
    * Governance Architect Task Force (gswg-ga-tf)
    * Attraction Pass Task Force (gswg-ap-tf)
    * Issuer Governance Requirements Task Force (gswg-igr-tf) (needs adding to wiki)
* Technology Stack Working Group (tswg)
    * Trust Registry Task Force (tswg-tr-tf)
    * Authentic Chained Data Containers (tswg-acdc-tf)
    * Technology Architecture Task Force (tswg-ta-tf)
    * Trust Spanning Protocol Task Force (tswg-tsp-tf)
    * AI & Metaverse Technology Task Force (tswg-aimt-tf)
    * Credential Exchange Protocols Task Force (tswg-cep-tf)
    * DID WebS Task Force (tswg-dw-tf) - PENDING VOTE
* Utility Foundry Working Group (ufwg)
* Ecosystem Foundry Working Group (efwg)
    * Internet of Research Ecosystem Task Force (efwg-ire-tf)
    * Human Trafficking Safety Response Ecosystem (efwg-htsre-tf)
    * YOMA Ecosystem Task Force (efwg-yomae-tf)
    * Good Health Pass Working Group (efwg-ghp-tf) (anomly it is named a working group under the task force list)
    * White Paper Task Force (efwg-wp-tf)
    * Solution Pack Task Force (efwg-sp-tf)
    * Learning Pathways Taskforce (efwg-lp-tf)
* Concepts & Terminology Working Group (ctwg)
* Human Experience Working Group (hewg)
* Data Modelling and Representation Working Group (dmrwg)
* Owners (owners) - A fallback for any orphaned repos to ensure continuity of access.


A more formal and known GitHub access strategy may make it easier for groups to contribute their work to ToIP.

### Existing Team clean up
Currently, GitHub naming is sporadic and access unaligned with current WG/TFs.

#### Team - "CTWG-Dev"
7 members

##### Recommendation
* Create `ctwg` team for naming consistency
* Copy members from `CTWG-Dev`
* Apply new team to repos
    * trustoverip/ctwg
    * trustoverip/ctwg-sandbox
    * trustoverip/ctwg-tev2
    * trustoverip/ctwg-toolkit-mrg
    * trustoverip/essiflab (see repo recommendations)
    * trustoverip/toip (see repo recommendations)
    * trustoverip/tt (see repo recommendations)
* Remove `CTWG-Dev` team


#### Team - "Deliverables Recommendations" 
3 members

##### Recommendation
* Remove

##### Repercussion
* trustoverip/deliverables needs new owners

#### Team - "GitHib Organization Task Force"
2 members

##### Recommendation
* Remove

##### Repercussion
* trustoverip/logo-assets needs new owners

#### Team - "HXWG - Maint"
3 members

##### Recommendation
* Create `hxwg` team for naming consistency
* Copy members from `HXWG - Maint`
* Apply new team to repos
    * trustoverip/hxwg
* Remove `HXWG - Maint` team

#### Team - "members"
2 members

##### Recommendation
* Remove

##### Repercussion
 * Add team `tswg-tsp-tf` as the owner of `trustoverip`/trust-spanning-protocol`

## GitHub Repositories

### Renaming
As noted in the [GitHub Blog](https://github.blog/2013-05-16-repository-redirects-are-here/) renaming and keeping existing references unbroken is trivial.

#### Rational
Consistent naming will ease access, maintenance and discoverability.

##### Recommendation
 * trustoverip/essiflab -> trustoverip/ctwg-essiflab 
 * trustoverip/yoma -> trustoverip/ctwg-yoma 
 * trustoverip/tt -> trustoverip/ctwg-term-toolset
 * trustoverip/acdc -> trustoverip/terms-acdc
 * trustoverip/credential-exchange-protocols -> trustoverip/twsg-credential-exchange-protocols-tf
 * trustoverip/trust-spanning-protocol -> trustoverip/twsg-trust-spanning-protocol-tf
 * trustoverip/TechArch -> trustoverip/tswg-technology-architecture-tf
 * trustoverip/toip -> trustoverip/terms-toip
 * trustoverip/ctwg -> trustoverip/terms-ctwg
 * trustoverip/concepts-and-terminology-wg -> trustoverip/ctwg (consistent with tswg)
 * trustoverip/utility-foundry-wg -> trustoverip/ufwg
 * trustoverip/gswg -> trustoverip/terms-gswg

### Archive
Repositories not active, or not under governance of an exist WG/TF.

#### Rational

Keeping a clean and up-to-date set of repositories will make maintenance moving forward manageable.

##### Recommendation
* trustoverip/qr-code-spec
* trustoverip/TSS0033-technology-stack-acdc
* trustoverip/TRTF-trust-decision
* trustoverip/mega
* trustoverip/ghp-paper-creds
* trustoverip/deliverables
* trustoverip/WP0035-decentralized-resource-identifiers
* trustoverip/mkdocs-material
* trustoverip/ghp
* trustoverip/keri
* trustoverip/IG0029-utility-project-guide
* trustoverip/WP0010-toip-foundation-whitepaper
* trustoverip/TIP0028-saturn-v
* trustoverip/TSS0001-governance-stack
* trustoverip/TSS0013-layer3-interop-spec
* trustoverip/TSS0012-layer2-interop-spec
* trustoverip/spec-up
* trustoverip/TSS0011-layer1-Interop-spec
* trustoverip/WP0020-digital-trust-marketplace-faq
* trustoverip/TSS0001-goverance-stack
* trustoverip/TSS0002-technology-stack
* trustoverip/next-deliverable-num
* trustoverip/nymble-ecosystem
* trustoverip/technology-stack-wg
* trustoverip/governance-stack-wg
* trustoverip/SC
* trustoverip/admin
* trustoverip/ecosystem-foundry-wg

###### Nota bene
Reviewing the activity on these repositories, we should decide on archive vs delete.
There is a lot of boilerplate in here.


## 2FA

Configuring 2FA is described [here](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication)

##### Recommendation

Members of the ToIP with the "Owner" role must have 2FA enabled.
2FA should be a prerequisite to adding any member to a team or role with administrative permissions.

## New Team/Repository Archetype
An example of team/repository configuration.

### Scenario

The TSWG wants to add a new Task Force "did:webs". The Task Force is responsible for creating a community specification describing a new, better, more secure DID method.

##### Recommendation

A new child team of `tswg` is created using the prefix of the parent, the `tf` suffix and a shortened name (first character of each word) `tswg-dw-tf`.

The elected chairs/editors of the Task Force are added to the Team in GitHub.

A new repository for the specification is created with the Working Group prefix `tswg-did-webs-specification`.

The `tswg-dw-tf` is added as a collaborator on the repository with the "Maintainer" role.

Any contributions from outside the members of the `tswg-dw-tf` GitHub Team, meaning any collaborator or member of the task force meetings, should be made through a fork/pull request workflow.

##### Rational

This limits the number of people with "administrative" roles within the organization while being inclusive of any contributing member.
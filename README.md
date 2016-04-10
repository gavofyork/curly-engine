# Yellow Paper Committee
#### A blockchain-based organisation to manage the evolution of the Ethereum protocol specification.

## Introduction

The Yellow Paper exists as a formal, non-executable and implementation-neutral specification of the Ethereum protocol. Through being a strict formal specification it has avoided the project needing a specific reference implementation. This then avoided having a favoured development team and repository along with the access permissions that become politically centralisable as has happened in the case of Bitcoin.

The Ethereum protocol was initially the work of a very small number of people contained within a single organisational structure. As the ecosystem expands and the stakeholders and protocol implementers exist outside of a single organisational structure, it becomes harder to manage the process of protocol evolution.

The Yellow Paper Committee exists as a means of managing this evolution while maintaining the protocol as a pure, formal, implementation-neutral specification which favours no development team or organisation. 

## Overview

The Yellow Paper Committee is a minimally-funded, constitutionally-driven DAO charged with only one task: providing an up to date hash of the git branch containing the latest canonical source code for the non-implementation specific specification of the Ethereum protocol. It works in concert with the EIP process and acts as a final decision-making body.

The minimal funding is used for two things:

- Paying to have the formal specification updated from a (less-formal) EIP specification;
- paying travel and accommodation expenses of the Ethereum implementers for a physical meeting.

The DAO's constitution essentially describes the critical aspects of the present document.

The DAO has two groups of identities: an Ethereum Implementer Group (EIG) and a Ethereum General Assembly (EGA). The EIG exists as a voting body to ratify alterations to this constitution and to the formal specification. Membership for the EIG is limited to those people who have, themselves, contributed most of an independent implementation of the protocol described in any canonical Yellow Paper of the previous `ancient_impl` months (members may unite to remove delegates representing out-of-date implementations); it should be demonstrably functional and should not borrow substantially from any other single implementation (e.g. line-by-line translations of a single implementation into another language should not qualify). The members of the EIG are charged with interpreting these rules when judging potential new entries. No single person or organisation may be allowed to materially influence more than `gang_bound` of the total membership; if this is the case, then members shall act, in good conscience, to remedy the situation. Membership may not be withheld for any other reasons.

The EIG has a rotating chair. The role of the chair is to submit potential alterations, known as _proposals_.  A proposal is simply a hash to a commit in a git repository; the provenance and author(s) of a proposal is immaterial. It may take the form of a (semi-formal) EIP or a (properly formal) pull-request to the yellow paper repository. Proposals may be ratified through a voting process described later. If an EIP is ratified, available funds may be spent by the chair to submit a further formalising proposal which shall be the pull-request counterpart to the ratified EIP. This must go through the same ratification phase. Members should not withhold ratification except for reasons that the proposals are materially different. The meaning of "materially" is left to their conscience; EIPs should be as formal and unambiguous as possible to avoid a sensitive meaning of "materially" hold up ratification.

The EGA exists as a forum to help air, clarify and formalise the views of the community. It should rightly include middleware developers, application developers, infrastructure projects, commercial endeavours powered by Ethereum, substantial holders of ether and affiliate organisations. Inclusion and expulsion happens through voting: all members of the EGA may vote; a greater number of positive to negative votes is needed to ratify membership, and it must happen with a quorum greater than `ega_vote_quorum` of the EGA membership. Membership may be withheld only because the proposed member is not a sufficiently great stakeholder in the Ethereum ecosystem or because it would allow a single interest to directly or indirectly influence greater than `gang_bound` of the total vote. Membership of the EGA elapses after `ega_membership_renewal` and must be renewed with new membership proposal.

For any given proposal, all EIP members have a vote and may execute a single veto. The proposal may be resubmitted in an unaltered form only after the `resubmission_period` has elapsed. Any member who has previously vetoed a particular proposal may never veto it again. Aside from the members, one further vote is reserved for the EGA. The EGA may vote either positively or negatively. A positive vote translates into a positive vote for the proposal; a negative overall vote into an abstention. The EGA does not have a veto. For a proposal to pass, there must be a strict majority of positive votes and no valid veto.

The EIG chair may propose funds be spent on a meeting of all EIG members. Modest accommodation and standard class travel may be expensed to the DAO; any other expenses, including subsistence, may not. All expenses must be receipted and declared publicly. The EGA must ratify the expenses through an overall positive vote of `ega_vote_quorum` members. The EIG has no authority to ratify or refund expenses.

#### Suggested Parameters

- `resubmission_period`: 3 months;
- `ancient_impl`: 6 months;
- `ega_vote_quorum`: 50%;
- `ega_membership_renewal`: 12 months;
- `gang_bound`: 25%;

.. _chapter-problem:

Problem and purpose
===================

The multi-organizational agentic system
---------------------------------------

A single agentic AI system in production is the work of several independent
organizations. A model provider trains and serves the model. One or more
developers or fine-tuners adapt it. A deployer places it inside a business
process. Infrastructure hosts run it. The organizations whose processes the
agents act within, and the humans those processes serve, complete the chain.
Each party answers to its own obligations, often under a different regime.
No party controls the whole system.

Identity establishes who acts while authorization establishes what the
authenticated party may access. However, for an agent, sanctioned operation
requires a third question to be answered: whether, and under what conditions,
that party should be trusted to act in a given operation. The agreements
between the organizations answer that question statically. The operation
contract carries that answer at runtime to the point of action.

When such a system fails, the failure is rarely confined to one party's
component. It arises between the parties. One party assumed an objective that
another never accepted. Nobody was assigned to monitor a condition. An
obligation was stated in a policy document and never carried into a check at
the point of action. A change at one party reached the others late or never.

Why existing instruments leave a gap
------------------------------------

Frameworks for AI risk management acknowledge the multi-party setting. The
NIST AI Risk Management Framework asks for risk to be managed across the AI
value chain. The EU AI Act requires, in Article 25, written agreements between
providers and deployers of high-risk systems that specify how obligations are
allocated. Management-system standards such as ISO/IEC 42001, and technical
alignment methods for models, are designed for one organization with control
over the lifecycle. The frameworks state what must be achieved. The content and
structure of the agreements that achieve it across organizations, and the
method for arriving at them, are left open. In practice the agreements are
written ad hoc, and the technical complexity of agentic systems outruns them.

The position within FG-TIDA
---------------------------

The work of FG-TIDA to date specifies the objects that cross the boundary
between two organizations at the moment of an agent action, and the records
that remain afterwards:

* the conferral record: the grant, its bounds, who conferred it, and its
  standing at the moment of the act (FG-TIDA/themes#5, the draft charter on
  provenance of authority);
* the operation contract and the decision record: what an agent may commit to
  without independent verification, which party verifies, the disposition when
  an input is absent or stale, and what the decision left behind (FG-TIDA WG2,
  deliverable 2; joint issue FG-TIDA/themes#60);
* the consultation of the record where acts take place, its recency, and the
  reach of a decided change (FG-TIDA/themes#61, Workstream E of the proposed
  trust control plane group);
* findings and amendments exchanged between organizations after an incident,
  received under the recipient's local authority (FG-TIDA/themes#13);
* whether a connection between two parties should exist and remain in force
  (FG-TIDA/themes#29);
* which authority vouches for an agent's identity, how delegated authority is
  scoped, and what one jurisdiction needs to recognise another's
  authorizations (FG-TIDA/themes#41).

Each of these takes the agreement between the organizations as given. The
operation contract is applied at an enforcement point. Where its conditions
come from, and how they relate to what the other organizations in the chain
have undertaken, is outside WG2's scope by design. The conferral record
carries a grant. The content of the grant is negotiated elsewhere. Workstream E
carries a change to the record. What counts as a change the parties must
honour is decided elsewhere. That "elsewhere" has no home in the Focus Group.

The object proposed for standardization
---------------------------------------

The objects FG-TIDA specifies are consumed at the moment of an action. The
grant in a conferral record, the conditions in an operation contract, and the
set of changes an enforcement point must honour are all decided before the
act, across organizational boundaries. This contribution proposes that
earlier process as the object to standardize. The process has inputs, steps,
outputs and properties that can be stated independently of any one of its
outputs.

Inputs
    The objectives the parties share for the initiative, the regimes each
    party declares, and each party's internal mandates.

Steps
    Identify the systemic drivers that bear on the objectives
    (:ref:`chapter-drivers`). State the obligations that address each driver
    as agreements at four layers (:ref:`chapter-architecture`). Formulate
    operation contracts from the agreements (:ref:`chapter-formulation`).

Outputs
    The domain-layer agreement between parties. The operation contracts under
    it, bound to the processes they serve. The record of coherence checks and
    approvals. The declared semantic residual.

Properties
    Traceability from a runtime check to the obligation it discharges.
    Confidentiality of each party's internal layer by construction. Coherence
    within and across layers, re-established whenever a layer changes.
    Identification of the agreement an artifact was issued under.

The outputs are what WG2, the work under FG-TIDA/themes#5 and Workstream E
consume. The process that produces them is held by none of them. Chapters 3
to 5 specify the process. Chapter 6 states which of its properties are
established in the author's prior work and which remain open.

Relation to the terms of reference
----------------------------------

The contribution maps to deliverables 4.3 (trust frameworks and lifecycle
management) and 4.4 (technical-policy and machine-readable trust metadata) of
the FG-TIDA terms of reference. Within Annex A, it addresses A.2.1, a reference
framework linking technical trust mechanisms with governance structures, and
A.2.5, trust interoperability requirements across jurisdictions and sectors.
A.3.3, the translation of policies into a machine-readable format, is adjacent
to its regulatory layer. The contribution stays inside the scope line the SG17
Chair drew for FG-TIDA/themes#41. It states which technical properties an
agreement structure must have so that requirements arising from a regime can
be applied to it.

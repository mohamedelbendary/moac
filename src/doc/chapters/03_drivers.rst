.. _chapter-drivers:

Systemic risk analysis method
=============================

Origin
------

The methodology paper this contribution derives from [ElBendary2026b]_ adapts
the work of Alberts and Dorofee, who developed a framework for categorizing
key drivers of risk in large software-intensive defense programs executed by
several independent enterprises with no central command authority
[Alberts2009]_. The framework was designed for the condition that defines
multi-organizational agentic AI. Objectives are pursued through negotiated
collaboration. Local incentives conflict. Counterparty risk and emergent risk
escape any single party's risk register.

The framework tames the complexity of such settings by working top down. It
starts from the objectives of the program and identifies the drivers, the
conditions and factors that strongly influence whether the objectives are
reached. Tactical risks from individual activities stay in each party's own
risk register. The result is a manageable set of drivers, each a short step
from an objective, which the human parties can reason about.

The six dimensions
------------------

Alberts and Dorofee analyse a program along six dimensions. The five driver
categories of this contribution derive from them.

Objectives
    The purpose and scope of the initiative, stated as the future state it is
    meant to create. Assessed for coherence across parties and for
    achievability with current capabilities.

Preparation
    The processes, resources and values that must be in place to mobilize a
    strategy that is aware of its environment.

Execution
    How tasks and activities are managed and performed, including dependency
    management and indicators, across capital, people, technology and other
    assets.

Environment
    External factors acting on execution: laws and regulations, market forces,
    organizational structure, culture, politics and tacit knowledge.

Resilience
    The levers available under specific risk scenarios, and the adaptability
    built into the strategy for unforeseen events.

Result
    What constitutes successful delivery of the system, successful operation
    once deployed, and the preconditions for deployment and maintenance, with
    responsibilities allocated accordingly.

Adaptation to agentic AI initiatives
------------------------------------

The driver analysis keeps the top-down direction. An initiative begins by stating
the objectives the parties share (for example "fair selection" in a hiring
process, or "no payment above the mandate's limit"), and then identifies the
drivers that bear on each objective. For each driver the parties record a
definition, the objectives it relates to, the responsibilities of each
organization, and a risk synopsis stating what happens when the driver is
neglected. The output of the analysis is the set of obligations the
agreements of :ref:`chapter-architecture` must state. The analysis assumes
that each party's own risk management continues under the frameworks that
apply to it.

The starter set comprises 22 drivers in five categories. The categories are
summarized in the next section; the full set is in the annex
(:ref:`annex-drivers`). It is industry and jurisdiction agnostic by design, so
that an initiative can start without analysis paralysis. The parties begin
from the set, keep the drivers that bear on their objectives, add those their
setting requires, and discard the rest. The fifth category,
cross-organizational coordination, is the one that distinguishes the
multi-party setting. Where a single organization holds full control of the
initiative, the framework reduces to four categories.

Driver categories
-----------------

The categories are summarized here. The full starter set, with each driver's
primary owner and the objectives it supports, is in :ref:`annex-drivers`.

Data ecosystem
    How data is sourced, managed and kept aligned across the lifecycle:
    training data quality and representativeness, data provenance and
    lineage, deployment data alignment, cross-boundary data governance, and
    training data sufficiency. Together these drivers support accuracy,
    fairness, transparency and auditability, and depend on consistent data
    stewardship across the parties.

Model capability and behaviour
    The technical soundness of the model in operation: architecture
    appropriateness for the task and its risk exposure, uncertainty
    quantification and out-of-distribution detection, emergent capability
    management, interpretability and explainability, and adversarial
    robustness including resistance to prompt injection.

Human-AI interaction
    How people supervise and learn from the system: human oversight
    effectiveness, including intervention, refusal and kill-switch pathways;
    user interface and experience design that communicates purpose and
    boundaries; AI literacy and training across the organizations; and
    feedback and improvement mechanisms that return user and system insight
    to the product cycle.

Cross-organizational coordination
    The collaborative mechanisms the multi-party setting requires: objective
    alignment among providers, fine-tuners, deployers and regulators;
    bidirectional information sharing of technical, operational and risk
    intelligence; contractual clarity delineating responsibilities and
    liabilities across the chain; and incident response coordination for
    cross-boundary failures and breaches.

Regulatory and operational compliance
    Operation within an evolving landscape of international and sectoral law:
    regulatory monitoring, documentation and audit readiness, conformity
    assessment readiness for high-risk systems, and change management and
    versioning that keeps modifications from compromising compliance.

Worked driver
-------------

**Change management and versioning** (regulatory and operational compliance).

Definition
    The condition that a change to any component the agentic system depends
    on (model version, policy reference, operation contract, conferral
    record) takes effect at the point of action only after the parties'
    agreed checks, and leaves a record of when it took effect.

Related objectives
    Reliability, compliance, accountability.

Responsibilities
    Provider: announce a model version change with its effective time, and
    keep the prior version available for the agreed window. Deployer: re-run
    the coherence check of the affected operation contracts against the new
    version before further acts proceed, and record the version in force at
    each decision. Host or model router: ensure the inference infrastructure serves the model
    version the deployer requests for the act.

Risk synopsis
    A provider changes the model under a contract approved for the previous
    version. Acts after the change proceed under conditions never checked
    against the new version. Decision records before and after the change
    look alike. Where the driver is unaddressed, no party has breached an
    obligation, and the loss has no owner. Where it is addressed, the record
    shows the version in force at each decision and which party failed its
    obligation.

The worked driver shows the shape of the output: an obligation for each
party, stated in terms both can verify, and a consequence that names which
party bears the loss when the obligation is unmet. It also shows the link to
the record. The recency and consulted-version requirements on
FG-TIDA/themes#60 are the operation-layer form of this driver.

Relation to themes in FG-TIDA's record
--------------------------------------

Several drivers correspond to objects already under specification in
FG-TIDA. Contractual clarity and objective alignment are what the conferral
record (FG-TIDA/themes#5) and the domain-layer agreement make concrete.
Incident response coordination is the object of FG-TIDA/themes#13's F3
function. Human oversight effectiveness is the object of FG-TIDA/themes#16.
Change management and versioning is the worked driver above. The driver analysis supplies
the step before each of these. It decides, per initiative, that the driver
bears on an objective and which party owns it.

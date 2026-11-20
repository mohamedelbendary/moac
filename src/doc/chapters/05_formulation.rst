.. _chapter-formulation:

Contract formulation process
============================

Principle
---------

Contracts are formulated from the semantics of the operations they govern.
An operation in a business process (reviewing a resume, approving a loan,
releasing a shipment) exists independently of the technology that performs
it. Its normative definition lives in standard operating procedures, in
process documentation and in the tacit knowledge of the people who perform it
today. That knowledge is the source of the contractual obligations.

The work this requires is less than it appears. Identifying operation
boundaries, inputs and outputs, preconditions, postconditions, and success
and failure conditions is standard systems analysis, performed to some degree
of formality in any well-engineered system; domain modelling [Evans2003]_
supplies the entities, attributes and behaviours the contracts refer to. The process below organizes that
existing work under the four-layer architecture so that it yields operation
contracts without a separate modelling effort. It also forces an early
question. Is an AI solution needed for the operation at all, given the cost
and the risk exposure it adds?

Steps
-----

#. **Identify the use case.** Select a business process suitable for AI
   augmentation, with clear boundaries, identifiable stakeholders across the
   participating organizations, and operational significance.

#. **State the objectives and the drivers.** Express the objectives the
   parties share for the use case, run the driver analysis of
   :ref:`chapter-drivers`, and record for each retained driver its owner and
   its risk synopsis. This step populates the domain layer with the
   obligations the operation contracts will have to discharge, and surfaces
   the regulatory and enterprise constraints that bind them.

#. **Assess data maturity and observability.** Establish whether every input
   and state variable an operation will need is available, captured reliably,
   and observable at execution time. Where gaps exist, language models
   grounded in the organization's own documentation may extract process
   activities into an Entry-Task-Validate-Exit form for human validation.

#. **Express the use case semi-formally.** Write it as a fully dressed,
   sea-level use case [Cockburn2001]_: actors and goals, main success path,
   alternate flows, failure paths, and escalation conditions, so that every
   execution scenario the contracts must cover is explicit. The same form
   expresses aligned behaviour whether the interaction is human to agent or
   agent to agent.

#. **Identify the intelligent behaviours.** Within the use case, name the
   decision-making or interpretive responsibilities an agent will carry out,
   distinguishing them from mechanical steps.

#. **Decompose into operations.** Break each intelligent behaviour into
   atomic operations with distinct responsibilities, boundaries that can be
   verified independently, and inputs drawn from observable state.

#. **Define the operation contract.** For each operation, specify required
   and optional inputs, preconditions, postconditions, invariants, failure
   end conditions, and the special conditions for termination, escalation,
   rollback and human engagement. Where permitted conduct differs between
   value streams, model separate operations with separate contracts.

#. **Separate structural and semantic predicates.** Classify each condition
   as structural, enforced by a deterministic verifier, or semantic,
   delegated to a separately governed inference layer with its own
   assurance requirements. Conditions that require interpretation of content
   are semantic; everything decidable over observable inputs is structural.

#. **Validate completeness and coherence.** Confirm that every path in the
   use case is covered by a contract, that no contracts conflict, that every
   predicate is grounded in the domain model and in observable state, and
   that no contract relaxes a constraint from the layers above. Compile each
   contract into machine-readable form (JSON is one example) and obtain the
   approval of the legal person responsible for its deployment.

Where generative AI assists, and where it does not decide
----------------------------------------------------------

Steps 3 to 7 can be AI-assisted. A grounded domain ontology and the use-case
form make language models serviceable as a compilation layer from the
organization's prose (policies, procedures, training manuals) to draft
contracts. Correctness is never derived from the model's output. It is
established by the deterministic validation in step 9 and by the human
approval that precedes deployment. The contract verification path keeps its
integrity whatever produced the draft.

Outputs
-------

The process yields, per use case: the retained drivers with owners; the
domain-layer agreement terms that discharge them; the set of operation
contracts under that agreement, each bound to the value stream it serves and
to its verifier; and the record of the coherence check and approval. A
receiving organization inspects the domain terms and the operation-layer
interface. The enforcement point reads the contract in force at decision
time.

.. _chapter-scope:

Scope, target and served work
=============================

Scope
-----

This contribution covers:

* a method for identifying, from the objectives of a multi-organizational
  agentic AI initiative, the systemic conditions that can defeat those
  objectives, and for allocating responsibility for each condition to a party;
* a layered structure for the agreements between the parties, with a
  composition rule that states what a party may rely on from a counterparty;
* the traceability from a requirement at the regulatory layer to a
  machine-verifiable check at the operation layer, and the coherence conditions
  that hold between layers;
* a process for formulating operation contracts from business process
  analysis, aligned with the operation contract discovery process of the
  containment architecture [ElBendary2026a]_.

Position on machine-readable regulation
---------------------------------------

The architecture assumes no machine-readable form for regulation. The
regulatory layer records obligations as written, in prose, with a legal person
accountable for the reading of them. Translation into a form the parties can
be held to happens at the enterprise and domain layers, by people, under
approval, with each term traceable to its source. At the operation layer every
condition is classified as structural or semantic. A structural condition is
decidable over inputs the deployment can observe and is verified
deterministically. A semantic condition requires interpretation. It is
delegated to a separately governed inference layer, with an owner, an assurance
requirement, and a stated disposition when assurance is insufficient.

A regulatory obligation therefore reaches the point of action in one of two
forms: as a structural predicate with full traceability, or as a declared
semantic residual with an owner and a bound. The driver analysis decides, per
initiative, which obligations take which form. The layering keeps the residual
visible. Some regulatory content will stay in the second form indefinitely.
That is the case the process exists to manage.

Out of scope
------------

* Encodings, schemas, wire formats and protocols for any of the objects named
  here. The operation layer is described by what it must state.
* Assessment of any national or regional regime. Regulatory requirements
  appear as inputs to the regulatory layer, cited by example.
* The verdict on a single action, which is WG2's; the provenance and standing
  of a grant, which is the work under FG-TIDA/themes#5; the availability and
  consistency of the record where acts consult it, which is Workstream E of
  the proposed trust control plane group; records and reconstruction after the
  act, which is the work under FG-TIDA/themes#1.
* Semantic safety of model outputs. The architecture places semantic
  conditions in a separately governed inference layer and bounds the residual
  risk. Reducing that risk is the inference layer's work.

Declared target
---------------

The contribution is submitted with the target **no working group yet**. Its
object is the process by which the organizations of an agentic system
coordinate its operation. WG0, WG1 and WG2 hold no such object. The proposed
trust control plane group places it outside its workstreams. The author asks
the incubation committee to read the contribution against the work it serves,
listed below, and to dispatch it as the committee sees fit.

Work served
-----------

.. list-table::
    :header-rows: 1
    :widths: 28 72

    * - FG-TIDA work
      - What this contribution supplies to it
    * - WG2, deliverable 2 (enforcing security policy on agent actions)
      - The origin and lineage of the operation contract the enforcement point
        applies: how its conditions descend from the domain and enterprise
        layers, and the coherence check that must pass when an upper layer
        changes.
    * - Joint issue FG-TIDA/themes#60
      - The authoring side of the "operation contract in force" row: which
        inputs an operation requires is decided at the domain layer and stated
        in the contract.
    * - FG-TIDA/themes#5 (provenance of authority)
      - The content of a grant between two organizations as a domain-layer
        agreement, and the regulatory and enterprise constraints it must not
        relax.
    * - FG-TIDA/themes#29 (governed connection decisions)
      - The basis each party accepts for forming and maintaining a connection,
        as the domain-layer agreement, with its change behaviour given by the
        coherence rule.
    * - FG-TIDA/themes#41 (technical requirements arising from governance)
      - A structure for what the policy an artifact references must contain,
        and how policies issued under different regimes map to each other at
        the domain layer.
    * - FG-TIDA/themes#13 (ecosystem-level defense)
      - The obligations under which a finding or amendment from another
        organization is received and acted upon, as domain-layer terms.
    * - FG-TIDA/themes#61, Workstream E (act-time consultation)
      - What counts as a change to the record that the parties have agreed to
        honour, and at which layer it is decided.
    * - FG-TIDA/themes#62 (agent discovery and cross-border trust), deliverable 3
      - The agreement behind the evidence a discovery record points to, where
        recognition across jurisdictions is written.

Conventions
-----------

The document is descriptive. "Must" and "may" describe properties of the
proposed architecture and carry no normative force outside it.
Theme and issue references of the form FG-TIDA/themes#n refer to the FG-TIDA
GitHub repositories as of the date of this document.

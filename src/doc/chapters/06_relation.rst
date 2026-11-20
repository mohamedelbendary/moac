.. _chapter-relation:

Relation to FG-TIDA work and open questions
===========================================

Mapping to the record
---------------------

.. list-table::
    :header-rows: 1
    :widths: 24 16 60

    * - FG-TIDA item
      - Layer
      - How the item relates to the layer
    * - Conferral record (themes#5)
      - Domain
      - The grant, its bounds and who conferred it are domain-layer terms
        between the conferring and receiving parties. The regulatory and
        enterprise layers above state what the grant may not relax.
    * - Operation contract in force (themes#60, part B; WG2 D2)
      - Operation
      - Identical object. This contribution supplies its lineage: the
        domain term each condition implements, and the re-check when the
        upper layer changes.
    * - Decision record (themes#60, part C; themes#1)
      - Operation
      - Produced under the operation contract. Crosses the boundary only as
        the domain terms require. Its content is WG2's. Its record-side
        properties are themes#1's.
    * - Basis for a connection (themes#29)
      - Domain
      - The domain-layer agreement is the basis. The cross-layer coherence
        condition is its change behaviour.
    * - What a policy must contain; regime mapping (themes#41)
      - Regulatory, domain
      - The regulatory layer declares the regime per party; the domain layer
        is where policies issued under different regimes are reconciled as
        terms both parties accept.
    * - Findings and amendments across organizations (themes#13)
      - Domain
      - Received under terms the domain agreement states. Confer no
        authority. May bear on a declared precondition and so trigger
        re-evaluation at the operation layer.
    * - Reach of a decided change (themes#61, Workstream E)
      - Domain, operation
      - What the parties agreed to honour as a change is a domain-layer
        term. Its effect at the point of action is the operation contract's
        coherence lifecycle.
    * - Cross-border recognition (themes#62, deliverable 3)
      - Regulatory, domain
      - The evidence a discovery record points to is issued under a domain
        agreement between parties whose regulatory layers differ.
        Recognition requirements are requirements on that agreement.
    * - Layered security stack (WG2 issue #5 on the charter repository)
      - All
      - The four contract layers are orthogonal to the four enforcement
        layers (identity, resource access, role-structural, semantic). The
        contract layers say where an obligation is authored. The enforcement
        layers say which control applies it.

Open questions
--------------

The author states these as open, and invites the incubation committee and
any interested group to take them up.

Machine-readable form of regulatory obligations
    The architecture's position is stated in :ref:`chapter-scope`. What
    remains open is per regime: which obligations admit structural predicates
    at all, and how the semantic residual is kept bounded as regimes change.
    The SG17 Chair's statement on FG-TIDA/themes#41 identifies the same
    question. A.3.3 of the terms of reference is its natural home.

Identifier of the domain-layer agreement
    The operation contract is identified by version and content hash
    (LA-2.3, LA-2.5, LA-2.6 on FG-TIDA/themes#4). The process is identified
    by its value stream. Neither identifies the agreement between two
    organizations under which a process runs. One agreement can govern
    several processes. One process can run under several agreements over
    time. The traceability argument requires an identifier for the agreement,
    stable across reissuance of the contracts beneath it. No FG-TIDA text
    supplies it. Its form is unspecified here.

Coherence checking across layers
    Coherence within the operation layer is required by LA-2.7 and its
    4 November append. The containment architecture names cross-layer
    coherence among the properties a deterministic verifier establishes. No
    text states how coherence between a domain term and the contracts beneath
    it is checked, nor what happens when two parties' regulatory layers impose
    incompatible constraints on one domain agreement. Both are open.

Driver set validation
    The 22 drivers are a starter set derived from the six dimensions and the
    author's enterprise experience. Validation against submitted FG-TIDA use
    cases, in particular the multi-party cases under WG0, would confirm or
    revise the set.

Residual semantic risk
    The architecture bounds semantic risk to a separately governed inference
    layer and makes the residual explicit. Reducing it is the inference
    layer's work, outside the contract architecture's guarantees.

Proposed next steps
-------------------

#. Dispatch by the incubation committee to the group or queue it judges
   appropriate, with this document as the input.
#. Validation of the driver starter set against two or three multi-party
   use cases from the WG0 repository, with the resulting domain-layer terms
   and operation contracts published as a worked example.
#. Alignment of the operation layer's description with the final form of
   the "operation contract in force" row on FG-TIDA/themes#60, so that the
   two texts use one vocabulary.
#. A short study, under A.3.3 or wherever the Focus Group places it, of the
   regulatory layer in machine-readable form.

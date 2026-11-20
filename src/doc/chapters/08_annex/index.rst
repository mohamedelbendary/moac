.. _annex-drivers:

Annex: starter set of systemic risk drivers
===========================================

The starter set comprises 22 drivers in five categories. The properties column
names the objectives a driver typically supports; ownership is allocated per
initiative during the analysis of :ref:`chapter-drivers`, and the worked
driver in that chapter shows the form an allocation takes. Where a single
organization controls the initiative, the cross-organizational coordination
category may be omitted.

.. tabularcolumns:: |>{\raggedright\arraybackslash}p{0.20\linewidth}|>{\raggedright\arraybackslash}p{0.26\linewidth}|>{\raggedright\arraybackslash}p{0.46\linewidth}|

.. list-table::
    :header-rows: 1
    :class: longtable
    :widths: 22 30 48

    * - Category
      - Driver
      - Definition and properties supported
    * - Data ecosystem
      - Training data quality and representativeness
      - How well training data mirrors the deployment context and populations.
        Accuracy, fairness.
    * - Data ecosystem
      - Data provenance and lineage
      - Traceability of sources, transformations and rights across the data
        supply chain. Transparency, auditability.
    * - Data ecosystem
      - Deployment data alignment
      - Congruence between training and operational data distributions.
        Reliability, safety.
    * - Data ecosystem
      - Cross-boundary data governance
      - Enforcement of data policies, access control and privacy safeguards
        collaboratively among all parties. Privacy, accountability.
    * - Data ecosystem
      - Training data sufficiency
      - Adequacy of dataset volume and diversity for complete and reliable
        model behaviour. Reliability.
    * - Model capability and behaviour
      - Architecture appropriateness
      - Fit of the model design to the task, operational constraints and risk
        exposure. Performance, efficiency.
    * - Model capability and behaviour
      - Uncertainty quantification
      - How well the model expresses confidence and identifies
        out-of-distribution scenarios. Safety, reliability.
    * - Model capability and behaviour
      - Emergent capability management
      - Controls to detect and mitigate unintended or novel behaviours in
        large models. Safety.
    * - Model capability and behaviour
      - Interpretability and explainability
      - Decisions understandable, auditable and transparent across
        stakeholders. Transparency, accountability.
    * - Model capability and behaviour
      - Adversarial robustness
      - Resilience against malicious perturbation and prompt injection.
        Security, reliability.
    * - Human-AI interaction
      - Human oversight effectiveness
      - Ability of people to monitor, comprehend and intervene, including
        intervention, refusal and kill-switch pathways. Safety,
        accountability.
    * - Human-AI interaction
      - User interface and experience design
      - How the system communicates purpose, boundaries and functions.
        Trust, effectiveness.
    * - Human-AI interaction
      - AI literacy and training
      - Personnel understanding of capabilities, limitations and risks across
        the organizations. Appropriate and safe use.
    * - Human-AI interaction
      - Feedback and improvement mechanisms
      - Channels returning user and system insight into enhancement cycles.
        Continuous correction.
    * - Cross-organizational coordination
      - Objective alignment
      - Shared understanding of goals and commitments among providers,
        fine-tuners, deployers and regulators. Coherence of the initiative.
    * - Cross-organizational coordination
      - Information sharing
      - Bidirectional exchange of technical, operational and risk
        intelligence. Coordination, risk mitigation.
    * - Cross-organizational coordination
      - Contractual clarity
      - Formal delineation of responsibilities and liabilities across the
        chain. Accountability.
    * - Cross-organizational coordination
      - Incident response coordination
      - Joint procedures for identifying, investigating and resolving
        cross-boundary failures and breaches. Resilience.
    * - Regulatory and operational compliance
      - Regulatory monitoring
      - Continuous tracking of and response to jurisdiction-specific
        requirements as they evolve. Compliance.
    * - Regulatory and operational compliance
      - Documentation and audit
      - Accuracy, completeness and accessibility of system records to
        auditors and regulators. Transparency, accountability.
    * - Regulatory and operational compliance
      - Conformity assessment
      - Readiness for formal evaluations of compliance with legal or
        market-entry standards. Compliance.
    * - Regulatory and operational compliance
      - Change management and versioning
      - Regulatory integrity maintained across system updates. Compliance,
        stability.

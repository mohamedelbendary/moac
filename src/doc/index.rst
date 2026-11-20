.. raw:: latex

    \pagestyle{plain}
    \thispagestyle{plain}
    \let\osiaorigaddcontentsline\addcontentsline
    \renewcommand{\addcontentsline}[3]{}

.. _chapter-overview:

Multi-Organizational Operational Coordination for Agentic AI
=============================================================

Abstract
--------

An agentic AI system in production is operated by several independent
organizations: a model provider, developers or fine-tuners, a deployer,
infrastructure hosts, and the organizations whose processes the agents act
within. Each holds different obligations under different regimes. None controls
the whole system.

FG-TIDA work to date specifies the objects that cross the boundary between two
such organizations at the moment of an agent action: the conferral record
(FG-TIDA/themes#5), the operation contract and the decision record (WG2;
FG-TIDA/themes#60), the consultation of the record where acts take place
(FG-TIDA/themes#61, Workstream E), and findings exchanged after an incident
(FG-TIDA/themes#13). No theme or working group addresses the process by which
those organizations coordinate the operation of the shared system as a whole:
how they state the objectives the system serves, identify the conditions that
can defeat them, allocate responsibility for each condition, and write the
agreements that keep that allocation enforceable at runtime. The grant, the
contract conditions and the admissible changes listed above are all drawn from
those agreements.

This contribution proposes the process as a standardization object in its own
right. It assumes that each organization runs its own risk management under
the frameworks that apply to it, such as the NIST AI RMF or ISO/IEC 42001, and
starts where those frameworks stop: at the agreement between organizations and
its carriage to the point where an agent acts. It specifies two instruments.
The first is a driver analysis for multi-organizational agentic AI
initiatives, adapted from Alberts and Dorofee's method for multi-enterprise
programs. It derives, from the objectives the parties share, the conditions
each party must answer for, and yields the obligations the agreements must
state. A starter set of 22 drivers in five categories seeds the analysis. The
second is a four-layer contract architecture (regulatory, enterprise, domain,
operation). Obligations
identified through the drivers are stated as agreements at those layers,
composed by an assume-guarantee rule, and traced to the operation contract an
enforcement point applies. The architecture assumes no machine-readable form
for regulation. Regulatory obligations reach the point of action as
deterministic checks where they can be stated over observable inputs, and
otherwise as a declared semantic residual with an owner and a bound.

The contribution is submitted with no working group as target. Its outputs
serve the work under FG-TIDA/themes#5, #13, #29 and #41, WG2 deliverable 2,
and Workstream E of the proposed trust control plane group. It maps to
deliverables 4.3 and 4.4 of the terms of reference and to Annex A items A.2.1
and A.2.5.

History
-------

.. tabularcolumns:: |>{\raggedright\arraybackslash}p{0.08\linewidth}|>{\raggedright\arraybackslash}p{0.40\linewidth}|>{\raggedright\arraybackslash}p{0.12\linewidth}|>{\raggedright\arraybackslash}p{0.10\linewidth}|>{\raggedright\arraybackslash}p{0.20\linewidth}|

.. list-table::
    :header-rows: 1
    :widths: 10 40 14 12 24

    * - Version
      - Document
      - Date
      - Focus Group
      - Working Group
    * - 0.1
      - Multi-Organizational Operational Coordination for Agentic AI
      - 2026-11-19
      - TIDA
      - No working group yet

Authors
-------

.. tabularcolumns:: |>{\raggedright\arraybackslash}p{0.17\linewidth}|>{\raggedright\arraybackslash}p{0.33\linewidth}|>{\raggedright\arraybackslash}p{0.42\linewidth}|

.. list-table::
    :header-rows: 1
    :widths: 18 34 48

    * - Name
      - Affiliation
      - Contact
    * - Mohamed ElBendary
      - Individual capacity (independent expert, United States)
      - mohamed.elbendary@gmail.com

Keywords
--------

Agentic AI, multi-organizational coordination, operational coordination,
agreements between organizations, operation contract, traceability, trust
interoperability.

.. raw:: latex

    \newpage

Foreword
--------

Agentic AI systems now act as autonomous entities capable of reasoning, planning, and
executing tasks across services, infrastructures, and organizational boundaries. This
fundamentally changes the nature of identity in digital systems: identity is no longer
limited to human users and static machine instances but must also encompass autonomous,
dynamic, and goal-oriented agents. And identity alone is insufficient: the core question
extends beyond "what an entity is" to "whether, and under what conditions, that entity
should be trusted to act".

The Focus Group on Trust and Identity for humans and agentic AI (FG-TIDA) addresses trust
management and interoperable digital identity infrastructure for humans and for agentic AI,
supporting the development of secure, trustworthy digital ecosystems in which humans and
agentic AI can safely interact and collaborate.

FG-TIDA was established under Recommendation ITU-T A.7 (Focus groups: Establishment and
working procedures), with ITU-T Study Group 17 as its parent group. Further details are
available in the group's terms of reference.

Note
----

This document is a contribution to the first FG-TIDA meeting, submitted in the
author's individual capacity. The content derives from two publications by the author, listed in the references:
a methodology paper on multi-organizational AI coordination enforceable at
runtime, presented at the AAAI 2026 Workshop on AI Governance (Singapore,
2026), and an architecture paper published in the IntelliSys 2026 proceedings
(Springer LNNS). The author requests clause-level attribution of
any part of this contribution that a working group takes up, per the working
methods the FG-TIDA charters have adopted.

Material prepared with the assistance of generative AI tools was reviewed and
approved by the author, who is responsible for the content.

.. raw:: latex

    \let\addcontentsline\osiaorigaddcontentsline
    \sphinxtableofcontents
    \osiamainmatter
    %% The toctree below sits inside the Note section, so Sphinx emits the
    %% body documents one level down. Shift LaTeX headings up one level so
    %% body documents are chapters, as in the HTML.
    \let\paragraph\subsubsection \let\subsubsection\subsection \let\subsection\section \let\section\chapter

.. toctree::
    :maxdepth: 3
    :numbered:
    :hidden:

    chapters/01_problem
    chapters/02_scope
    chapters/03_drivers
    chapters/04_architecture
    chapters/05_formulation
    chapters/06_relation
    chapters/07_references
    chapters/08_annex/index

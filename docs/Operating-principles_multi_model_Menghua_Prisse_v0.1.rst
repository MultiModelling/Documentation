Introduction

Multi-models better handle complex issues than singular-models due to
the combination of the strength of individual models [1,2]. However,
combining models is challenging on both technical and non-technical
levels. Technical challenges involve differences in the system design
and alignment of each model. Alignment involves several topics, the most
common being formalism, resolution, and scale. There are predominantly
two non-technical challenges. First, it becomes increasingly difficult
to understand and interpret the meaning of the numbers and outcomes
within a multi-model when they become more complex.

One of the critical challenges for multi-models is the coupling of
individual models and studying how the coupled models might affect the
outcome. This thesis focused on understanding which interaction
structures exist for coupling optimization and simulation models and how
the choices might affect the workings of the multi-model. Accordingly,
the overall research question was formulated as follows:

What is the effect of coupling an agent-based model to an existing
optimization model?

This thesis was conducted within the boundaries of the micro case of the
multi-modeling project. The case study area was the industrial area of
Tholen in Zeeland province. This thesis coupled two models: an
optimization and an agent-based model (ABM).

State-of-the-art

An ABM can be constructed by following a ten-step method [3]. One of the
main issues associated with coupling is interoperability [4–6]. Coupling
tightness refers to the fundamental concept of interdependence between
models, how they are connected, and their variables intertwined. Five
different levels of coupling tightness have been identified based on
coupling methodologies [7]. Four levels of interoperability have been
determined: technical, syntactical, semantic, and organizational [8].
Four model configurations for coupling a simulation and optimization
model have been provided [9].

Methods, results, and findings

An existing optimization model named Techno-Economic Analysis Of Complex
Option Spaces (TEACOS), developed by our project partner QUOMARE, was
used. It is a long-term optimization tool designed to facilitate the
transition towards low-carbon energy systems, identifying the most
profitable investments while adhering to supply-demand balances and
environmental constraints set by the modeler. Optional choices as input
to TEACOS are converted to fixed investment decisions based on the total
system cost minimization objective. Since TEACOS is not openly
available, an adapter was created that communicated with the model
through API calls (this creation was external to the master’s thesis
scope). The standard communication occurred via Energy System
Description Language (ESDL) files.

The industrial area of Tholen was selected because of its strong
intention towards low-carbon energy system transition. For this study,
the optional assets were limited to solar panels as the purpose was to
test the feasibility of the multi-model within the micro case.

An ABM was created to simulate the buying behavior of the companies in
Tholen. The Mesa modeling environment was chosen because of the relative
ease of linking with ESDL files and sufficient documentation related to
the tool. ABM aimed to simulate investment decisions in the optional
assets selected by TEACOS. One key outcome of the model was the number
and distribution of solar panels purchased by agents in a single
simulation run. The conceptual model consisted of environment, agents,
and time.

A short overview of model characteristics that are important for
coupling was presented to create a meaningful interface between models.
The modeling steps are conceptualization, implementation, verification
and validation, and implementing data. Conceptualization hypothesized
what a multi-model output might look like and how this would answer the
overall research question. This coupling is loose, i.e., the modeler
interfaces with each model using automated data transfer. The coupling
was executed using a Python script to call TEACOS, followed by the ABM,
for iterations. This allowed for the investigation into the ABM's
effects on the outcome of TEACOS. The implementation was performed using
Python script in the modeler’s integrated development environment.
Verification and validation ensured that the developed multi-model was
created correctly and performed the way it should. Data implementation
involved preparing ESDL files to be exchanged between the coupled
models.

Two key performance indicators (KPIs) were devised to facilitate the
multi-model investigation: investment trajectory returned by the
multi-model and inflection point KPI (iteration at which the suggested
optimum trajectory of investment alters). Dynamic experimental setup
allowed for a cyclical, adaptive approach to conducting experiments.
Observations indicated that KPIs stabilized after 6-8 iterations. When
the general tipping point was reached, TEACOS did not recommend further
investments, a little over 400 kW for PV array power output. Process
analyses demonstrated challenges faced during different phases of the
project. A two-dimensional array was created with axes representing
interoperability categories and research phases. Organizational and
technical interoperability proved to be the most cumbersome, with six
and five challenges, respectively.

Conclusion and future work

The iterative process of conceptualizing the ABM and the multi-model
resulted in a very fit ABM. When coupling models, high cohesion and low
coupling are desired [10], which this combination did. Overfitting of
coupled models should be avoided [11]. Instead, a generic ABM should be
created and connected via a wrapper or an adapter. This study highlights
the need for more focus on the broader organizational, practical context
within which the models operate, particularly related to different
operating principles. The limitation is the simplicity and abstraction
of the ABM, which might not capture the intricacies of human behavior.
The ABM still successfully fulfilled its core function of making
decisions, working with ESDL files, and interacting with the TEACOS
model. This study shows that coupling an optimization and agent-based
model is possible.

This research serves as a basis for integrating optimization and
simulation models in a more complicated manner in the future. This can
involve more interaction between models than only PV array capacity. ABM
can incorporate more complicacies of human behavior. Multi-period
optimization can be performed in a singular iteration.

A link to Menghua Prisse’s master thesis work follows:
https://repository.tudelft.nl/islandora/object/uuid:53acc329-7990-4fe0-8374-3418d10c3f85

Bibliography

[1] Duboz R, Ramat É, Preux P, Raphae¨ R, Duboz R, Ramat R. Scale
transfer modeling: Using emergent computation for coupling an ordinary
differential equation system with a reactive agent model. Systems
Analysis Modelling Simulation 2003;43:793–814.
https://doi.org/10.1080/0232929031000150355.

[2] Quesnel G, Duboz R, Ramat É. The Virtual Laboratory Environment – An
operational framework for multi-modelling, simulation and analysis of
complex dynamical systems. Simul Model Pract Theory 2008;17:641–53.
https://doi.org/10.1016/j.simpat.2008.11.003.

[3] van Dam KH, Nikolic I, Lukszo Z. Agent-Based Modelling of
Socio-Technical systems. n.d.

[4] Bollinger LA, Davis CB, Evins R, Chappin EJL, Nikolic I. Multi-model
ecologies for shaping future energy systems: Design patterns and
development paths 2017. https://doi.org/10.1016/j.rser.2017.10.047.

[5] Nikolic I, Warnier M, Kwakkel JH, Chappin EJL, Lukszo Z, Brazier FM,
et al. Principles, challenges and guidelines for a multi-model ecology.
Citation 2019.
https://doi.org/10.4233/UUID:1AA3D16C-2ACD-40CE-B6B8-0712FD947840.

[6] Rezaeiahari M, Khasawneh MT. Simulation optimization approach for
patient scheduling at destination medical centers. Expert Syst Appl
2020;140:112881. https://doi.org/10.1016/j.eswa.2019.112881.

[7] Brandmeyer JE, Karimi HA. Coupling methodologies for environmental
models. Environmental Modelling & Software 2000;15:479–88.
https://doi.org/10.1016/S1364-8152(00)00027-X.

[8] van der Veer H, Wiles A. Achieving Technical Interoperability-the
ETSI Approach. 2008.

[9] Figueira G, Almada-Lobo B. Hybrid simulation-optimization methods: A
taxonomy and discussion. Simul Model Pract Theory 2014;46:118–34.
https://doi.org/10.1016/j.simpat.2014.03.007.

[10] Hellhake D, Bogner J, Schmid T, Wagner S. Towards using coupling
measures to guide black-box integration testing in component-based
systems. Software Testing Verification and Reliability 2022;32.
https://doi.org/10.1002/STVR.1811.

[11] Shahumyan H, Moeckel R. Integrating Models for Complex Planning
Policy Analysis: Challenges and a Solution in Coupling Dissimilar
Models, Computers in Urban Planning and Urban Management; 2015.

 

===========================================
Optimization and Simulation model coupling
===========================================

Master thesis summary – Menghua Prisse


5 December 2023

Introduction
============

Multi-models better handle complex issues than singular models due to
the combination of the strength of individual models (`Duboz et al. 2003`_;
`Quesnel, Duboz, and Ramat 2008`_). However, combining models is
challenging on both technical and non-technical levels. Technical
challenges involve differences in the system design and alignment of
each model. Alignment involves several topics, the most common being
formalism, resolution, and scale. There are predominantly two
non-technical challenges. First, it becomes increasingly difficult to
understand and interpret the meaning of the numbers and outcomes within
a multi-model when they become more complex.

One of the critical challenges for multi-models is the coupling of
individual models and studying how the coupled models might affect the
outcome. This thesis focused on understanding which interaction
structures exist for coupling optimization and simulation models and how
the choices might affect the workings of the multi-model. Accordingly,
the overall research question was formulated as follows:

*What is the effect of coupling an agent-based model to an existing
optimization model?*

This thesis was conducted within the boundaries of the micro case of the
multi-modeling project. The case study area was the industrial area of
Tholen in Zeeland province. This thesis coupled two models: an
optimization and an agent-based model (ABM).

State-of-the-art
================

An ABM can be constructed by following a ten-step method (`van Dam,
Nikolic, and Lukszo n.d.`_). One of the main issues associated with
coupling is interoperability (`Bollinger et al. 2017`_; `Nikolic et al.
2019`_; `Rezaeiahari and Khasawneh 2020`_). Coupling tightness refers to the
fundamental concept of interdependence between models, how they are
connected, and their variables intertwined. Five different levels of
coupling tightness have been identified based on coupling methodologies
(`Brandmeyer and Karimi 2000`_). Four levels of interoperability have been
determined: technical, syntactical, semantic, and organizational (`van
der Veer and Wiles 2008`_). Four model configurations for coupling a
simulation and optimization model have been provided (`Figueira and
Almada-Lobo 2014`_).

Methods, results, and findings
==============================

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
==========================

The iterative process of conceptualizing the ABM and the multi-model
resulted in a very fit ABM. When coupling models, high cohesion and low
coupling are desired (`Hellhake et al. 2022`_), which this combination did.
Overfitting of coupled models should be avoided (`Shahumyan and Moeckel
2015`_). Instead, a generic ABM should be created and connected via a
wrapper or an adapter. This study highlights the need for more focus on
the broader organizational, practical context within which the models
operate, particularly related to different operating principles. The
limitation is the simplicity and abstraction of the ABM, which might not
capture the intricacies of human behavior. The ABM still successfully
fulfilled its core function of making decisions, working with ESDL
files, and interacting with the TEACOS model. This study shows that
coupling an optimization and agent-based model is possible.

This research serves as a basis for integrating optimization and
simulation models in a more complicated manner in the future. This can
involve more interaction between models than only PV array capacity. ABM
can incorporate more complicacies of human behavior. Multi-period
optimization can be performed in a singular iteration.

A link to Menghua Prisse’s master thesis work follows:
https://repository.tudelft.nl/islandora/object/uuid:53acc329-7990-4fe0-8374-3418d10c3f85


 Bibliography

Bollinger, L. A., C. B. Davis, R. Evins, E. J. L. Chappin, and I.
Nikolic. 2017. “Multi-Model Ecologies for Shaping Future Energy Systems:
Design Patterns and Development Paths.” https://doi.org/10.1016/j.rser.2017.10.047.

Brandmeyer, Jo Ellen, and Hassan A. Karimi. 2000. “Coupling
Methodologies for Environmental Models.” *Environmental Modelling &
Software* 15(5):479–88. https://doi.org/10.1016/S1364-8152(00)00027-X.

van Dam, Koen H., Igor Nikolic, and Zofia Lukszo. n.d. *Agent-Based
Modelling of Socio-Technical Systems*. https://link.springer.com/book/10.1007/978-94-007-4933-7. 

Duboz, Raphaël, Éric Ramat, Philippe Preux, Raphae¨l Raphae¨, Raphae¨l
Duboz, and Ric Ramat. 2003. “Scale Transfer Modeling: Using Emergent
Computation for Coupling an Ordinary Differential Equation System with a
Reactive Agent Model.” *Systems Analysis Modelling Simulation*
43(6):793–814. https://doi.org/10.1080/0232929031000150355.

Figueira, Gonçalo, and Bernardo Almada-Lobo. 2014. “Hybrid
Simulation-Optimization Methods: A Taxonomy and Discussion.” *Simulation
Modelling Practice and Theory* 46:118–34. https://doi.org/10.1016/j.simpat.2014.03.007.

Hellhake, Dominik, Justus Bogner, Tobias Schmid, and Stefan Wagner.
2022. “Towards Using Coupling Measures to Guide Black-Box Integration
Testing in Component-Based Systems.” *Software Testing Verification and
Reliability* 32(4). https://doi.org/10.1002/STVR.1811.

Nikolic, I., Martijn Warnier, J. H. Kwakkel, E. J. L. Chappin, Z.
Lukszo, F. M. Brazier, A. Verbraeck, M. Cvetkovic, and P. Palensky.
2019. “Principles, Challenges and Guidelines for a Multi-Model Ecology.”
*Citation*. https://doi.org/10.4233/UUID:1AA3D16C-2ACD-40CE-B6B8-0712FD947840.

Quesnel, Gauthier, Raphaël Duboz, and Éric Ramat. 2008. “The Virtual
Laboratory Environment – An Operational Framework for Multi-Modelling,
Simulation and Analysis of Complex Dynamical Systems.” *Simulation
Modelling Practice and Theory* 17:641–53. https://doi.org/10.1016/j.simpat.2008.11.003.

Rezaeiahari, Mandana, and Mohammad T. Khasawneh. 2020. “Simulation
Optimization Approach for Patient Scheduling at Destination Medical
Centers.” *Expert Systems With Applications* 140:112881. https://doi.org/10.1016/j.eswa.2019.112881.

Shahumyan, Harutyun, and Rolf Moeckel. 2015. “Integrating Models for
Complex Planning Policy Analysis: Challenges and a Solution in Coupling
Dissimilar Models.” Computers in Urban Planning and Urban Management. 
http://web.mit.edu/cron/project/CUPUM2015/proceedings/Content/modeling/208_shahumyan_h.pdf

van der Veer, Hans, and Anthony Wiles. 2008. *Achieving Technical
Interoperability-the ETSI Approach*.

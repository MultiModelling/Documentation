=======================================================
Scaling Analysis – Resolution difference-based coupling
=======================================================
--------------------------------------
Master thesis summary - Bram Boereboom
--------------------------------------


20 November 2023

Introduction 
=============

Energy infrastructure is expected to be an essential component of future
energy systems within the Netherlands. Models form the basis of
understanding complex interactions of energy systems. Many models that
analyze energy infrastructure are available. However, their capabilities
and scopes are scattered. Policymakers are interested in a comprehensive
oversight of information to provide informed decision-making on
integrated energy systems. Here, a multi-modeling concept with the scope
of scaling comes into the picture. In addition, models used for
energy-related decision support are either available at a higher
abstract level or do not contain the entire energy system. Separate
modeling of the system is insufficient when studying complex
socio-technical systems, as the behavior of the whole system is more
than the sum of the behavior of individual parts due to possible
interactions between system components (`Vangheluwe et al., 2002`_). One of
the main challenges of creating coupling infrastructure is addressing
issues related to bridging different resolution levels between models
(`Nikolic et al., 2019`_). ‘Resolution’ in this context corresponds to the
level of detail on which the models operate, related to space, time, or
modeled object (`Rabelo et al., 2016`_). The aim was to bridge the gaps
between models regarding the abovementioned resolution gaps by applying
the scaling method. Accordingly, the research question is formulated as
follows:

How can issues arising when coupling multiple energy models with
different resolutions be resolved effectively?

This thesis is part of a larger project aiming to create a multi-model
infrastructure to couple existing models to understand better complex
energy systems at different geographical scopes within the Netherlands
(`Nikolic, 2023`_). Bram focused on detecting and alleviating
coupling-related issues related to combining models with different
resolutions.

State-of-the-art
================

Brandmeyer and Karimi (`Brandmeyer & Karimi, 2000`_) suggested five levels
of coupling: one-way data transfer, loose coupling, shared coupling,
joined coupling, and tool coupling. Aggregation and Disaggregation (A/D)
of objects is complicated because this requires changing functions and
writing an adjacent model at a different resolution (`Salome, 2021`_). The
proper choice of resolution is decided by the purpose of a model (`Jie
Chen & Xiaoyu Li, 2021`_) and data availability (`Degbelo & Kuhn, 2018`_). It
is sometimes advantageous to use multiple low-resolution models instead
of a singular high-resolution model, such as for military simulation
(`Xuefei et al., 2017`_). Within a multi-model structure, all models can
contribute meaningfully to each other to create a more integral view of
a complex system (`Nikolic, 2023`_; `Seck & Honig, 2012`_).

Method, results, and findings 
==============================

The method involved creating a model audit for each model. During this
process, the auditing method was standardized to facilitate its reuse.
The audit enabled better model understanding and identified parameters
or variables to be considered when determining A/D functions and
consistency checks.

*Criteria for shortlisting models*

-  The models must vary in resolution sufficiently to provide a
   challenging gap to bridge

-  The models must be energy modeling-related

-  There must be a feasible case for why one would want to couple these
   models

-  The models must be readily available to research

Models shortlisted:

-  Energy Transition model (ETM) (`Quintel, n.d.`_)

-  Hydrogen-buffered Wind Power Model (HWP) (`Boereboom, n.d.`_)

-  Electric vehicle power demand Model (EVM) (`Boereboom, n.d.`_)

Two coupling cases were finalized:

-  ETM-HWP coupling: ETM provided electricity price, power production,
   and wind speed. HWP model derived the profitability of a wind farm.
   This is a one-way connection from ETM to HWP. The coupling is static.
   The resolution difference is related to wind farm modeling details.

-  ETM-EVM coupling: ETM provided electricity price and population
   information (along with growth) to EVM. EVM calculated electric
   vehicle (EV) electricity demand and storage supply curves. ETM has a
   national approach, while EVM distributes agents across space at a
   municipality level. This coupling effort tried to address spatial
   resolution difference-based challenges in multi-modeling.

..

   The method involved three steps:

1) Model auditing: a set of questions was prepared as a guide to
   understand or investigate critical elements related to each model
   resolution to have a complete model audit.

2) Coupling auditing: Each model coupling underwent an audit to identify
   variable-related issues and suggested mitigation strategies.

3) Coupling implementation: with the knowledge of coupling issues and
   steps to mitigate them, an actual coupling was implemented.

Results showed that increasing the price of electricity and power supply
increases the cash flow from wind farms (ETM-HWP coupling). Changing the
electricity price does not have any impact on the constraints of the HWP
model, whereas changing the power output has minimal impact. With an
increase in the hourly electricity price input to the EVM (ETM-EVM
coupling) and an increase in the national population (translated into an
increase in municipality population), the mean national power demand and
mean national vehicle-to-grid capacity increased. Changing only the
electricity price did not impact the aspects mentioned above.

The results provided a clear overview of the effectiveness and limits of
the described method to alleviate resolution-based coupling challenges.

Conclusions and future work 
============================

This study was an exploratory modeling effort conducted to reflect the
feasible consistency limits of various techniques to the stakeholders to
which the models belong. Some of the essential conclusions from the
couple auditing activity are:

-  the main research question can be answered by using a coupling
   process based on audits, comprised of questions aimed at detecting
   issues and checking the effectiveness of the means to solve the
   problems\ *.*

-  System expertise is highly advantageous for identifying and tackling
   problems encountered during the auditing and coupling process.

-  Coupling models with different resolutions requiring aggregation and
   disaggregation efforts need an intermediate data model to translate
   and (possibly) store data to facilitate coupling.

-  The coupling of two models will likely require constructing an A/D
   effort specifically tailored to the needs of the models in question.

-  It is challenging to determine what constitutes a good consistency or
   sufficient overlap. There are no benchmarks to compare with.

In the future, we have options to carry on the research by Bram in the
following manner:

-  Use the macro case, which performs scaling activity, to analyze the
   demand distribution of different sectors at a regional level.

-  Identify the differences in the impact of energy infrastructure
   between the national and regional levels regarding interregional
   energy flows, investment, and technical characteristics.

   A link to Bram Boereboom’s master thesis work follows:

https://repository.tudelft.nl/islandora/object/uuid%3A6b5867d3-e6bb-46f8-bf2a-aea9399cae17

 Bibliography

Boereboom, B. (n.d.). *EVM and HWP model*. 2022. Retrieved November 16,
2023, from https://github.com/bramboereboom/MSc-thesis

Brandmeyer, J. E., & Karimi, H. A. (2000). Coupling methodologies for
environmental models. *Environmental Modelling & Software*, *15*\ (5),
479–488. https://doi.org/10.1016/S1364-8152(00)00027-X

Degbelo, A., & Kuhn, W. (2018). Spatial and temporal resolution of
geographic information: an observation-based theory. *Open Geospatial
Data, Software and Standards 2018 3:1*, *3*\ (1), 1–22.
https://doi.org/10.1186/S40965-018-0053-8

Jie Chen, & Xiaoyu Li. (2021). *Research on Key Technologies of
Multi-resolution Modeling Simulation*. 687–693.

Nikolic, I. (2023). *Towards integrated decision-making in the energy
transition*. https://multi-model.nl/

Nikolic, I., Warnier, M., Kwakkel, J. H., Chappin, E. J. L., Lukszo, Z.,
Brazier, F. M., Verbraeck, A., Cvetkovic, M., & Palensky, P. (2019).
Principles, challenges and guidelines for a multi-model ecology.
*Citation*.
https://doi.org/10.4233/UUID:1AA3D16C-2ACD-40CE-B6B8-0712FD947840

..Quintel, n.d.. *Energy Transition Model*. Retrieved December 10, 2019,
from https://energytransitionmodel.com/?locale=en

Rabelo, L., Kim, K., Park, T. W., Pastrana, J., Marin, M., Lee, G.,
Nagadi, K., Ibrahim, B., & Gutierrez, E. (2016). Multi resolution
modeling. *Proceedings - Winter Simulation Conference*, *2016-February*,
2523–2534. https://doi.org/10.1109/WSC.2015.7408362

Salome, S. (2021). *On the challenge of designing a robust military
force: a multi-resolution modelling approach to improve the performance
of a naval force support system*.
https://repository.tudelft.nl/islandora/object/uuid%3Abaa50bd3-e32a-44ee-9fe4-f9593d3e0829

Seck, M. D., & Honig, H. J. (2012). Multi-perspective modelling of
complex phenomena. *Computational and Mathematical Organization Theory*,
*18*\ (1), 128–144. https://doi.org/10.1007/S10588-012-9119-9/TABLES/2

Vangheluwe, H., de Lara, J., & Mosterman, P. J. (2002). *(PDF) An
introduction to multi-paradigm modelling and simulation*.
https://www.researchgate.net/publication/243776266_An_introduction_to_multi-paradigm_modelling_and_simulation

Xuefei, Y., Qiang, L., Xiaolong, W., Dong, L., & Shoubiao, W. (2017).
*Non-consistence aggregation-disaggregation technology for battle
simulation study of SoS.* https://doi.org/10.18178/wcse.2017.06.066

 

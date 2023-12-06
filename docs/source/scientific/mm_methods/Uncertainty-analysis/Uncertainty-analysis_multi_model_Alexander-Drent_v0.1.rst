==================================================================================
Uncertainty Analysis – Exploratory modeling and analysis (EMA) tool-based coupling
==================================================================================
---------------------------------------
Master thesis summary – Alexander Drent
---------------------------------------


29 November 2023

Introduction 
=============

Large-scale complex systems are increasingly becoming essential
components of an evolving society comprising social and technical or
socio-technical aspects combined with a network of different actors.
These systems are unpredictable, highly uncertain, and evolve
dynamically. To analyze these systems, multi-models need to be developed
with each focusing on a specific part of the (sub)system. Multi-models
allow the investigation of different uncertainty paths across the entire
range of the system. Developing multi-models faces the following
challenges: interoperability, composability, and fidelity. In modeling
socio-technical systems, there are different sources of uncertainties,
such as stochastic variables and processes, a lack of accuracy and
precision, and errors (`Pace, 2015`_). Uncertainties within multi-models
impact the ability to make decisions. Three types of uncertainties are
pointed out: aleatory uncertainty (this uncertainty is impossible to
reduce by measurements), epistemic uncertainty (new measurements can
reduce this uncertainty), and errors (`Pennock & Gaffney, 2018`_).

Uncertainty might propagate when coupling socio-technical models in a
multi-model ecology (`Cuppen et al., 2021`_; `Nikolic et al., 2019`_).
Accordingly, the research question was formulated as ‘To what extent can
we apply existing uncertainty analysis methods to multi-models?’. This
study identified additional sources of uncertainties in multi-model
ecologies compared to constituent single models. Existing methods are
applied to analyze uncertainty propagation in single models. This study
explored a variety of uncertainty analysis tools and methods for
performing sensitivity analyses of single models within a multi-model,
along with the whole multi-model ecology.

State-of-the-art
================

Based on the literature (`Kwakkel et al., 2010`_; `Petersen, 2012; W.E.
Walker P. Harremoës & von Krauss, 2003`_), five locations of uncertainty
have been identified: conceptual model, computer model, including model
structure and parameters, input data, implemented technical model, and
processed output data. The level of uncertainty indicates the degree or
severity of uncertainty. Five levels of uncertainty have been identified
between deterministic knowledge and total ignorance (`Pruyt & Kwakkel,
2014`_). These levels vary in context, system model, system outcomes, and
weights on outcomes (`W.E. Walker P. Harremoës & von Krauss, 2003`_). The
nature of uncertainty concerns whether uncertainty is caused by
variability in the real-world system (ontic) or by the lack of knowledge
(epistemic) (`Kwakkel et al., 2010`_; `Petersen, 2012`_; `van den Hoek et al.,
2014`_; `W.E. Walker P. Harremoës & von Krauss, 2003`_).

Multiple methodologies for uncertainty analyses were studied, and some
were applied. They were categorized into sensitivity analyses,
calibration, and comparison of methods. Two main approaches to
sensitivity analyses were identified: local and global. Sensitivity
analyses are sometimes called independent sampling because they use
model parameters whose values are specified beforehand. The distinction
is made between one-at-a-time (OAT) and all-at-a-time (AAT) sampling.
The benefit of AAT sampling is that interaction effects between input
parameters can be evaluated, which is impossible using OAT sampling.
Three types of AAT sampling are mainly classified: Monte Carlo (MC),
Latin Hypercube Sampling (LHS), and Sobol sequences (`Pianosi et al.,
2016`_). Sensitivity analyses are used for different applications
depending upon the purpose of the analysis: factor prioritization (FP –
identifies parameters that have a significant influence on the output of
the model), factor fixing (FF – identifies the parameters that have a
minimal effect on the variance of the output), variance cutting (VC –
bring the output uncertainty below a determined threshold by fixing the
lowest amount of input values as possible), and factor mapping (FM –
determines which region of the output space is associated with which
part in the input space) (`Saltelli, A., Ratto, M., Andres, T.et al., 2007`_). 
Other sensitivity analysis methods identified in this
study are Morris, RBD-FAST, PAWN, Random Decision Forests, and Patient
Rule Induction Method.

Calibration methods come from an understanding that multiple parameter
sets may result in comparable outcomes and can match calibration data or
a statistical model. This understanding is called equifinality (Beven &
Freer, 2001). Different calibration methods have been suggested in the
literature, such as the Generalized Likelihood Uncertainty Estimation
(GLUE) (`Beven & Binley, 1992`_) and Markov Chain Monte Carlo (MCMC or
MC\ :sup:`2`) (`Vrugt, 2016`_) method.

Two archetypes of multi-model interaction can be considered: directed
graph and undirected graph with feedback mechanisms. The directed graph
has no run-time interaction between separate computer models. The
undirected graph has run-time interaction between the models.

Method, results, and findings 
==============================

A framework is presented to assess uncertainty in used simulation models
and the interface based on the uncertainty matrices proposed in the
literature (`Kwakkel et al., 2010`_; `Petersen, 2012`_; `W.E. Walker P.
Harremoës & von Krauss, 2003`_). This matrix consists of the location of
uncertainty on one axis and the level and nature of uncertainty on the
other axis. XPIROV framework (`Agusdinata, 2006`_) captured the impact of
uncertainty and policies on the model output.

The global method of sensitivity analyses was focused on as local
methods do not adequately explore uncertainty in models with
non-linearities (`Saltelli et al., 2019`_). A matrix was created to compare
the methods mentioned in the previous section for uncertainty analyses.
The methods differ in intended purpose, assumed output distribution,
type of uncertainties, sampling methods, and sample size.

An experimental setup was for multi-models with undirected graphs, which
was applied to a Windmaster model (described below). First, the
uncertainties in the multi-model were assessed using the XPIROV
framework and uncertainty matrix. Then, a selection of methods mentioned
above was applied. Sensitivity analyses were applied with independent
sampling techniques and calibration with dependent sampling. EMA
workbench (`Kwakkel, 2017`_) was used as the multi-model is already
implemented using this workbench. MC sampling technique was chosen
because it allows the possibility of adding samples afterward and
investigating the convergence of feature scores over the increasing
number of used samples.

The Windmaster model is developed to discover robust policies regarding
the investments in the infrastructure and explore uncertainties in the
energy demand and supply of the industrial cluster of the port of
Rotterdam. The multi-model consists of three connected single models
with different modeling paradigms: an exploratory modeling scenario
model, a technical-economical infrastructure model, and an investment
behavior model. The transition pathways developed in EMA were defined as
a series of discrete events affecting peak energy demand, required
feedstock, and energy production or conversion. Uncertainty lies in the
timing of the availability of new technology options and their
implementation lead time.

The policies are included in the model by four defined investment
decision-making strategies of different network operators: reactive,
current, proactive, and collaborative. These are influenced by time
horizon, investment goals, investment budget, the propensity to save,
and lead time per investment.

Feature scores showed that decision-making strategies strongly influence
electricity transmission network capacity and total capital expenditure
costs. Extra-tree features scoring performed per time step, i.e., a
year, showed that decision-making strategies after 2030 and 2020
strongly influenced transmission capacity and capital expenditure,
respectively. The extra trees feature score also showed that
decision-making strategies have high uncertainty scores for the capacity
used of the transmission network. In general, uncertainties have a
strong influence on aspects such as boiler paths (technologies to
produce steam), cogeneration paths (combined production of heat and
electricity), decision-making strategies, and furnace paths (production
of heat). Sobol analysis was used to understand which uncertainties
strongly impact different investment categories. The uncertainties
related to the interface had a limited impact.

Conclusions and future work: 
=============================

The results showed that the EMA workbench can be used for uncertainty
analysis in the multi-model structure. Sobol showed that interaction
effects between uncertainties played a role in the Windmaster model.
Different assets had different influences on the uncertainty, some
significantly more than others, for example, capital investments,
network capacity, or impact of policies. Future research will focus on
using this tool to perform uncertainty analysis of an existing case
study within the multi-modeling project using the tools and methods
described in this research.

A link to Alexander Drent’s master thesis work follows:

https://repository.tudelft.nl/islandora/object/uuid%3Adebfcd39-38fc-493d-8948-012bb8e02f6b

 Bibliography

Agusdinata, D. B. (2006). Specification of System of Systems for
Policymaking in The Energy Sector. *2006 IEEE/SMC International
Conference on System of Systems Engineering*, 197–203.
https://doi.org/10.1109/SYSOSE.2006.1652298

Beven, K., & Binley, A. (1992). The future of distributed models: Model
calibration and uncertainty prediction. *Hydrological Processes*,
*6*\ (3), 279–298.
https://doi.org/https://doi.org/10.1002/hyp.3360060305

Beven, K., & Freer, J. (2001). Equifinality, data assimilation, and
uncertainty estimation in mechanistic modelling of complex environmental
systems using the GLUE methodology. *Journal of Hydrology*, *249*\ (1),
11–29. https://doi.org/10.1016/S0022-1694(01)00421-8

Cuppen, E., Nikolic, I., Kwakkel, J., & Quist, J. (2021). *Participatory
multi-modelling as the creation of a boundary object ecology: the case
of future energy infrastructures in the Rotterdam Port Industrial
Cluster*. *16*, 901–918. https://doi.org/10.1007/s11625-020-00873-z

Kwakkel, J. H. (2017). The Exploratory Modeling Workbench: An open
source toolkit for exploratory modeling, scenario discovery, and
(multi-objective) robust decision making. *Environmental Modelling and
Software*, *96*, 239–250. https://doi.org/10.1016/j.envsoft.2017.06.054

Kwakkel, J. H., Walker, W. E., & Marchau, V. A. W. J. (2010).
Classifying and communicating uncertainties in model-based policy
analysis. *International Journal of Technology, Policy and Management*,
*10*\ (4), 299–315. https://doi.org/10.1504/IJTPM.2010.036918

Nikolic, I., Warnier, M., Kwakkel, J. H., Chappin, E. J. L., Lukszo, Z.,
Brazier, F. M., Verbraeck, A., Cvetkovic, M., & Palensky, P. (2019).
Principles, challenges and guidelines for a multi-model ecology.
*Citation*.
https://doi.org/10.4233/UUID:1AA3D16C-2ACD-40CE-B6B8-0712FD947840

Pace, D. K. (2015). Fidelity, Resolution, Accuracy, and Uncertainty. In
*Modeling and Simulation in the Systems Engineering Life Cycle*.
http://www.springer.com/series/10128

Pennock, M. J., & Gaffney, C. (2018). Managing Epistemic Uncertainty for
Multimodels of Sociotechnical Systems for Decision Support. *IEEE
Systems Journal*, *12*\ (1), 184–195.
https://doi.org/10.1109/JSYST.2016.2598062

Petersen, A. C. (Arthur C. (2012). *Simulating nature : a philosophical
study of computer-simulation uncertainties and their role in climate
science and policy advice*. https://doi.org/10.1201/b11914

Pianosi, F., Beven, K., Freer, J., Hall, J. W., Rougier, J., Stephenson,
D. B., & Wagener, T. (2016). Sensitivity analysis of environmental
models: A systematic review with practical workflow. *Environmental
Modelling & Software*, *79*, 214–232.
https://doi.org/https://doi.org/10.1016/j.envsoft.2016.02.008

Pruyt, E., & Kwakkel, J. H. (2014). Radicalization under deep
uncertainty: a multi-model exploration of activism, extremism, and
terrorism. *System Dynamics Review*, *30*\ (1–2), 1–28.
https://doi.org/https://doi.org/10.1002/sdr.1510

Saltelli, A., Aleksankina, K., Becker, W., Fennell, P., Ferretti, F.,
Holst, N., Li, S., & Wu, Q. (2019). Why so many published sensitivity
analyses are false: A systematic review of sensitivity analysis
practices. *Environmental Modelling & Software*, *114*, 29–39.
https://doi.org/https://doi.org/10.1016/j.envsoft.2019.01.012

Saltelli, A., Ratto, M., Andres, T., Campolongo, F., Cariboni, J., Gatelli, 
D., Saisana, M. and Tarantola, S. (2007). Sensitivity Analysis: From Theory to Practice. 
In Global Sensitivity Analysis. The Primer (eds A. Saltelli, M. Ratto, T. Andres, 
F. Campolongo, J. Cariboni, D. Gatelli, M. Saisana and S. Tarantola). 
https://doi.org/10.1002/9780470725184.ch6

van den Hoek, R. E., Brugnach, M., Mulder, J. P. M., & Hoekstra, A. Y.
(2014). Analysing the cascades of uncertainty in flood defence projects:
How “not knowing enough” is related to “knowing differently.” *Global
Environmental Change*, *24*, 373–388.
https://doi.org/https://doi.org/10.1016/j.gloenvcha.2013.11.008

Vrugt, J. A. (2016). Markov chain Monte Carlo simulation using the DREAM
software package: Theory, concepts, and MATLAB implementation.
*Environmental Modelling & Software*, *75*, 273–316.
https://doi.org/https://doi.org/10.1016/j.envsoft.2015.08.013

W.E. Walker P. Harremoës, J. R. J. P. van der S. M. B. A. van A. P. J.,
& von Krauss, M. P. K. (2003). Defining Uncertainty: A Conceptual Basis
for Uncertainty Management in Model-Based Decision Support. *Integrated
Assessment*, *4*\ (1), 5–17. https://doi.org/10.1076/iaij.4.1.5.16466

 

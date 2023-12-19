=====
ESSIM
=====


ESSIM is an energy system model simulating energy balances over time and
across scales. Refer to
https://multimodelling.readthedocs.io/en/latest/energy_models/ESSIM/index.html
for more overall information regarding the model.

General model information
=========================

General model information questions were asked regarding basic
information, model versions, and point of contact for questions. The
ESSIM model is developed and maintained by TNO.

+---------------------------+------------------------------------------+
| Questions to ask          | Answers/Explanation                      |
+===========================+==========================================+
| Model name                | ESSIM                                    |
+---------------------------+------------------------------------------+
| Model owner               | TNO                                      |
+---------------------------+------------------------------------------+
| Model Developer           | TNO                                      |
+---------------------------+------------------------------------------+
| The latest model          |                                          |
| version/date              |                                          |
+---------------------------+------------------------------------------+
| The model version used in |                                          |
| this project              |                                          |
+---------------------------+------------------------------------------+
| Organization              | TNO                                      |
+---------------------------+------------------------------------------+
| Individual                |                                          |
+---------------------------+------------------------------------------+

A second set of questions was asked regarding whether the model is type
or token, the intended purpose of the model, and the level of decision
that the model aims to support. We understand that the model can be
categorized as a token model as this represents a small part of the
energy system. The model's intended purpose is to simulate network
balancing and its effects in an interconnected hybrid system. Long-term
planning aspects include future scenario investigation or studies. In
the medium term, the model calculates optimal schedule of flexible
producers and the effects of this schedule on emissions, costs, load on
the network, etc.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| Is the model a token       | A small part of the energy system is    |
| model? If so,              | described.                              |
|                            |                                         |
| give illustration(s).      |                                         |
+----------------------------+-----------------------------------------+
| Is the model a type model? |                                         |
| If so,                     |                                         |
|                            |                                         |
| give illustration(s).      |                                         |
+----------------------------+-----------------------------------------+
| Briefly describe the       | 1. Energy balances over time and across |
| intended purpose           | scales.                                 |
|                            |                                         |
| of the model               | 2. Simulates network balancing and the  |
|                            | effects thereof,                        |
|                            |                                         |
|                            | in an interconnected hybrid system.     |
+----------------------------+-----------------------------------------+
| Strategic - long-term      | Future scenario investigation/studies   |
| planning; what             |                                         |
|                            |                                         |
| do we want?                |                                         |
+----------------------------+-----------------------------------------+
| Tactical - medium-term;    | The model calculates optimal schedule   |
| how do we                  | of flexible                             |
|                            |                                         |
| approach this?             | producers and the effects of this       |
|                            | schedule on                             |
|                            |                                         |
|                            | emissions, costs, load on the network,  |
|                            | etc.                                    |
+----------------------------+-----------------------------------------+
| Operational - short-term;  |                                         |
| regular/                   |                                         |
|                            |                                         |
| day-to-day operations?     |                                         |
+----------------------------+-----------------------------------------+

Typical questions about the model include dimensioning and balance of
any hybrid system over the whole year. Similarly, questions can be asked
about shortage or excess of any particular energy carrier, interactions
between them, effects of adding storage, or emissions from different
producers.

The model can be used to model the behavior of an aggregator (the role
in the energy system, aggregating flex, dealing on markets, etc.). One
of the important limitations of the model is a lack of representation of
full-scale interactions within an energy system. The model has been used
as a model orchestrator between multiple lower-level infrastructure
models.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| What are typical types of  | 1. Is my energy system well-dimensioned |
| questions that             | and in                                  |
|                            |                                         |
| can be asked to the model? | balance during the whole year?          |
| provide                    |                                         |
|                            | 2. During what periods of the year do I |
| examples of such questions | have excess                             |
|                            |                                         |
|                            | or shortage of energy, and for what     |
|                            | energy carrier?                         |
|                            |                                         |
|                            | 3. How do the different energy carriers |
|                            | interact with                           |
|                            |                                         |
|                            | each other?                             |
|                            |                                         |
|                            | 4. What is the load on the transport    |
|                            | infrastructure                          |
|                            |                                         |
|                            | over the year, and how often does       |
|                            | overloading                             |
|                            |                                         |
|                            | happen, and to what extent?             |
|                            |                                         |
|                            | 5. What is the total CO2 emission for   |
|                            | the simulated                           |
|                            |                                         |
|                            | system, and how is CO2 emission         |
|                            | distributed over                        |
|                            |                                         |
|                            | the different producers?                |
|                            |                                         |
|                            | 6. What are the effects of adding       |
|                            | storage?                                |
+----------------------------+-----------------------------------------+
| What are the strengths of  | It can be used to model the behavior of |
| this model?                | an aggregator                           |
|                            |                                         |
| What is unique?            | (the role in the energy system,         |
|                            | aggregating flex, dealing               |
|                            |                                         |
|                            | on markets).                            |
+----------------------------+-----------------------------------------+
| What are the important     | It does not represent full-scale energy |
| limitations of             | system                                  |
|                            |                                         |
| the model?                 | interactions.                           |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | It has been used as a model             |
| model was                  | orchestrator between                    |
|                            |                                         |
| used for its intended      | multiple lower-level infrastructure     |
| purpose                    | models;                                 |
|                            |                                         |
|                            | **Additional comments/remarks**:        |
|                            |                                         |
|                            | 1. ESSIM acts as the connection between |
|                            | the energy                              |
|                            |                                         |
|                            | carrier models (basically responsible   |
|                            | for all ‘conversion                     |
|                            |                                         |
|                            | assets’).                               |
|                            |                                         |
|                            | 2. It orchestrates and simulates the    |
|                            | behavior of the                         |
|                            |                                         |
|                            | conversion.                             |
+----------------------------+-----------------------------------------+
| Cases/examples where the   |                                         |
| model was                  |                                         |
|                            |                                         |
| *not* used for its         |                                         |
| intended purpose; are      |                                         |
|                            |                                         |
| there any examples of      |                                         |
| model abuse or             |                                         |
|                            |                                         |
| misuse?                    |                                         |
+----------------------------+-----------------------------------------+

The next set of questions is related to model documentation,
accessibility, and type. The model documentation is complete and is
available online in English. The Application Programming Interfaces
(APIs) are online. The model is static, deterministic, and discrete.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| Is the model             | Yes                                       |
| documentation            |                                           |
|                          |                                           |
| complete?                |                                           |
+--------------------------+-------------------------------------------+
| Is the documentation     | Yes, online                               |
| accessible?              |                                           |
|                          | *https://essim                            |
| If so, how?              | -documentation.readthedocs.io/en/latest/* |
+--------------------------+-------------------------------------------+
| Is the documentation in  | Yes                                       |
| English?                 |                                           |
+--------------------------+-------------------------------------------+
| Does the model have a    |                                           |
|                          |                                           |
| GUI? If so, how to       |                                           |
| access                   |                                           |
|                          |                                           |
| it?                      |                                           |
+--------------------------+-------------------------------------------+
| Does the model have an   | Yes, APIs are also online.                |
| Application              |                                           |
|                          | *https://essim-documentation.read         |
| Programming Interface    | thedocs.io/en/latest/essim_api/index.html*|
| (API) ? If so,           |                                           |
|                          |                                           |
| how to access it?        |                                           |
+--------------------------+-------------------------------------------+
| Is the model static or   | Static                                    |
| dynamic?                 |                                           |
|                          | **Additional comments/remarks**:          |
|                          |                                           |
|                          | ESSIM simulates a certain period of time  |
|                          | with a specific                           |
|                          |                                           |
|                          | resolution (so a simulation of a year on  |
|                          | an hourly basis).                         |
|                          |                                           |
|                          | Most of the time, the system description  |
|                          | doesn't change                            |
|                          |                                           |
|                          | (the hourly values in the profiles are    |
|                          | the things that                           |
|                          |                                           |
|                          | change).                                  |
+--------------------------+-------------------------------------------+
| Is the model continuous  | discrete                                  |
| or discrete?             |                                           |
+--------------------------+-------------------------------------------+
| Is the model stochastic  | Deterministic                             |
| or                       |                                           |
|                          |                                           |
| deterministic?           |                                           |
+--------------------------+-------------------------------------------+
| Is it an optimization    | No                                        |
| model? If so, what       |                                           |
|                          |                                           |
| type of algorithms it    |                                           |
| uses?                    |                                           |
+--------------------------+-------------------------------------------+

The next set of questions are regarding the modeling paradigm,
implementation environment, and license. The model applies multiple
formalisms, such as graph/network-based, non-linear functions, etc.
Multiple general-purpose programming languages, such as Python, JAVA,
etc., are used. No license is required to run the model; however,
permission is required from the model owner.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| What modeling paradigm   | Graph/network-based, code is              |
| or formalism             | object-oriented, heavily                  |
|                          |                                           |
| does the model use?      | data-driven, assets dynamics are          |
|                          | non-linear functions,                     |
|                          |                                           |
|                          | etc.                                      |
+--------------------------+-------------------------------------------+
| Is it implemented in a   | 1. ESSIM is implemented in JAVA. Some     |
| General                  | extensions are                            |
|                          |                                           |
| purpose programming      | written in Python (KPI modules)           |
| language?                |                                           |
|                          | 2. The internal component uses the NATS   |
|                          | message bus                               |
|                          |                                           |
|                          | interface, other projects use MQTT, and   |
|                          | others use                                |
|                          |                                           |
|                          | Rabbit MQ.                                |
+--------------------------+-------------------------------------------+
| Does it use a            | No                                        |
| modeling/Simulation      |                                           |
|                          |                                           |
| environment/package?     |                                           |
+--------------------------+-------------------------------------------+
| Is it implemented in a   |                                           |
| spreadsheet?             |                                           |
+--------------------------+-------------------------------------------+
| Is any license required  | No license is required.                   |
| to run the               |                                           |
|                          | Permission is required from the model     |
| model?                   | owner, however.                           |
+--------------------------+-------------------------------------------+

Model content
=============

A preliminary set of model content questions were related to energy
system integration and scope. The model represents an integrated energy
system. Though, the user has to define and scope them. Essential
elements and concepts included in the model are energy carriers,
production, conversion, transport, and storage. The model focuses on
flexibility in energy and time for different technology options.

+------------------------------+---------------------------------------+
| Questions to ask             | Answers/Explanation                   |
+==============================+=======================================+
| Does the model represent an  | Yes                                   |
| integrated                   |                                       |
|                              | The user has to define and scope      |
| energy system?               | them, though.                         |
+------------------------------+---------------------------------------+
| What important elements and  | Describes energy carriers, energy     |
| concepts                     | production,                           |
|                              |                                       |
| are included in the model?   | consumption, conversion, transport,   |
|                              | and storage.                          |
+------------------------------+---------------------------------------+
| What elements and concepts   |                                       |
| are                          |                                       |
|                              |                                       |
| currently not included in    |                                       |
| the model,                   |                                       |
|                              |                                       |
| but in your opinion, those   |                                       |
| shall be                     |                                       |
|                              |                                       |
| included?                    |                                       |
+------------------------------+---------------------------------------+
| Specific attention to        | Yes, it focuses on flexibility in     |
| flexibility options:         | energy and time for                   |
|                              |                                       |
| What type of flexibility     | different technology options, for     |
| options are                  | example, gas                          |
|                              |                                       |
| included in the model?       | heaters (energy flexible, time        |
|                              | inflexible), batteries                |
|                              |                                       |
|                              | (energy and time flexible), etc.      |
+------------------------------+---------------------------------------+

The next set of content-related questions included scale and resolution.
There is no specific spatial scale of the model. The model has an annual
temporal scale. The model has no specific spatial resolution. The input
file can have spatial information included. Temporal resolution is an
hour.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What spatial (or            | Not specific                           |
| geospatial) scale does the  |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| What temporal (or time)     | Annual                                 |
| scale does the              |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| Spatial resolution          | Not specific                           |
|                             |                                        |
|                             | **Additional comments/remarks**:       |
|                             |                                        |
|                             | ESSIM can be used to model the energy  |
|                             | system of a                            |
|                             |                                        |
|                             | single house or the world's energy     |
|                             | balance. The ESDL                      |
|                             |                                        |
|                             | that goes into ESSIM contains          |
|                             | geographical information               |
|                             |                                        |
|                             | 99% of the time, but ESSIM doesn’t do  |
|                             | anything with                          |
|                             |                                        |
|                             | this information.                      |
+-----------------------------+----------------------------------------+
| Temporal resolution         | hourly                                 |
+-----------------------------+----------------------------------------+

The next set of questions is related to model assumptions, model inputs,
parameters, and outputs, and data sources related to the model. The
model follows an internal algorithm to determine the order of solving
various commodity networks. The model follows flexibility-based
demand-supply matching algorithm that uses the costs of energy
production as a means to grade the desirability of producers. The model
does not fully enforce energy or mass conservation, which might be
contested by others. The input and output file format is Energy System
Description Language (ESDL). Important model inputs are household demand
and supply, related technology options, energy network infrastructure,
large-scale energy supply options, etc. Important model outputs are
production/consumption time series at each node, total production, total
costs, imports/exports, full-load hours, etc.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What critical assumptions   | 1. The model follows an algorithm to   |
| does the                    | determine the                          |
|                             |                                        |
| model have?                 | order of solving various commodity     |
|                             | networks.                              |
|                             |                                        |
|                             | 2. A flexibility-based demand-supply   |
|                             | matching                               |
|                             |                                        |
|                             | algorithm that uses costs of energy    |
|                             | production                             |
|                             |                                        |
|                             | as a means to grade the desirability   |
|                             | of producers.                          |
|                             |                                        |
|                             | 3. A tree-based transport network      |
|                             | solver that                            |
|                             |                                        |
|                             | calculates the load on various         |
|                             | transport elements                     |
|                             |                                        |
|                             | based on the demand-supply solution    |
|                             | determined                             |
|                             |                                        |
|                             | above.                                 |
+-----------------------------+----------------------------------------+
| Which ones are likely to be | 1. Infrastructure cycles/loops are     |
| contested by                | “randomly” cut                         |
|                             |                                        |
| others? Why?                | to make a directed tree.               |
|                             |                                        |
|                             | 2. Energy conservation is not fully    |
|                             | enforced                               |
|                             |                                        |
|                             | (conversion losses can be ignored or   |
|                             | made                                   |
|                             |                                        |
|                             | explicit)                              |
|                             |                                        |
|                             | 3. Transport losses are not considered |
|                             |                                        |
|                             | 4. Mass conservation is not enforced   |
+-----------------------------+----------------------------------------+
| What is/are the model input | ESDL                                   |
| format(s)?                  |                                        |
+-----------------------------+----------------------------------------+
| What is/are the model       | ESDL                                   |
| output format(s)?           |                                        |
+-----------------------------+----------------------------------------+
| What are the important      | Topological city household demand and  |
| model inputs?               | supply,                                |
|                             |                                        |
|                             | related technology options, energy     |
|                             | network                                |
|                             |                                        |
|                             | infrastructure, large-scale energy     |
|                             | supply options,                        |
|                             |                                        |
|                             | etc.                                   |
+-----------------------------+----------------------------------------+
| What important parameters   | Parameters related to the inputs       |
| does the                    | mentioned above                        |
|                             |                                        |
| model have?                 | **Additional comments/remarks**:       |
|                             |                                        |
|                             | There are no internal parameters in    |
|                             | the model.                             |
|                             |                                        |
|                             | All necessary data is in the input     |
|                             | data files.                            |
+-----------------------------+----------------------------------------+
| What are the important      | 1. Mainly time-series (hourly profiles |
| model outputs?              | for                                    |
|                             |                                        |
|                             | consumption/production) at each node   |
|                             |                                        |
|                             | 2. CO2 output profiles (for each       |
|                             | producer or each                       |
|                             |                                        |
|                             | energy carrier)                        |
|                             |                                        |
|                             | 3. KPI modules (metrics: energy        |
|                             | neutrality, total                      |
|                             |                                        |
|                             | (local) production/consumption, total  |
|                             | import/export,                         |
|                             |                                        |
|                             | full load hours, etc.)                 |
+-----------------------------+----------------------------------------+
| What are the data sources   |                                        |
| used by the                 |                                        |
|                             |                                        |
| model?                      |                                        |
+-----------------------------+----------------------------------------+
| Any data that can be        |                                        |
| shared? If so, what         |                                        |
|                             |                                        |
| and how to access them?     |                                        |
+-----------------------------+----------------------------------------+

Continuing with the model content, there were questions regarding
verification, validation, and test, and uncertainty descriptions. There
is no specific test coverage of the model. Units and data consistency
checks are held manually. The results and inputs are validated by
experts. Over-production and system failure are other method of
validating and verifying.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| Can you comment on the test | There is no specific comment on the    |
| coverage of                 | test coverage                          |
|                             |                                        |
| the model?                  | of the model.                          |
+-----------------------------+----------------------------------------+
| What is being verified,     | 1. Unit and data consistency checks,   |
| validated, or tested        | including                              |
|                             |                                        |
| in the model?               | conversion units - manually            |
|                             |                                        |
|                             | 2. Results consistency                 |
+-----------------------------+----------------------------------------+
| What methods are used for   | 1. Experts validation                  |
| the model                   |                                        |
|                             | 2. Overproduction and system failure   |
| verification, validation,   |                                        |
| and testing, if any?        |                                        |
+-----------------------------+----------------------------------------+
| Can you comment on the      |                                        |
| uncertainty in              |                                        |
|                             |                                        |
| model parameters?           |                                        |
+-----------------------------+----------------------------------------+
| Can you comment on the      |                                        |
| uncertainty in              |                                        |
|                             |                                        |
| model input?                |                                        |
+-----------------------------+----------------------------------------+
| Can you comment on the      |                                        |
| uncertainty in              |                                        |
|                             |                                        |
| the model structure?        |                                        |
+-----------------------------+----------------------------------------+

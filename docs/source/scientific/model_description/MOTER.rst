=====
MOTER
=====


**Somadutta Sahoo, Last update: 14 December 2023**

MOTER is an optimization model for dispatching multi-commodity energy
systems in an interconnected network of multiple energy carriers. Refer
to
https://multimodelling.readthedocs.io/en/latest/energy_models/MOTER/index.html
for more overall information regarding the model.

General model information
=========================

General model information questions were asked regarding basic
information, model versions, and point of contact for questions. The
MOTER model is developed and maintained by DNV.

+---------------------------+------------------------------------------+
| Questions to ask          | Answers/Explanation                      |
+===========================+==========================================+
| Model name                | MOTER (Modeler of Three Energy Regimes)  |
+---------------------------+------------------------------------------+
| Model owner               | DNV                                      |
+---------------------------+------------------------------------------+
| Model Developer           | DNV                                      |
+---------------------------+------------------------------------------+
| The latest model          |                                          |
| version/date              |                                          |
+---------------------------+------------------------------------------+
| The model version used in |                                          |
| this project              |                                          |
+---------------------------+------------------------------------------+
| Organization              | DNV                                      |
+---------------------------+------------------------------------------+
| Individual                | Jan Willem Turkstra                      |
+---------------------------+------------------------------------------+

A second set of questions was asked regarding whether the model is type
or token, the intended purpose of the model, and the level of decision
that the model aims to support. We understand that the model can be
categorized as type and token model. The model focuses on long-term
investment in energy infrastructure and technology options related to
storage and conversions. In the mid-term, the model dispatches assets
(for example, generators and heat pumps) within the physical limitations
of the system at the minimum overall costs. In the short term, the model
balances demand-supply energy and addresses mismatches related to energy
flows.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| Is the model a token       | Yes. For example, the model analyses    |
| model? If so,              | energy infrastructure in                |
|                            |                                         |
| give illustration(s).      | detail, i.e., voltage and current       |
|                            | levels of different electricity         |
|                            |                                         |
|                            | networks, rather than the universal     |
|                            | property of energy flows.               |
+----------------------------+-----------------------------------------+
| Is the model a type model? | Yes. For example, one of the major      |
| If so,                     | components of an                        |
|                            |                                         |
| give illustration(s).      | integrated energy system, i.e., energy  |
|                            | infrastructure, is                      |
|                            |                                         |
|                            | modeled in detail.                      |
+----------------------------+-----------------------------------------+
| Briefly describe the       | A global optimization model for         |
| intended purpose of        | dispatching flexible assets in          |
|                            |                                         |
| the model                  | a multi-commodity energy system         |
+----------------------------+-----------------------------------------+
| Strategic - long-term      | Investment in capacity of energy        |
| planning; what do          | infrastructure and                      |
|                            |                                         |
| we want?                   | technology options related to storage   |
|                            | and conversions.                        |
+----------------------------+-----------------------------------------+
| Tactical - medium-term;    | MOTER dispatches the assets (i.e.,      |
| how do we                  | generators, heat pumps,                 |
|                            |                                         |
| approach this?             | boilers, compressors, gas blending,     |
|                            | storage, etc.) within the               |
|                            |                                         |
|                            | physical limitations of the system at   |
|                            | the minimum overall                     |
|                            |                                         |
|                            | cost. Also included in the dispatch     |
|                            | plan are supply/ demand                 |
|                            |                                         |
|                            | curtailment, intraday load shifting,    |
|                            | transport and storage                   |
|                            |                                         |
|                            | losses, and any limitations on maximal  |
|                            | annual volumes                          |
|                            |                                         |
|                            | (like for biogas)                       |
+----------------------------+-----------------------------------------+
| Operational - short-term;  | Demand-supply energy balances, energy   |
| regular/day-to-day         | flows to address                        |
|                            |                                         |
| operations?                | mismatches, dispatch of flexible        |
|                            | assets, etc.                            |
+----------------------------+-----------------------------------------+

Typical questions asked of the model include future capacities and
energy from different technology options. The model has many strengths,
including the detailed representation of energy infrastructure, for
example, electricity, heat, and gas. One of the critical limitations of
the model is that it has only been used in the context of the DNV Energy
Transition Simulator. The model has been used to provide near real-time
feedback on the techno-economic performance of the investment choices
made by the stakeholders. Refer to the table below for further
discussion on these aspects.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| What are typical types of  | 1. What are the capacity and energy     |
| questions that             | supply from different                   |
|                            |                                         |
| can be asked to the model? | technology options?                     |
| provide                    |                                         |
|                            | 2. What type of system integration can  |
| examples of such questions | be achieved with the                    |
|                            |                                         |
|                            | model?                                  |
|                            |                                         |
|                            | 3. What flexibility options are         |
|                            | included in the analysis? Etc.          |
+----------------------------+-----------------------------------------+
| What are the strengths of  | All energy carriers can be configured   |
| this model?                | within three classes:                   |
|                            |                                         |
| What is unique?            | Electric (HV/ MV voltage ranges),       |
|                            | gaseous (pressure,                      |
|                            |                                         |
|                            | composition ranges), and heat           |
|                            | (temperature ranges).                   |
+----------------------------+-----------------------------------------+
| What are the important     | 1. As a global optimizer, the number of |
| limitations of the         | assets combined                         |
|                            |                                         |
| model?                     | with the time resolution is a limiting  |
|                            | factor                                  |
|                            |                                         |
|                            | 2. Only used in the context of the DNV  |
|                            | Energy Transition                       |
|                            |                                         |
|                            | Simulator                               |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | 1. The primary purpose of the MOTER     |
| model was                  | tool is to provide                      |
|                            |                                         |
| used for its intended      | stakeholders with near real-time        |
| purpose                    | feedback on the techno-                 |
|                            |                                         |
|                            | economic performance of the investment  |
|                            | choices made.                           |
|                            |                                         |
|                            | 2. Users can co-create any future       |
|                            | multi-commodity energy                  |
|                            |                                         |
|                            | system                                  |
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
accessibility, and type. The model documentation is not complete and not
accessible. The graphical user interface (GUI) can be accessed with the
owner’s permission. The model is static, deterministic, and linear
programming (LP)-based.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| Is the model             | No                                        |
| documentation            |                                           |
|                          |                                           |
| complete?                |                                           |
+--------------------------+-------------------------------------------+
| Is the documentation     | Not accessible                            |
| accessible?              |                                           |
|                          |                                           |
| If so, how?              |                                           |
+--------------------------+-------------------------------------------+
| Is the documentation in  | Not available                             |
| English?                 |                                           |
+--------------------------+-------------------------------------------+
| Does the model have a    | No                                        |
|                          |                                           |
| GUI? If so, how to       |                                           |
| access                   |                                           |
|                          |                                           |
| it?                      |                                           |
+--------------------------+-------------------------------------------+
| Does the model have an   | In general, the model does not have an    |
| Application              | API.                                      |
|                          |                                           |
| Programming Interface    |                                           |
| (API) ? If so,           |                                           |
|                          |                                           |
| how to access it?        |                                           |
+--------------------------+-------------------------------------------+
| Is the model static or   | Static                                    |
| dynamic?                 |                                           |
+--------------------------+-------------------------------------------+
| Is the model continuous  | continuous                                |
| or discrete?             |                                           |
+--------------------------+-------------------------------------------+
| Is the model stochastic  | Deterministic                             |
| or                       |                                           |
|                          |                                           |
| deterministic?           |                                           |
+--------------------------+-------------------------------------------+
| Is it an optimization    | Yes, LP                                   |
| model? If so, what       |                                           |
|                          |                                           |
| type of algorithms it    |                                           |
| uses?                    |                                           |
+--------------------------+-------------------------------------------+

The next set of questions are regarding the modeling paradigm,
implementation environment, and license. The model applies multiple
formalisms, such as mathematical equations and logical expressions. The
model is implemented using a modeling package called AIMMS. An AIMMS
license is needed, and the owner can share the model.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| What modeling paradigm   | Mathematical equations, logical           |
| or formalism             | expressions, energy balances,             |
|                          |                                           |
| does the model use?      | math equations, etc.                      |
+--------------------------+-------------------------------------------+
| Is it implemented in a   | No                                        |
| General                  |                                           |
|                          |                                           |
| purpose programming      |                                           |
| language?                |                                           |
+--------------------------+-------------------------------------------+
| Does it use a            | AIMMS                                     |
| modeling/Simulation      |                                           |
|                          |                                           |
| environment/package?     |                                           |
+--------------------------+-------------------------------------------+
| Is it implemented in a   |                                           |
| spreadsheet?             |                                           |
+--------------------------+-------------------------------------------+
| Is any license required  | AIMMS license is needed, except for       |
| to run the               | educational and research                  |
|                          |                                           |
| model?                   | purposes                                  |
+--------------------------+-------------------------------------------+

Model content
=============

A preliminary set of model content questions were related to energy
system integration and scope. The model does not represent an integrated
energy system. Essential elements and concepts included in the model are
production, transport, storage, conversion, and end-use of resources.
Some flexibility options included in the model are combined heat and
power plants and heat pumps.

+------------------------------+---------------------------------------+
| Questions to ask             | Answers/Explanation                   |
+==============================+=======================================+
| Does the model represent an  | No                                    |
| integrated                   |                                       |
|                              |                                       |
| energy system?               |                                       |
+------------------------------+---------------------------------------+
| What important elements and  | 1. Production, transport, storage,    |
| concepts are                 | conversion, and end-                  |
|                              |                                       |
| included in the model?       | use are in scope. Networks may have   |
|                              | ring topologies                       |
|                              |                                       |
|                              | with multiple interconnections        |
|                              |                                       |
|                              | 2. MOTER can be configured to include |
|                              | all classes of                        |
|                              |                                       |
|                              | supply and demand                     |
+------------------------------+---------------------------------------+
| What elements and concepts   |                                       |
| are currently                |                                       |
|                              |                                       |
| not included in the model,   |                                       |
| but in your                  |                                       |
|                              |                                       |
| opinion, those shall be      |                                       |
| included?                    |                                       |
+------------------------------+---------------------------------------+
| Specific attention to        | Some examples of flexibility options  |
| flexibility options:         | are combined heat                     |
|                              |                                       |
| What type of flexibility     | and power plants, heat pumps,         |
| options are included         | storage, gas blending,                |
|                              |                                       |
| in the model?                | and other similar options.            |
+------------------------------+---------------------------------------+

The next set of content-related questions included scale and resolution.
There is no spatial representation. The model has a topological
representation of a fictive world of 'Enerland.' Similarly, there is no
specified time scale. Users can define the topological resolutions of
regions. Temporal resolution is the time slices representing a year,
varying from 16 to 800.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What spatial (or            | There is no spatial representation.    |
| geospatial) scale does the  | The model has a                        |
|                             |                                        |
| model have?                 | topological representation of a        |
|                             | fictive world of 'Enerland.'           |
|                             |                                        |
|                             | The modeling framework can represent   |
|                             | energy systems                         |
|                             |                                        |
|                             | ranging from local to national scale.  |
+-----------------------------+----------------------------------------+
| What temporal (or time)     | There is no specified time scale.      |
| scale does the              | Modelers can determine                 |
|                             |                                        |
| model have?                 | the scale based on                     |
|                             | applications/projects.                 |
+-----------------------------+----------------------------------------+
| Spatial resolution          | Users can define the topological       |
|                             | resolution of regions. No              |
|                             |                                        |
|                             | fixed preexisting category is present  |
|                             | in the model.                          |
+-----------------------------+----------------------------------------+
| Temporal resolution         | A yearly dispatch plan is created with |
|                             | hourly resolution                      |
|                             |                                        |
|                             | using “time slices” (i.e., a limited   |
|                             | number of hours                        |
|                             |                                        |
|                             | (16-800) representing the total 8760   |
|                             | hours of a year).                      |
+-----------------------------+----------------------------------------+

The next set of questions is related to model assumptions, model inputs,
parameters, and outputs, and data sources related to the model. The
model's standard input and output format is MS Access. Some important
model inputs are technology options (supply options) and costs
(annualized investments, fixed, variable, and operation and maintenance
costs). Similarly, some important model outputs are production,
transport, conversion, and storage. Data can be shared with permission
from model owners. Most of the data are from open sources.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What critical assumptions   |                                        |
| does the                    |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| Which ones are likely to be |                                        |
| contested by                |                                        |
|                             |                                        |
| others? Why?                |                                        |
+-----------------------------+----------------------------------------+
| What is/are the model input | MS Access                              |
| format(s)?                  |                                        |
+-----------------------------+----------------------------------------+
| What is/are the model       | MS Access                              |
| output format(s)?           |                                        |
+-----------------------------+----------------------------------------+
| What are the important      | Technology inputs (supply,             |
| model inputs?               | transformation, transport, and         |
|                             |                                        |
|                             | storage options), costs (investments,  |
|                             | fixed, variable, and                   |
|                             |                                        |
|                             | operation and maintenance costs)       |
+-----------------------------+----------------------------------------+
| What important parameters   | technology- and process-related        |
| do the                      | parameters (such as,                   |
|                             |                                        |
| model have?                 | efficiency), demand and supply         |
|                             | profiles, limits and ranges            |
|                             |                                        |
|                             | on output, etc.                        |
+-----------------------------+----------------------------------------+
| What are the important      | 1. The model outputs include an        |
| model outputs?              | envisaged operation                    |
|                             |                                        |
|                             | of the production, transport,          |
|                             | conversion, storage, and               |
|                             |                                        |
|                             | (intelligent) end-use assets on an     |
|                             | hourly basis during a                  |
|                             |                                        |
|                             | year.                                  |
|                             |                                        |
|                             | 2. System KPIs on the renewable share, |
|                             | CO2 emission,                          |
|                             |                                        |
|                             | energy cost levels, and security of    |
|                             | supply                                 |
+-----------------------------+----------------------------------------+
| What are the data sources   |                                        |
| used by the                 |                                        |
|                             |                                        |
| model?                      |                                        |
+-----------------------------+----------------------------------------+
| Any data that can be        | Databases can be accessed with         |
| shared? If so, what         | permission from model                  |
|                             |                                        |
| and how to access them?     | owners.                                |
+-----------------------------+----------------------------------------+

Continuing with the model content, there were questions regarding
verification, validation, and test, and uncertainty descriptions. The
answer to test coverage of the model is that there is no formal testing
possibility within the modeling framework. Verification, validation, and
testing can be done on boundary conditions and input limits/ranges.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| Can you comment on the test | There is not much formal testing       |
| coverage of                 | possibility within the                 |
|                             |                                        |
| the model?                  | modeling framework. Input parameters   |
|                             | can be tested by                       |
|                             |                                        |
|                             | sensitivity analyses, for example.     |
|                             | Non-optimality or model                |
|                             |                                        |
|                             | not converging conditions validate     |
|                             | modeling                               |
|                             |                                        |
|                             | outputs/results.                       |
+-----------------------------+----------------------------------------+
| What is being verified,     | Verification, validation, and testing  |
| validated, or tested        | can be on the                          |
|                             |                                        |
| in the model?               | boundary conditions, inputs,           |
|                             | limits/ranges, etc.                    |
+-----------------------------+----------------------------------------+
| What methods are used for   | 1. Qualitative method: stakeholder and |
| the model                   | expert opinions                        |
|                             |                                        |
| verification, validation,   | and perspectives, literature,          |
| and testing, if any?        | government reports, etc.               |
|                             |                                        |
|                             | 2. Quantitative method: comparison     |
|                             | with other                             |
|                             |                                        |
|                             | contemporary national models, scenario |
|                             | comparisons,                           |
|                             |                                        |
|                             | and result ranges are also indicative  |
|                             | based on the                           |
|                             |                                        |
|                             | experience of modelers, etc.           |
+-----------------------------+----------------------------------------+
| Can you comment on the      | Important model parameters within the  |
| uncertainty in              | model operate                          |
|                             |                                        |
| model parameters?           | within ranges, depending upon          |
|                             | scenarios, to handle                   |
|                             |                                        |
|                             | uncertainty                            |
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

**References**:

Model Description:

-  https://www.dnvgl.com/services/energy-transition-simulator-138088

-  https://etrm.nl/

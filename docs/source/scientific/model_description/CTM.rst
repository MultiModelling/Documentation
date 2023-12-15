===
CTM
===


OPERA is a Dutch-based national energy system model focusing on total
system cost minimization. Refer to
https://multimodelling.readthedocs.io/en/latest/energy_models/CTM/index.html
for more overall information regarding the model.

General model information
=========================

General model information questions were asked regarding basic
information, model versions, and point of contact for questions. The CTM
model is developed and maintained by Kalavasta.

+---------------------------+------------------------------------------+
| Questions to ask          | Answers/Explanation                      |
+===========================+==========================================+
| Model name                | CTM (Carbon Transition Model)            |
+---------------------------+------------------------------------------+
| Model owner               | Kalavasta                                |
+---------------------------+------------------------------------------+
| Model Developer           | Kalavasta                                |
+---------------------------+------------------------------------------+
| The latest model          |                                          |
| version/date              |                                          |
+---------------------------+------------------------------------------+
| The model version used in | 5th April 2022                           |
| this project              |                                          |
+---------------------------+------------------------------------------+
| Organization              | Kalavasta                                |
+---------------------------+------------------------------------------+
| Individual                | Karel Zwetsloot                          |
+---------------------------+------------------------------------------+

A second set of questions was asked regarding whether the model is type
or token, the intended purpose of the model, and the level of decision
that the model aims to support. We understand that the model can be
categorized as a token model as it analyzes the feedstock and energy
balance of the Dutch energy-intensive industries. The model focuses on
large industrial sites and performs bottom-up calculations. The model
considers location-specific demand and supply values under different
future scenario conditions. The long-term strategy is discussions
between industries, grid operators, and the government regarding what
energy infrastructure type would be needed for climate neutrality.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| Is the model a token       | Yes. The model analyzes the feedstock   |
| model? If so,              | and energy balance                      |
|                            |                                         |
| give illustration(s).      | of the energy-intensive Dutch           |
|                            | industries per site. The                |
|                            |                                         |
|                            | starting point is the major energy and  |
|                            | mass consumers in                       |
|                            |                                         |
|                            | the Netherlands.                        |
+----------------------------+-----------------------------------------+
| Is the model a type model? |                                         |
| If so,                     |                                         |
|                            |                                         |
| give illustration(s).      |                                         |
+----------------------------+-----------------------------------------+
| Briefly describe the       | 1. CTM takes large industrial sites and |
| intended purpose of        | does the calculation                    |
|                            |                                         |
| the model                  | bottom-up.                              |
|                            |                                         |
|                            | 2. Material and energy balance for      |
|                            | Dutch energy-intensive                  |
|                            |                                         |
|                            | industry on a per-site basis.           |
|                            |                                         |
|                            | 3. Location-specific demand and supply  |
|                            | values under                            |
|                            |                                         |
|                            | different change scenarios.             |
|                            |                                         |
|                            | 4. It could be used for forecasting     |
|                            | infrastructure needs, but               |
|                            |                                         |
|                            | this is not the primary goal. It can    |
|                            | also be used to explore                 |
|                            |                                         |
|                            | other options given potential           |
|                            | transition goals.                       |
+----------------------------+-----------------------------------------+
| Strategic - long-term      | The long-term strategy of the Dutch     |
| planning; what do          | energy-intensive industry               |
|                            |                                         |
| we want?                   | is included by considering the 2025 –   |
|                            | 2050 time frame. For                    |
|                            |                                         |
|                            | strategic discussion between industry,  |
|                            | industry and grid                       |
|                            |                                         |
|                            | operators, industry and government, and |
|                            | industry and NGOs.                      |
|                            |                                         |
|                            | For example, from the perspective of    |
|                            | TSO/DSOs, what kind                     |
|                            |                                         |
|                            | of energy infrastructure would be       |
|                            | needed depending on                     |
|                            |                                         |
|                            | plans to go carbon neutral? The model   |
|                            | provides a localized,                   |
|                            |                                         |
|                            | location-specific, scenario-building    |
|                            | tool for large energy flows.            |
+----------------------------+-----------------------------------------+
| Tactical - medium-term;    |                                         |
| how do we approach         |                                         |
|                            |                                         |
| this?                      |                                         |
+----------------------------+-----------------------------------------+
| Operational - short-term;  |                                         |
| regular/day-to-day         |                                         |
|                            |                                         |
| operations?                |                                         |
+----------------------------+-----------------------------------------+

One of the model's strengths is the ability to perform energy and mass
balance analyses of specific industrial sites. The model has been used
to create the II3050 infrastructure outlook for the Dutch industry to
provide demand profiles to industrial sites for specific future years,
such as 2025 and 2030, based on pre-existing scenarios.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| What are typical types of  |                                         |
| questions that             |                                         |
|                            |                                         |
| can be asked to the model? |                                         |
| provide                    |                                         |
|                            |                                         |
| examples of such questions |                                         |
+----------------------------+-----------------------------------------+
| What are the strengths of  | Specific analysis of mass and energy    |
| this model?                | balance of industrial                   |
|                            |                                         |
| What is unique?            | sites.                                  |
+----------------------------+-----------------------------------------+
| What are the important     |                                         |
| limitations of the         |                                         |
|                            |                                         |
| model?                     |                                         |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | 1. Used for the II3050 infrastructure   |
| model was                  | outlook for the Dutch                   |
|                            |                                         |
| used for its intended      | industry to provide demand profiles in  |
| purpose                    | industrial sites in                     |
|                            |                                         |
|                            | 2025, 2030, and 2050 based on four      |
|                            | pre-existing scenarios.                 |
|                            |                                         |
|                            | 2. First Application for II3050 edition |
|                            | 2 together with the 14                  |
|                            |                                         |
|                            | largest emitters in the industry, Min.  |
|                            | of Economic Affairs and                 |
|                            |                                         |
|                            | Climate, the Grid Operators, and        |
|                            | VNO-NCW.                                |
|                            |                                         |
|                            | **Additional comments/remarks**:        |
|                            |                                         |
|                            | It could be used for forecasting        |
|                            | infrastructure needs, but this          |
|                            |                                         |
|                            | is not the primary goal. It can also be |
|                            | used to explore other                   |
|                            |                                         |
|                            | options given potential transition      |
|                            | goals.                                  |
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
accessibility, and type. The model documentation is not complete. The
graphical user interface (GUI) is available online. The model is static,
continuous, and deterministic. The model is not an optimization model.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| Is the model             | No                                        |
| documentation            |                                           |
|                          |                                           |
| complete?                |                                           |
+--------------------------+-------------------------------------------+
| Is the documentation     | Some documentation is available online.   |
| accessible?              |                                           |
|                          |                                           |
| If so, how?              |                                           |
+--------------------------+-------------------------------------------+
| Is the documentation in  | Not available                             |
| English?                 |                                           |
+--------------------------+-------------------------------------------+
| Does the model have a    | Yes, online                               |
|                          |                                           |
| GUI? If so, how to       | https://carbontransitionmodel.com/        |
| access                   |                                           |
|                          |                                           |
| it?                      |                                           |
+--------------------------+-------------------------------------------+
| Does the model have an   |                                           |
| Application              |                                           |
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
| Is it an optimization    | No                                        |
| model? If so, what       |                                           |
|                          |                                           |
| type of algorithms it    |                                           |
| uses?                    |                                           |
+--------------------------+-------------------------------------------+

The next set of questions are regarding the modeling paradigm,
implementation environment, and license. The model applies multiple
formalisms, such as one-shot calculations, mass and energy flow-based
calculations, mathematical expressions and equations, and graph or
network-based calculations. The model uses JAVA-based web applications
for online spreadsheets. The model is implemented in Excel spreadsheets.
Therefore, no specific license is required to run the model.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| What modeling paradigm   | 1. One-shot calculation and mass and      |
| or formalism             | energy flow-based                         |
|                          |                                           |
| does the model use?      | calculations                              |
|                          |                                           |
|                          | 2. Mathematical expressions and equations |
|                          |                                           |
|                          | 3. Graph (or network) based.              |
+--------------------------+-------------------------------------------+
| Is it implemented in a   | 1. Python orchestrator and API            |
| General                  | application (connects the                 |
|                          |                                           |
| purpose programming      | frontend and the web access)              |
| language?                |                                           |
|                          | 2. JAVA-based web application for online  |
|                          | spreadsheets                              |
|                          |                                           |
|                          | (Keikai - API) - AWS input/output for the |
|                          | spreadsheet                               |
|                          |                                           |
|                          | model                                     |
|                          |                                           |
|                          | 3. The user interface in HTML and JS      |
|                          | (front end)                               |
|                          |                                           |
|                          | **Additional comments/remarks**:          |
|                          |                                           |
|                          | Operating system: Windows for now, AWS    |
|                          | container, Mac                            |
|                          |                                           |
|                          | soon available                            |
+--------------------------+-------------------------------------------+
| Does it use a            |                                           |
| modeling/Simulation      |                                           |
|                          |                                           |
| environment/package?     |                                           |
+--------------------------+-------------------------------------------+
| Is it implemented in a   | Excel model                               |
| spreadsheet?             |                                           |
+--------------------------+-------------------------------------------+
| Is any license required  | No                                        |
| to run the               |                                           |
|                          |                                           |
| model?                   |                                           |
+--------------------------+-------------------------------------------+

Model content
=============

A preliminary set of model content questions were related to energy
system integration and scope. The model does not represent an integrated
energy system. The model fully covers industries; however, heat
integration is still in development.

Essential elements and concepts the model includes are most energy
carriers used by Dutch industries, such as Electricity, natural gas,
hydrogen, heat, and others (including different types of methane,
biowaste/non-biowaste, biomass, waste, carbon monoxide, etc.). No
specific attention is paid to including flexibility options.

+------------------------------+---------------------------------------+
| Questions to ask             | Answers/Explanation                   |
+==============================+=======================================+
| Does the model represent an  | No                                    |
| integrated                   |                                       |
|                              | **Additional comments/remarks**:      |
| energy system?               |                                       |
|                              | Fully integrated for industries, heat |
|                              | integration is still                  |
|                              |                                       |
|                              | in development                        |
+------------------------------+---------------------------------------+
| What important elements and  | 1. Energy carriers: Electricity,      |
| concepts are                 | natural gas, hydrogen,                |
|                              |                                       |
| included in the model?       | heat, and others (including different |
|                              | types of methane,                     |
|                              |                                       |
|                              | biowaste/non-biowaste, biomass,       |
|                              | waste, carbon                         |
|                              |                                       |
|                              | monoxide, etc.)                       |
|                              |                                       |
|                              | 2. A carbon pricing system is in      |
|                              | place.                                |
|                              |                                       |
|                              | 3. The model considers spatial data   |
|                              | regarding grid                        |
|                              |                                       |
|                              | connections (H2, electricity, CO2,    |
|                              | and gas). Distance                    |
|                              |                                       |
|                              | is considered for heat                |
|                              | transportation.                       |
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
| Specific attention to        | No                                    |
| flexibility options:         |                                       |
|                              |                                       |
| What type of flexibility     |                                       |
| options are included         |                                       |
|                              |                                       |
| in the model?                |                                       |
+------------------------------+---------------------------------------+

The next set of content-related questions included scale and resolution.
The spatial scale of the model is the national level, and the temporal
scale is one future target year, approximately 30 years ahead. The
spatial resolution is industry site or cluster level.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What spatial (or            | National                               |
| geospatial) scale does the  |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| What temporal (or time)     | One target year. Approx. 30 years      |
| scale does the              | ahead. Though the                      |
|                             |                                        |
| model have?                 | year is arbitrary                      |
+-----------------------------+----------------------------------------+
| Spatial resolution          | Industry site level or Industry        |
|                             | cluster level                          |
+-----------------------------+----------------------------------------+
| Temporal resolution         |                                        |
+-----------------------------+----------------------------------------+

The next set of questions is related to model assumptions, model inputs,
parameters, and outputs, and data sources related to the model. One of
the critical assumptions is that material and energy balance need to add
up for every industrial site. Industries emitting <100 kT CO2 are not
included in the analysis. Electricity production is not included, but
facilities having their own power production are included in the
analysis. One may contest the level of detail in describing a site. Some
mass/energy streams might be missed. Some important model inputs are the
costs of energy carriers, investments in technologies, annualized
investment costs, costs of carbon emissions (the carbon pricing system
is in place), and the infrastructure cost at the national level.
Similarly, some important model outputs are emissions, demand, cost,
etc., at the cluster, sector, and national levels.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What critical assumptions   | 1. For every industrial site, a        |
| does the                    | material and energy balance            |
|                             |                                        |
| model have?                 | needs to add up. Sites are networked   |
|                             | together. So, a                        |
|                             |                                        |
|                             | network of mass-balanced elements.     |
|                             |                                        |
|                             | 2. There is a cut-off of the size of   |
|                             | facilities included,                   |
|                             |                                        |
|                             | namely <100kT CO2 is considered too    |
|                             | small. Electricity                     |
|                             |                                        |
|                             | production is usually not included;    |
|                             | some facilities have                   |
|                             |                                        |
|                             | power generation of their own, which   |
|                             | is generally                           |
|                             |                                        |
|                             | included. Project consortium and       |
|                             | expert estimate driven.                |
|                             |                                        |
|                             | To illustrate, some smaller sites than |
|                             | the cutoff are                         |
|                             |                                        |
|                             | included as they are project partners. |
+-----------------------------+----------------------------------------+
| Which ones are likely to be | Base year assumptions for site         |
| contested by                | activity are approximations            |
|                             |                                        |
| others? Why?                | made using the best available data.    |
|                             | 10-15 main activities                  |
|                             |                                        |
|                             | are considered. One may contest        |
|                             | specific data on the                   |
|                             |                                        |
|                             | operation of the elements, not their   |
|                             | presence. The level                    |
|                             |                                        |
|                             | of detail in describing the site can   |
|                             | be contested. In                       |
|                             |                                        |
|                             | addition, some mass/energy streams are |
|                             | missed.                                |
+-----------------------------+----------------------------------------+
| What is/are the model input |                                        |
| format(s)?                  |                                        |
+-----------------------------+----------------------------------------+
| What is/are the model       |                                        |
| output format(s)?           |                                        |
+-----------------------------+----------------------------------------+
| What are the important      | 1. Site setting, national setting,     |
| model inputs?               | economic interaction                   |
|                             |                                        |
|                             | within a pool, and technological       |
|                             | inputs for industries                  |
|                             |                                        |
|                             | 2. Costs of carriers and investments   |
|                             | in technologies,                       |
|                             |                                        |
|                             | annualized investment costs, costs of  |
|                             | carbon emissions                       |
|                             |                                        |
|                             | (carbon pricing system is in place),   |
|                             | infrastructure cost                    |
|                             |                                        |
|                             | (National)                             |
+-----------------------------+----------------------------------------+
| What important parameters   | Technological, energetic, and          |
| does the                    | financial parameters related           |
|                             |                                        |
| model have?                 | to industries                          |
+-----------------------------+----------------------------------------+
| What are the important      | Emissions, demand, cost, etc., at      |
| model outputs?              | cluster, sector, and                   |
|                             |                                        |
|                             | national level                         |
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
is limited testing on verification, validation, and testing within the
model. Mass balance checking could be implemented in Excel. One of the
validation methods is feedback from industrial partners, i.e., the
qualitative method. Similarly, base year data is matched with publicly
available data.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| Can you comment on the test |                                        |
| coverage of                 |                                        |
|                             |                                        |
| the model?                  |                                        |
+-----------------------------+----------------------------------------+
| What is being verified,     | Limited testing                        |
| validated, or tested        |                                        |
|                             | **Additional comments/remarks**:       |
| in the model?               |                                        |
|                             | Mass balance checking could be         |
|                             | implemented in Excel                   |
+-----------------------------+----------------------------------------+
| What methods are used for   | 1. Qualitative method: feedback from   |
| the model                   | industrial partners                    |
|                             |                                        |
| verification, validation,   | 2. Quantitative method: face           |
| and testing, if any?        | validation, i.e., checking with        |
|                             |                                        |
|                             | industrial sites and matching base     |
|                             | year data to public data               |
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

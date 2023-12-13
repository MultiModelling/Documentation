=====
OPERA
=====


OPERA is a Dutch-based national energy system model focusing on total
system cost minimization. Refer to :ref:`OPERA<energy_models/OPERA/index>` for more
overall information regarding the model.

General model information
=========================

General model information questions were asked regarding basic
information, model versions, and point of contact for questions. The
OPERA model is developed and maintained by the TNO-ETS group in
Amsterdam.

+---------------------------+------------------------------------------+
| Questions to ask          | Answers/Explanation                      |
+===========================+==========================================+
| Model name                | OPERA (Options Portfolio for Emission    |
|                           | Reduction Assessment)                    |
+---------------------------+------------------------------------------+
| Model owner               | TNO-ETS                                  |
+---------------------------+------------------------------------------+
| Model Developer           | TNO-ETS                                  |
+---------------------------+------------------------------------------+
| Latest model version/date |                                          |
+---------------------------+------------------------------------------+
| The model version used in | 2022_3                                   |
| this project              |                                          |
+---------------------------+------------------------------------------+
| Organization              | TNO-ETS                                  |
+---------------------------+------------------------------------------+
| Individual                | Joost van Stralen                        |
+---------------------------+------------------------------------------+

A second set of questions was asked regarding whether the model is type
or token, the intended purpose of the model, and the level of decision
that the model aims to support. We understand that the model can be
categorized as type and token model. The model focuses on long-term
decision-making with different policies, targets, and measures. Even
though some policy measures are incorporated, the model does not
emphasize significantly in the mid-term (2025-2045). The model allows
the possibility to focus on the mid-term if needed. Energy balances are
maintained between the demand and supply on a regular basis, i.e.,
short-term.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| Is the model a token       | Yes. For example, the model analyses    |
| model? If so,              | the techno-                             |
|                            |                                         |
| give illustration(s).      | economical aspect of the energy system. |
+----------------------------+-----------------------------------------+
| Is the model a type model? | Yes. For example, the model reflects    |
| If so,                     | universal                               |
|                            |                                         |
| give illustration(s).      | characteristics of network              |
|                            | infrastructure, i.e., energy flows.     |
+----------------------------+-----------------------------------------+
| Briefly describe the       | Total system cost minimization at the   |
| intended purpose of        | national level                          |
|                            |                                         |
| the model                  | (the Netherlands)                       |
+----------------------------+-----------------------------------------+
| Strategic - long-term      | 1. Long-term national and regional      |
| planning; what do          | policy targets related                  |
|                            |                                         |
| we want?                   | to emissions reductions, efficiency,    |
|                            | renewable energy                        |
|                            |                                         |
|                            | | production                            |
|                            | | 2. Long-term targets of, for example, |
|                            |   production for                        |
|                            |                                         |
|                            | industries, including subsectors,       |
|                            | sectoral demands,                       |
|                            |                                         |
|                            | energy infrastructure capacity, if any  |
+----------------------------+-----------------------------------------+
| Tactical - medium-term;    | 1. Not much emphasis in the medium      |
| how do we approach         | term, except in the                     |
|                            |                                         |
| this?                      | dynamic run mode of the model           |
|                            |                                         |
|                            | 2. Model structure allows for the       |
|                            | inclusion of medium-                    |
|                            |                                         |
|                            | term policies. Most of them are already |
|                            | included are already                    |
|                            |                                         |
|                            | in the model.                           |
|                            |                                         |
|                            | 3. Certain input parameters are         |
|                            | adjusted based on                       |
|                            |                                         |
|                            | upcoming policies, for example, energy  |
|                            | labels of offices                       |
+----------------------------+-----------------------------------------+
| Operational - short-term;  | demand-supply energy balances, energy   |
| regular/day-to-day         | flows to address                        |
|                            |                                         |
| operations?                | mismatches, short-term flexibility      |
|                            | options                                 |
+----------------------------+-----------------------------------------+

Typical questions asked of the model include future capacities of
different renewable resources and energy supply options. The model has
many strengths, one of them being replicability. The model can readily
apply to other European national energy system modeling contexts. An
additional remark is that the model can simultaneously analyze
greenhouse gases (GHG), non-energy-related emissions, and air pollutants
at the regional and national levels. One of the critical limitations of
the model is the assumption of perfect foresight. The model has been
used to formulate strategic policy advice for the Dutch government on
energy decarbonization and climate change mitigation. Refer to the table
below for further discussion on these aspects.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| What are typical types of  | 1. What are different renewable         |
| questions that             | sources' future capacities and          |
|                            |                                         |
| can be asked to the model? | energy supplies                         |
| provide                    |                                         |
|                            | 2. What is the energy flow between      |
| examples of such questions | regions, and is the                     |
|                            |                                         |
|                            | network constrained to achieve that?    |
|                            | Etc.                                    |
+----------------------------+-----------------------------------------+
| What are the strengths of  | 1. Replicability: the structure can be  |
| this model?                | readily applied to other                |
|                            |                                         |
| What is unique?            | countries, particularly in Europe       |
|                            |                                         |
|                            | 2. System integration - an ideal tool   |
|                            | for assessing the                       |
|                            |                                         |
|                            | implementation of the energy transition |
|                            | and the                                 |
|                            |                                         |
|                            | establishment of a low-carbon economy   |
|                            |                                         |
|                            | 3. Linkage to the NEOMS model - this    |
|                            | model uses data from                    |
|                            |                                         |
|                            | the NEOMS model, which is used for      |
|                            | preparing the annual                    |
|                            |                                         |
|                            | Dutch national energy outlook.          |
|                            |                                         |
|                            | **Additional comments/remarks**:        |
|                            |                                         |
|                            | 1. The model analyzes greenhouse gases  |
|                            | (GHG), non-energy-                      |
|                            |                                         |
|                            | related emissions, and air pollutants.  |
|                            |                                         |
|                            | 2. The capacity limits (of at least     |
|                            | essential technology options            |
|                            |                                         |
|                            | or processes) are set by expert         |
|                            | consultation.                           |
+----------------------------+-----------------------------------------+
| What are the important     | 1. perfect foresight assumption         |
| limitations of the         |                                         |
|                            | 2. Social interaction and impacts       |
| model?                     | missing                                 |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | 1. Used for formulating strategic       |
| model was                  | policy advice on energy                 |
|                            |                                         |
| used for its intended      | decarbonization and climate change      |
| purpose                    | mitigation for the Dutch                |
|                            |                                         |
|                            | government                              |
|                            |                                         |
|                            | 2. Performed exploratory studies on the |
|                            | role of specific low-                   |
|                            |                                         |
|                            | carbon energy technologies in the       |
|                            | energy transition of the                |
|                            |                                         |
|                            | Netherlands                             |
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
accessibility, and type. The model content is documented in a journal
paper that is open source. The graphical user interface (GUI) can be
accessed with the owner’s permission. The model is static,
deterministic, and linear programming (LP)-based.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| Is the model             | Content documentation is a journal paper  |
| documentation            |                                           |
|                          | (see reference below). There is no public |
| complete?                | documentation on                          |
|                          |                                           |
|                          | the details of the model (for example,    |
|                          | GUI, API, etc.). In                       |
|                          |                                           |
|                          | addition, not every update is documented. |
+--------------------------+-------------------------------------------+
| Is the documentation     | The journal paper is open source.         |
| accessible?              |                                           |
|                          |                                           |
| If so, how?              |                                           |
+--------------------------+-------------------------------------------+
| Is the documentation in  | Yes                                       |
| English?                 |                                           |
+--------------------------+-------------------------------------------+
| Does the model have a    | Yes, the GUI can be accessed with the     |
|                          | whole model with                          |
| GUI? If so, how to       |                                           |
| access                   | the owner's permission.                   |
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
|                          | **Additional comments/remarks**:          |
|                          |                                           |
|                          | OPERA can consider 5/10-year time steps,  |
|                          | projecting till 2050,                     |
|                          |                                           |
|                          | i.e., years are optimized individually.   |
|                          | Previous year-cycle data                  |
|                          |                                           |
|                          | are not automatically fed to future       |
|                          | years. Dynamic modeling is                |
|                          |                                           |
|                          | in progress and will not be a part of     |
|                          | this project.                             |
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
|                          | **Additional comments/remarks**:          |
| type of algorithms it    |                                           |
| uses?                    | Due to linear structure, discrete values  |
|                          | (say, integers) are                       |
|                          |                                           |
|                          | not considered. However, limits (lower    |
|                          | and upper) can be set                     |
|                          |                                           |
|                          | as discrete values.                       |
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
system integration and scope. The model represents an integrated energy
system. Essential elements and concepts the model includes are all
greenhouse gas emissions in the Netherlands. Similarly, content-wise,
the model contains important energy infrastructure, such as electricity,
heat, and hydrogen. Some flexibility options included in the model are
salt caverns (spatially dependent), batteries, or hydrogen (spatially
independent).

+------------------------------+---------------------------------------+
| Questions to ask             | Answers/Explanation                   |
+==============================+=======================================+
| Does the model represent an  | Yes                                   |
| integrated                   |                                       |
|                              |                                       |
| energy system?               |                                       |
+------------------------------+---------------------------------------+
| What important elements and  | 1. Covers the entire energy system    |
| concepts are included in the | and all greenhouse gas emissions of   |
| model?                       | the Netherlands                       |
|                              |                                       |
|                              | 2. Content-wise coverage:             |
|                              | Energy-demanding sectors (built       |
|                              | environment, industries, agriculture, |
|                              | and mobility), energy supply options  |
|                              | (for example, wind, solar, biomass,   |
|                              | geothermal, and non-renewable         |
|                              | sources), and energy infrastructure   |
|                              | (electricity, heat, gas, hydrogen,    |
|                              | and CO2)                              |
+------------------------------+---------------------------------------+
| What elements and concepts   |                                       |
| are currently not included   |                                       |
| in the model, but in your    |                                       |
| opinion, those shall be      |                                       |
| included?                    |                                       |
+------------------------------+---------------------------------------+
| Specific attention to        | A few examples of flexibility options |
| flexibility options: What    | are salt caverns (space-specific),    |
| type of flexibility options  | batteries, hydrogen storage, and a    |
| are included in the model?   | significant range of conversion       |
|                              | techniques.                           |
|                              |                                       |
|                              | **Additional comments/remarks**:      |
|                              |                                       |
|                              | Storage, in general, has zero costs.  |
|                              | Only electricity and hydrogen have    |
|                              | storage costs.                        |
+------------------------------+---------------------------------------+

The next set of content-related questions included scale and resolution.
The spatial scale of the model is the national level, and the temporal
scale is long-term (till 2050). The spatial resolution is at the city or
municipality level, which has only been done for Groningen province in
the northern Netherlands. Temporal resolution is time slices, with a
maximum possible 80 slices for a year.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What spatial (or            | National                               |
| geospatial) scale does the  |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| What temporal (or time)     | Long-term (till 2050)                  |
| scale does the              |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| Spatial resolution          | town/city                              |
|                             |                                        |
|                             | **Additional comments/remarks**:       |
|                             |                                        |
|                             | This has been done only for Groningen  |
|                             | Province. The                          |
|                             |                                        |
|                             | structure allows us to perform similar |
|                             | analyses in other                      |
|                             |                                        |
|                             | regions within the Netherlands.        |
+-----------------------------+----------------------------------------+
| Temporal resolution         | Time slices                            |
|                             |                                        |
|                             | Currently, the maximum possible is 80  |
|                             | slices/year.                           |
+-----------------------------+----------------------------------------+

The next set of questions is related to model assumptions, model inputs,
parameters, and outputs, and data sources related to the model. One of
the critical assumptions is the state in which the energy infrastructure
is considered in the model. For some, the current state is the base; for
others, every investment starts from 0. The model standard input is MS
Access, and the output format is MS Excel. Some important model inputs
are Technology inputs (supply options), costs (annualized investments,
fixed, variable, and operation and maintenance costs), and industrial
processes. Similarly, some important model outputs are primary energy
supply, secondary energy demand-supply balances, energy flows, and
system costs. Data can be shared with permission from model owners. Most
of the data are from open sources.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What critical assumptions   | 1. For some infrastructure, the        |
| does the                    | current state of investment            |
|                             |                                        |
| model have?                 | is the base (or lower limit), for      |
|                             | example, high voltage                  |
|                             |                                        |
|                             | electricity network, for others, all   |
|                             | the investments start                  |
|                             |                                        |
|                             | from the scratch, for instance, medium |
|                             | voltage electricity                    |
|                             |                                        |
|                             | network                                |
|                             |                                        |
|                             | 2. Cost or capacity ranges are         |
|                             | primarily based on literature or       |
|                             |                                        |
|                             | expert suggestions.                    |
+-----------------------------+----------------------------------------+
| Which ones are likely to be | 1. Price includes material costs and   |
| contested by                | does not include social                |
|                             |                                        |
| others? Why?                | or environmental costs                 |
|                             |                                        |
|                             | 2. Every stakeholder has complete      |
|                             | knowledge of the market                |
|                             |                                        |
|                             | Behavior. Only the system operator     |
|                             | perspective is                         |
|                             |                                        |
|                             | considered.                            |
+-----------------------------+----------------------------------------+
| What is/are the model input | MS Access                              |
| format(s)?                  |                                        |
|                             | **Additional comments/remarks**:       |
|                             |                                        |
|                             | There is a preprocessing of inputs     |
|                             | within OPERA so that                   |
|                             |                                        |
|                             | to reduce the number of activities     |
|                             | (solving variables) that               |
|                             |                                        |
|                             | goes into the optimization process     |
+-----------------------------+----------------------------------------+
| What is/are the model       | MS Excel                               |
| output format(s)?           |                                        |
|                             | **Additional comments/remarks**:       |
|                             |                                        |
|                             | There is postprocessing of outputs     |
|                             | both in OPERA and in                   |
|                             |                                        |
|                             | Excel.                                 |
+-----------------------------+----------------------------------------+
| What are the important      | Technology inputs (supply options),    |
| model inputs?               | costs (annualized                      |
|                             |                                        |
|                             | investments, fixed, variable, and      |
|                             | operation and                          |
|                             |                                        |
|                             | maintenance costs), industrial         |
|                             | processes, emissions from              |
|                             |                                        |
|                             | industries and other activities,       |
|                             | future targets (for example,           |
|                             |                                        |
|                             | renewable energy production, emission  |
|                             | reduction, and                         |
|                             |                                        |
|                             | efficiency improvement)                |
+-----------------------------+----------------------------------------+
| What important parameters   | technology- and process-related        |
| do the                      | parameters (such as,                   |
|                             |                                        |
| model have?                 | efficiency), demand and supply         |
|                             | profiles, limits and ranges            |
|                             |                                        |
|                             | on output, demand service units (for   |
|                             | example, MT_steel)                     |
+-----------------------------+----------------------------------------+
| What are the important      | primary energy supply, secondary       |
| model outputs?              | energy demand-supply                   |
|                             |                                        |
|                             | balances, energy flows, system costs   |
+-----------------------------+----------------------------------------+
| What are the data sources   | Open sources, such as CBS, are mostly  |
| used by the                 | linked to other models                 |
|                             |                                        |
| model?                      | for specific inputs, etc.              |
+-----------------------------+----------------------------------------+
| Any data that can be        | Databases (MS access format) can be    |
| shared? If so, what         | accessed with                          |
|                             |                                        |
| and how to access them?     | permission from model owners.          |
|                             | Databases contain most                 |
|                             |                                        |
|                             | input-related data. The remaining data |
|                             | can be accessed by                     |
|                             |                                        |
|                             | accessing the model with permission    |
|                             | from the model                         |
|                             |                                        |
|                             | owners.                                |
+-----------------------------+----------------------------------------+

Continuing with the model content, there were questions regarding
verification, validation, and test, and uncertainty descriptions. The
answer to test coverage of the model is that there is no formal testing
possibility within the modeling framework. Verification, validation, and
testing can be done on boundary conditions and input limits/ranges,
generally done by sensitivity analyses, expert opinions, and comparisons
with other models. Inputs related to the long term are more uncertain
compared to the mid-term.

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
|                             | Non-optimality or model not converging |
|                             | conditions validate modeling           |
|                             | outputs/results.                       |
+-----------------------------+----------------------------------------+
| What is being verified,     | Verification, validation, and testing  |
| validated, or tested        | can be on the boundary                 |
|                             |                                        |
| in the model?               | conditions, inputs, limits/ranges,     |
|                             | etc.                                   |
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
|                             | comparisons, etc.                      |
+-----------------------------+----------------------------------------+
| Can you comment on the      | Important model parameters within the  |
| uncertainty in              | model operate                          |
|                             |                                        |
| model parameters?           | within ranges, depending upon          |
|                             | scenarios, to handle                   |
|                             |                                        |
|                             | uncertainty                            |
+-----------------------------+----------------------------------------+
| Can you comment on the      | Input is more uncertain for long-term  |
| uncertainty in              | scenarios compared                     |
|                             |                                        |
| model input?                | to the mid-term.                       |
+-----------------------------+----------------------------------------+
| Can you comment on the      |                                        |
| uncertainty in              |                                        |
|                             |                                        |
| the model structure?        |                                        |
+-----------------------------+----------------------------------------+

**References**:

Model Description:

-  https://doi.org/10.1007/s10666-020-09741-7

Model application:

-  https://doi.org/10.1016/j.apenergy.2021.118035

-  https://doi.org/10.1016/j.apenergy.2022.119149

-  

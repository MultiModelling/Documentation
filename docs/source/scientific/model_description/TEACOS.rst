======
TEACOS
======


**Somadutta Sahoo, Last update: 14 December 2023**

TEACOS is a Dutch-based mathematical optimization model focusing on mid-
to long-term investment analysis. Refer to
https://multimodelling.readthedocs.io/en/latest/energy_models/TEACOS/index.html
for more overall information regarding the model.

General model information
=========================

General model information questions were asked regarding basic
information, model versions, and point of contact for questions. The
TEACOS model is developed and maintained by QUOMARE.

+---------------------------+------------------------------------------+
| Questions to ask          | Answers/Explanation                      |
+===========================+==========================================+
| Model name                | TEACOS                                   |
+---------------------------+------------------------------------------+
| Model owner               | QUOMARE                                  |
+---------------------------+------------------------------------------+
| Model Developer           | QUOMARE                                  |
+---------------------------+------------------------------------------+
| The latest model          |                                          |
| version/date              |                                          |
+---------------------------+------------------------------------------+
| The model version used in |                                          |
| this project              |                                          |
+---------------------------+------------------------------------------+
| Organization              | TNO-ETS                                  |
+---------------------------+------------------------------------------+
| Individual                | Gregor Brandt                            |
+---------------------------+------------------------------------------+

A second set of questions was asked regarding whether the model is type
or token, the intended purpose of the model, and the level of decision
that the model aims to support. We understand that the model can be
categorized as type and token model. The model focuses on
techno-economic optimization, which is capable of long-term planning by
considering investment decisions in technology options.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| Is the model a token       | Yes, it captures investment decisions   |
| model? If so,              | related to specific                     |
|                            |                                         |
| give illustration(s).      | innovative technology options, for      |
|                            | example, hydrogen                       |
|                            |                                         |
|                            | electrolyzer.                           |
+----------------------------+-----------------------------------------+
| Is the model a type model? | Yes, it captures the core elements of   |
| If so,                     | an open, targeted                       |
|                            |                                         |
| give illustration(s).      | system.                                 |
+----------------------------+-----------------------------------------+
| Briefly describe the       | Techno-economic optimization            |
| intended purpose of        |                                         |
|                            |                                         |
| the model                  |                                         |
+----------------------------+-----------------------------------------+
| Strategic - long-term      | Investment decisions in technology      |
| planning; what do          | options                                 |
|                            |                                         |
| we want?                   |                                         |
+----------------------------+-----------------------------------------+
| Tactical - medium-term;    |                                         |
| how do we                  |                                         |
|                            |                                         |
| approach this?             |                                         |
+----------------------------+-----------------------------------------+
| Operational - short-term;  | Operational decisions of technology     |
| regular/                   | options                                 |
|                            |                                         |
| day-to-day operations?     |                                         |
+----------------------------+-----------------------------------------+

Typical questions asked of the model include future capacities and
energy supplies for different technology options. One of the significant
strengths of the model is its openness, i.e., user-defined system.
TEACOS finds the best combination of technology options while
considering optimal investment and operational decisions. One of the
critical limitations of the model is the assumption of perfect
foresight. The model has been used to identify the presence/absence of
different

technologies in a targeted energy system analysis. Refer to the table
below for further discussion on these aspects.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| What are typical types of  | 1. What are the capacity and energy     |
| questions that             | supply from different                   |
|                            |                                         |
| can be asked to the model? | technology options?                     |
| provide                    |                                         |
|                            | 2. Whether a given technology option    |
| examples of such questions | will be selected or not?                |
+----------------------------+-----------------------------------------+
| What are the strengths of  | 1. Open, user-defined system            |
| this model?                |                                         |
|                            | 2. TEACOS finds the best combination of |
| What is unique?            | technology options,                     |
|                            |                                         |
|                            | considering optimal investment and      |
|                            | operational decisions.                  |
+----------------------------+-----------------------------------------+
| What are the important     | 1. Perfect foresight assumption         |
| limitations of the         |                                         |
|                            | 2. Social interaction and impacts       |
| model?                     | missing                                 |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | 1. Used for identifying the             |
| model was                  | presence/absence of different           |
|                            |                                         |
| used for its intended      | technologies in a targeted energy       |
| purpose                    | system analysis                         |
|                            |                                         |
|                            | 2. Identifying the capacity of those    |
|                            | technologies and                        |
|                            |                                         |
|                            | investments in them.                    |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | Sometimes, for operational questions.   |
| model was                  | Core applications and                   |
|                            |                                         |
| *not* used for its         | edge cases.                             |
| intended purpose; are      |                                         |
|                            |                                         |
| there any examples of      |                                         |
| model abuse or             |                                         |
|                            |                                         |
| misuse?                    |                                         |
+----------------------------+-----------------------------------------+

The next set of questions is related to model documentation,
accessibility, and type. The model documentation is not complete. The
graphical user interface (GUI) can be accessed with the owner’s
permission. The model is static, deterministic, and linear programming
(LP)-based.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| Is the model             | No                                        |
| documentation            |                                           |
|                          |                                           |
| complete?                |                                           |
+--------------------------+-------------------------------------------+
| Is the documentation     | Some parts of it are accessible through   |
| accessible?              | the DNV-GL website                        |
|                          |                                           |
| If so, how?              | and this project.                         |
+--------------------------+-------------------------------------------+
| Is the documentation in  | Partly English                            |
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
|                          | TEACOS is a multi-period model (i.e.,     |
|                          | time steps). The model                    |
|                          |                                           |
|                          | uses information from the previous time   |
|                          | step. However, this                       |
|                          |                                           |
|                          | is not a prerequisite.                    |
+--------------------------+-------------------------------------------+
| Is the model continuous  | Continuous                                |
| or discrete?             |                                           |
|                          | **Additional comments/remarks**:          |
|                          |                                           |
|                          | The model has discrete system elements,   |
|                          | but flows are                             |
|                          |                                           |
|                          | continuous.                               |
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
energy system. The model's essential elements and concepts include
detailed information on costs/prices, such as investment profiles or
return on investments. Similarly, content-wise, the model contains
important supply-related technology options and their interactions.

+------------------------------+---------------------------------------+
| Questions to ask             | Answers/Explanation                   |
+==============================+=======================================+
| Does the model represent an  | No                                    |
| integrated                   |                                       |
|                              |                                       |
| energy system?               |                                       |
+------------------------------+---------------------------------------+
| What important elements and  | 1. Economics - CAPEX/full NPV,        |
| concepts are                 | investment profiles,                  |
|                              |                                       |
| included in the model?       | return on investment and other        |
|                              | standard economic KPIs                |
|                              |                                       |
|                              | 2. Content-wise coverage:             |
|                              | Supply-related technology             |
|                              |                                       |
|                              | options, their interactions           |
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
| Specific attention to        |                                       |
| flexibility options:         |                                       |
|                              |                                       |
| What type of flexibility     |                                       |
| options are included         |                                       |
|                              |                                       |
| in the model?                |                                       |
+------------------------------+---------------------------------------+

The next set of content-related questions included scale and resolution.
There is no spatial representation but rather a topology and visual
representation on a map for communication. The temporal scale is
long-term (2020 - 2050).

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What spatial (or            | There is no spatial representation but |
| geospatial) scale does the  | rather a topology                      |
|                             |                                        |
| model have?                 | and visual representation on a map for |
|                             | communication.                         |
|                             |                                        |
|                             | **Additional comments/remarks**:       |
|                             |                                        |
|                             | The transport sector could have cost   |
|                             | and distance                           |
|                             |                                        |
|                             | considerations.                        |
+-----------------------------+----------------------------------------+
| What temporal (or time)     | 30-year period (2020 – 2050)           |
| scale does the              |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| Spatial resolution          |                                        |
+-----------------------------+----------------------------------------+
| Temporal resolution         | Time slice of 5 years in a 30-year     |
|                             | investment trajectory.                 |
|                             |                                        |
|                             | Arbitrary applicable time periods,     |
|                             | given a strategic focus, a             |
|                             |                                        |
|                             | month, a quarter, or a year.           |
+-----------------------------+----------------------------------------+

The next set of questions is related to model assumptions, model inputs,
parameters, and outputs, and data sources related to the model. One of
the assumptions likely to be contested by others is that the model
considers the time-slice approach for faster processing speed, which is
problematic for analyzing peak loads for electricity. The model standard
input format is MS Access, and the output format is MS Excel. Some
important model inputs are technology inputs (supply options) and costs
(annualized investments, fixed, variable, and operation and maintenance
costs). Similarly, some important model outputs are secondary energy
demand-supply balances and system costs. Data can be shared with
permission from model owners.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What critical assumptions   |                                        |
| does the                    |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| Which ones are likely to be | The model considers the time-slice     |
| contested by                | approach for faster                    |
|                             |                                        |
| others? Why?                | processing speed. This is problematic  |
|                             | for analyzing peak                     |
|                             |                                        |
|                             | loads for electricity.                 |
+-----------------------------+----------------------------------------+
| What is/are the model input | MS Access                              |
| format(s)?                  |                                        |
+-----------------------------+----------------------------------------+
| What is/are the model       | MS Access                              |
| output format(s)?           |                                        |
+-----------------------------+----------------------------------------+
| What are the important      | Technology inputs (supply options),    |
| model inputs?               | costs (annualized                      |
|                             |                                        |
|                             | investments, fixed, variable, and      |
|                             | operation and                          |
|                             |                                        |
|                             | maintenance costs)                     |
+-----------------------------+----------------------------------------+
| What important parameters   | Technology-related parameters (such as |
| does the                    | efficiency)                            |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| What are the important      | Secondary energy demand-supply         |
| model outputs?              | balances, system costs,                |
|                             |                                        |
|                             | etc.                                   |
+-----------------------------+----------------------------------------+
| What are the data sources   |                                        |
| used by the                 |                                        |
|                             |                                        |
| model?                      |                                        |
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
answer to test coverage of the model is that TEACOS is continuously
developed using internal test sets to reference models. Internal review
before the branch merges into the master branch on GitHub. Verification,
validation, and testing can be done on boundary conditions and input
limits/ranges.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| Can you comment on the test | TEACOS is continuously developed using |
| coverage of                 | internal test sets                     |
|                             |                                        |
| the model?                  | to reference models. Internal review   |
|                             | before branch                          |
|                             |                                        |
|                             | merges into master on GitHub.          |
+-----------------------------+----------------------------------------+
| What is being verified,     | Verification, validation, and testing  |
| validated, or tested        | can be on the                          |
|                             |                                        |
| in the model?               | boundary conditions, inputs,           |
|                             | limits/ranges, etc. Forcing            |
|                             |                                        |
|                             | options to look at extreme edges of    |
|                             | the solution space.                    |
+-----------------------------+----------------------------------------+
| What methods are used for   | 1. Qualitative method: base case       |
| the model                   | review through                         |
|                             |                                        |
| verification, validation,   | consumer, etc.                         |
| and testing, if any?        |                                        |
|                             | 2. Quantitative method: comparison     |
|                             | with reference cases,                  |
|                             |                                        |
|                             | modeling practice, etc.                |
+-----------------------------+----------------------------------------+
| Can you comment on the      | Sensitivity testing, Monte Carlo on    |
| uncertainty in              | parameter values,                      |
|                             |                                        |
| model parameters?           | multivariant Monte Carlo               |
+-----------------------------+----------------------------------------+
| Can you comment on the      | The model is deterministic and,        |
| uncertainty in              | therefore, does not                    |
|                             |                                        |
| model input?                | propagate uncertainty.                 |
+-----------------------------+----------------------------------------+
| Can you comment on the      | No structural uncertainty              |
| uncertainty in              |                                        |
|                             |                                        |
| the model structure?        |                                        |
+-----------------------------+----------------------------------------+

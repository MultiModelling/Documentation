=============
Introduction
=============
---------------------------------------------------------
Somadutta Sahoo, Last update: 11\ :sup:`th` November 2023
---------------------------------------------------------


The model description template was created to compare models under
different categories. For this project, the focus is energy system
models. The intention was to create a platform for model filtering when
determining diverse energy system configuration analyses. The template
provides a standard format for model description, including
capabilities, important assumptions, data requirements, definitions, and
scales.

The template is categorized into the first level, second level,
questions to ask, answers, and additional comments. The first category
was further subdivided into:

-  General model information

-  Model content

Within general information, further subcategories or the second level
are basic information, model versions, type or token model, intended
purpose, level of decision that the model aims to support, questions
that the model can address, strengths, limitations, part usage of the
model, model documentation, model accessibility, model type, model
paradigms/formalisms, model implementation environment, and model
license.

The model content targets the model structure. The categories are energy
system integration, scope, scale, granularity/resolution, model
assumptions, model inputs, parameters and output, data sources,
verification, validation, test, and uncertainty description. The last
category is the reference section.

Questions and the explanation of the question sections were formulated
to ask questions and further explain those questions to different model
owners if needed. The examples of answers section was created to
facilitate model owners in answering some questions. The explanation of
the question and the example of answers sections provided clarity to
model owners in answering questions. Some question explanations are
based on the :ref:`Terminology` document. This allowed for clarity
among model owners regarding interpreting different meanings of the same
terms. The answers section provides answers from the model owners
regarding the questions asked. Some of the answers could be further
explained in the additional comments section. The following paragraphs
describe the model template in detail.

General model information
=========================

To start with general model information, basic questions were asked
about the model name, owner, and developer. Similarly, questions were
asked about the model's latest versions, versions used for this project,
and point of contact for posing any further questions.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Basic information       | Model name                                 |
+			  +--------------------------------------------+
|                         | Model owner                                |
+			  +--------------------------------------------+
|                         | Model Developer                            |
+-------------------------+--------------------------------------------+
| Model version           | Latest model version/date                  |
+			  +--------------------------------------------+
|                         | The model version used in this project     |
+-------------------------+--------------------------------------------+
| Point of contact for    | Organization                               |
| questions               |                                            |
+			  +--------------------------------------------+
|                         | Individual                                 |
+-------------------------+--------------------------------------------+

Within general information regarding the model, questions were asked
regarding whether the model is a token or a type model. Questions on the
modeling's intended purpose and level of decision support were asked.
Some of the questions were further explained in the process of asking
questions. Suitable references, wherever needed, were provided.

+-------------------------+-------------------------------------------------------------+
| Second level            | Questions to ask                                            |
+=========================+=============================================================+
| Type model or token     | Whether the model is a token model? If so,                  |
| model                   | give illustrations                                          |
|                         |                                                             |
|                         | **Explanation of the question**: These                      |
|                         | models capture elements or                                  |
|                         |                                                             |
|                         | individual properties of the system as                      |
|                         | opposed to universal property (ref:                         |
|                         |                                                             |
|                         | https://link.springer.com/article/10.1007/s10270-006-0017-9)|
+			  +-------------------------------------------------------------+
|                         | Is the model a type model? If so, give                      |
|                         | illustrations                                               |
|                         |                                                             |
|                         | **Explanation of the question**: These                      |
|                         | models capture the universal                                |
|                         |                                                             |
|                         | property of the system rather than                          |
|                         | emphasizing a particular property (ref:                     |
|                         |                                            			|
|                         | https://link.springer.com/article/10.1007/s10270-006-0017-9)|
+-------------------------+-------------------------------------------------------------+
| Intended purpose        | Briefly describe the intended purpose of   			|
|                         | the model.                                 			|
+-------------------------+-------------------------------------------------------------+
| The level of decision   | Strategic - long-term planning; what do we want?		|
| that the 		  |								|
|			  |								|
| model aims to  	  |                                      			|
| support                 |                                            			|
+			  +-------------------------------------------------------------+
|                         | Tactical - medium-term; how do we approach 			|
|                         | this?                                      			|
+			  +-------------------------------------------------------------+
|                         | Operational - short-term;                  			|
|                         | regular/day-to-day operations?             			|
+-------------------------+-------------------------------------------------------------+

Continuing with general model information, questions were asked related
to what kind of typical questions can be answered by the model or what
the strengths and limitations of the model are. Similarly, questions
were asked regarding cases/examples where the model was used for the
intended purpose or was not related to the past usage of the model.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Questions to address    | What are typical types of questions that   |
|                         | can be asked to the                        |
|                         |                                            |
|                         | model? Provide examples of such questions. |
|                         |                                            |
|                         | **Explanation of the question**: The       |
|                         | questions may relate to                    |
|                         |                                            |
|                         | categories such as technologies,           |
|                         | techno-economics,                          |
|		          |					       |			
|			  | society, environment     		       |
|                         | (also emission-related), and policies.     |
+-------------------------+--------------------------------------------+
| Strengths               | What are the strengths of this model? What |
|                         | is unique?                                 |
+-------------------------+--------------------------------------------+
| Limitations             | What are the important limitations of the  |
|                         | model?                                     |
+-------------------------+--------------------------------------------+
| Past usage of the model | Cases/examples where the model was used    |
|                         | for its intended purpose                   |
+			  +--------------------------------------------+
|                         | Cases/examples where the model was *not*   |
|                         | used for its intended                      |
|                         |                                            |
|                         | purpose; are there any examples of model   |
|                         | abuse or misuse?                           |
+-------------------------+--------------------------------------------+

Second-level categories of general model information included model
documentation, accessibility, and types. Questions within the model
documentation included whether the model documentation is complete,
whether the documentation is accessible, and whether the documentation
is in English. Model accessibility-related questions included asking the
modeler whether the model has a Graphical User Interface (GUI) and the
possibility to access the same. A similar question was whether the model
has an application programming interface (API) and how one can access
it. To understand the model type, questions were asked whether the model
is static or dynamic, continuous or discrete, stochastic or
deterministic, and optimization-based. To understand the type of
optimization, a question was asked regarding what algorithm the model
uses.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Model documentation     | Is the model documentation complete?       |
+			  +--------------------------------------------+
|                         | Is the documentation accessible? If so,    |
|                         | how?                                       |
+			  +--------------------------------------------+
|                         | Whether the documentation is in English?   |
+-------------------------+--------------------------------------------+
| Model accessibility     | Does the model have a GUI? If so, how to   |
|                         | access it?                                 |
+			  +--------------------------------------------+
|                         | Does the model have an API? If so, how to  |
|                         | access it?                                 |
+-------------------------+--------------------------------------------+
| Model type              | Is the model static or dynamic?            |
+			  +--------------------------------------------+
|                         | Is the model continuous or discrete?       |
+			  +--------------------------------------------+
|                         | Is the model stochastic or deterministic?  |
+			  +--------------------------------------------+
|                         | Is it an optimization model? If so, what   |
|                         | type of algorithms                         |
|                         |                                            |
|                         | does it use?                               |
|                         |                                            |
|                         | **Examples of answers**: linear            |
|                         | programming (LP), mixed integer            |
|                         |                                            |
|                         | (linear) programming (MIP), non-linear     |
|                         | programming (NLP), or                      |
|                         |                                            |
|                         | a combination of some of these             |
+-------------------------+--------------------------------------------+

Continuing with the general model information, the second-level
categorization followed was modeling paradigms/formalisms, model
implementation environment, and model license. A question was asked
regarding what modeling paradigm or formalism the model uses. Examples
of answers included discrete events, system dynamics, agent-based, etc.
Questions related to the model implementation environment included if
the model was implemented in a general-purpose programming language,
such as Python or JAVA, what modeling package the model used, for
example, off-the-shelf packages such as AIMMS or MATLAB, and whether the
model is implemented in a spreadsheet. The model licensing question was
whether any license is required to run the model.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Modeling                | What modeling paradigm or formalism does   |
| paradigms/formalisms    | the model use?                             |
|                         |                                            |
|                         | **Examples of answers**: discrete event,   |
|                         | systems dynamics,                          |
|                         |                                            |
|                         | agent-based, regression, network model,    |
|                         | math equations, etc.                       |
+-------------------------+--------------------------------------------+
| Model implementation    | Is it implemented in a General purpose     |
| environment             | programming language?                      |
|                         |                                            |
|                         | **Examples of answers**: Python, JAVA,     |
|                         | C++, etc.                                  |
+			  +--------------------------------------------+
|                         | Does it use a modeling/Simulation          |
|                         | environment/package?                       |
|                         |                                            |
|                         | **Examples of answers**: off-the-shelf     |
|                         | packages such as AIMMS,                    |
|                         |                                            |
|                         | GAMS, MATLAB; or modeling packages such as |
|                         | Mesa, PyDevs                               |
+			  +--------------------------------------------+
|                         | Is it implemented in a spreadsheet?        |
|                         |                                            |
|                         | **Examples of answers**: excel,            |
|                         | googlesheets, etc.                         |
+-------------------------+--------------------------------------------+
| Model license           | Is any license required for running the    |
|                         | model?                                     |
+-------------------------+--------------------------------------------+

Model content
=============

The next set of questions was related to the model content (first
level). The first set of second-level categories within this are energy
system integration and model scope. The integration question was whether
the model represents an integrated energy system. Scope-related
questions were what important elements and concepts are included in the
model and what are not. To explain these questions further, the
explanation was scope could include energy carriers, infrastructure,
supply options, demanding sectors, etc. Examples of energy carriers
could include heat, electricity, hydrogen, etc. Since flexibility is
gaining attention within the context of energy system modeling, an
explicit scope-related question was asked regarding what flexibility
options were included in the model.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Energy System           | Does the model represent an integrated     |
| Integration             | energy system?                             |
+-------------------------+--------------------------------------------+
| Scope                   | What important elements and concepts are   |
|                         | included in the                            |
|                         |                                            |
|                         | model?                                     |
|                         |                                            |
|                         | **Explanation of the question**: This can  |
|                         | include energy carriers,                   |
|                         |                                            |
|                         | infrastructure, supply options, demanding  |
|                         | sectors, etc.                              |
|                         |                                            |
|                         | **Examples of answers**: heat,             |
|                         | electricity, hydrogen, etc. – for          |
|                         |                                            |
|                         | energy carriers.                           |
+			  +--------------------------------------------+
|                         | What elements and concepts are currently   |
|                         | not included in the                        |
|                         |                                            |
|                         | model, but in your opinion, those shall be |
|                         | included?                                  |
+			  +--------------------------------------------+
|                         | Specific attention to flexibility options: |
|                         | What type of flexibility                   |
|                         |                                            |
|                         | options are included in the model?         |
|                         |                                            |
|                         | **Examples of answers**: seasonal storage, |
|                         | demand response, etc.                      |
+-------------------------+--------------------------------------------+

Continuing with the model content, the next second-level category was
scale and granularity or resolution. Within the scale category,
questions were asked about the model's spatial (or geospatial) and
temporal (or time) categorization. Answers could include neighborhood,
city, province, etc, for spatial scale and a year or multiple years for
temporal scale. Granularity also included spatial and temporal
categorization with similar possible answers.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Scale                   | What spatial (or geospatial) scale does    |
|                         | the model have?                            |
|                         |                                            |
|                         | **Examples of answers**: neighborhood,     |
|                         | district, town/city,                       |
|                         |                                            |
|                         | province, country, continent, global, etc. |
+			  +--------------------------------------------+
|                         | What temporal (or time) scale does the     |
|                         | model have?                                |
|                         |                                            |
|                         | **Examples of answers**: annual, multiple  |
|                         | years, etc.                                |
+-------------------------+--------------------------------------------+
| Granularity/resolution  | Spatial                                    |
|                         |                                            |
|                         | **Explanation of the question**: This can  |
|                         | be further classified into                 |
|                         |                                            |
|                         | structural or information granularity.     |
|                         | Structural granularity                     |
|                         |                                            |
|                         | represents the level of disaggregation     |
|                         | between model elements                     |
|                         |                                            |
|                         | and the relationships between them.        |
|                         | Information granularity                    |
|                         |                                            |
|                         | represents the information content of the  |
|                         | model elements and                         |
|                         |                                            |
|                         | output.                                    |
|                         |                                            |
|                         | **Examples of answers**: individual        |
|                         | buildings, neighborhood,                   |
|                         |                                            |
|                         | district, town/city, province, country     |
+			  +--------------------------------------------+
|                         | Temporal                                   |
|                         |                                            |
|                         | **Examples of answers**: seconds, minutes, |
|                         | hours, annual, 			       |
|			  |					       |
|			  | time slices within a year,                 |
|                         | time slices over a time period, etc.       |
+-------------------------+--------------------------------------------+

Within the model-content context, the next set of second-level
categories are model assumptions; model inputs, parameters, and outputs;
and data sources of the model. Model assumption questions are what
important assumptions the model has and what assumptions are likely to
be contested by others. Questions related to model input, parameters,
and output are: what is/are the model format for input and output, and
what important inputs, parameters, and outputs does the model include?
Data sources-related questions included the model's data sources and
whether any data can be shared.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Model assumptions       | What important assumptions does the model  |
|                         | have?                                      |
+			  +--------------------------------------------+
|                         | Which ones are likely to be contested by   |
|                         | others? Why?                               |
+-------------------------+--------------------------------------------+
| Model input,            | What is/are the model input format(s)?     |
| parameters, and output  |                                            |
+			  +--------------------------------------------+
|                         | What is/are the model output format(s)?    |
+			  +--------------------------------------------+
|                         | What are the important model inputs?       |
+			  +--------------------------------------------+
|                         | What important parameters does the model   |
|                         | have?                                      |
+			  +--------------------------------------------+
|                         | What are the important model outputs?      |
+-------------------------+--------------------------------------------+
| Data sources            | What are the data sources used by the      |
|                         | model?                                     |
+			  +--------------------------------------------+
|                         | Any data that can be shared? If so, what   |
|                         | and how to access                          |
|                         |                                            |
|                         | them?                                      |
+-------------------------+--------------------------------------------+

The next second-level categories within the model content are
verification, validation, and test and uncertainty descriptions. Within
the first category, questions included what the test coverage of the
model is, what is verified, validated, and tested within the model, and
what methods are deployed for model verification, validation, and
testing. Examples of answers related to the test coverage are direct
structure tests, parameter confirmation, structural boundary adequacy,
etc. Examples of testing and validation methods include Monte Carlo
simulations. Questions related to uncertainty descriptions were
simplistic, for example, what could modelers comment on the
uncertainties associated with model parameters, inputs, and structure?
In the end, there is a description and application-related reference of
the model.

+-------------------------+--------------------------------------------+
| Second level            | Questions to ask                           |
+=========================+============================================+
| Verification,           | Can you comment on the test coverage of    |
| validation, and test    | the model?                                 |
|                         |                                            |
|                         | **Explanation of the question**: The test  |
|                         | could be on structure,                     |
|                         |                                            |
|                         | behavior, policy implications, etc.        |
|                         |                                            |
|                         | **Examples of answers**: direct structure  |
|                         | tests, parameter                           |
|                         |                                            |
|                         | confirmation, extreme conditions,          |
|                         | structural boundary adequacy,              |
|                         |                                            |
|                         | unit checks, sensitivity tests,            |
|                         | reproduction/prediction tests, etc.        |
+			  +--------------------------------------------+
|                         | What are being verified, validated, or     |
|                         | tested in the model, if any?               |
|                         |                                            |
|                         | **Explanation of the question**: What type |
|                         | of methods are                             |
|                         |                                            |
|                         | employed? It could be qualitative,         |
|                         | quantitative, etc.                         |
|                         |                                            |
|                         | **Examples of answers**: expert opinion,   |
|                         | contemporary literature                    |
|                         |                                            |
|                         | review, running the same model under       |
|                         | different scenarios, etc.                  |
+			  +--------------------------------------------+
|                         | What methods are used for model            |
|                         | verification, validation, and              |
|                         |                                            |
|                         | testing, if any?                           |
|                         |                                            |
|                         | **Explanation of the question**: Are there |
|                         | any inbuilt tools, such as                 |
|                         |                                            |
|                         | Monte Carlo, or ways to perform            |
|                         | sensitivity analyses on model              |
|                         |                                            |
|                         | inputs?                                    |
+-------------------------+--------------------------------------------+
| Uncertainty             | Can you comment on the uncertainty in      |
| descriptions            | model parameters?                          |
+			  +--------------------------------------------+
|                         | Can you comment on the uncertainty in      |
|                         | model input?                               |
+			  +--------------------------------------------+
|                         | Can you comment on the uncertainty in the  |
|                         | model structure?                           |
+-------------------------+--------------------------------------------+

In the following section, each of the models used in the project is
described in detail.

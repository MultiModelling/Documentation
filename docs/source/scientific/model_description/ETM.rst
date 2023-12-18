===
ETM
===


OPERA is a Dutch-based national energy system model focusing on total
system cost minimization. Refer to
https://multimodelling.readthedocs.io/en/latest/energy_models/ETM/index.html
for more overall information regarding the model.

General model information
=========================

General model information questions were asked regarding basic
information, model versions, and point of contact for questions. The ETM
model is developed and maintained by Quintel.

+---------------------------+------------------------------------------+
| Questions to ask          | Answers/Explanation                      |
+===========================+==========================================+
| Model name                | ETM (Energy Transition Model)            |
+---------------------------+------------------------------------------+
| Model owner               | Quintel                                  |
+---------------------------+------------------------------------------+
| Model Developer           | Quintel                                  |
+---------------------------+------------------------------------------+
| The latest model          |                                          |
| version/date              |                                          |
+---------------------------+------------------------------------------+
| The model version used in | Latest version                           |
| this project              |                                          |
+---------------------------+------------------------------------------+
| Organization              | Quintel                                  |
+---------------------------+------------------------------------------+
| Individual                | Chael Kruip                              |
+---------------------------+------------------------------------------+

A second set of questions was asked regarding whether the model is type
or token, the intended purpose of the model, and the level of decision
that the model aims to support. We understand that the model can be
categorized as type and token model. The model's intended purpose is to
analyze the energy system of the Netherlands. Long-term national policy
targets are emission reductions, efficiency, and renewable energy
production. The medium-term focus is on flexibility analysis and annual
demand requirements under different ‘if’ conditions.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| Is the model a token       | Users/modelers can define specific      |
| model? If so,              | parts of the energy                     |
|                            |                                         |
| give illustration(s).      | system in detail                        |
+----------------------------+-----------------------------------------+
| Is the model a type model? | It is an energy domain-specific model   |
| If so,                     | that can be configured                  |
|                            |                                         |
| give illustration(s).      | to represent a specific target system   |
|                            | (ETM is a framework:                    |
|                            |                                         |
|                            | model structure predefined; can be      |
|                            | initialized for different               |
|                            |                                         |
|                            | energy systems; can be applied to       |
|                            | sub-systems)                            |
+----------------------------+-----------------------------------------+
| Briefly describe the       | Energy System Analysis of the           |
| intended purpose           | Netherlands                             |
|                            |                                         |
| of the model               |                                         |
+----------------------------+-----------------------------------------+
| Strategic - long-term      | 1. Long-term national policy targets    |
| planning; what             | related                                 |
|                            |                                         |
| do we want?                | to emissions reductions, efficiency,    |
|                            | renewable energy                        |
|                            |                                         |
|                            | production                              |
|                            |                                         |
|                            | 2. Long-term targets of, for example,   |
|                            | production for                          |
|                            |                                         |
|                            | industries, including subsectors,       |
|                            | sectoral demands,                       |
|                            |                                         |
|                            | energy infrastructure capacity          |
+----------------------------+-----------------------------------------+
| Tactical - medium-term;    | 1. Flexibility analysis                 |
| how do we                  |                                         |
|                            | 2. Annual demand requirement under      |
| approach this?             | different 'if' conditions               |
+----------------------------+-----------------------------------------+
| Operational - short-term;  |                                         |
| regular/                   |                                         |
|                            |                                         |
| day-to-day operations?     |                                         |
+----------------------------+-----------------------------------------+

Typical questions about the model include future flexibility in a
national energy system or electrification volume needed to replace heat
demand in the built environment. The model is handy for quickly
exploring and quantifying potential future energy systems in detail. The
model is free to use, open-source, and applicable to national and
regional contexts within the EU. One of the major limitations of the
model is the lack of complex interactions between different components
of an integrated energy system. The governments at different levels
within the Netherlands have used the model for regional and national
energy transition analysis. The model has been pushed to achieve a given
political agenda, which is a case of the model not being used for its
intended purpose.

+----------------------------+-----------------------------------------+
| Questions to ask           | Answers/Explanation                     |
+============================+=========================================+
| What are typical types of  | 1. What flexibility is needed?          |
| questions that             |                                         |
|                            | 2. What is the heat demand for          |
| can be asked to the model? | electrifying the built                  |
| provide                    |                                         |
|                            | environment?                            |
| examples of such questions |                                         |
|                            | 3. How many petrol-fueled vehicles need |
|                            | to be replaced                          |
|                            |                                         |
|                            | to reduce mobility emissions by x %?    |
|                            | Etc.                                    |
+----------------------------+-----------------------------------------+
| What are the strengths of  | 1. A handy calculation tool allowing    |
| this model?                | for quick exploration and               |
|                            |                                         |
| What is unique?            | quantification of potential future      |
|                            | energy systems in detail.               |
|                            |                                         |
|                            | 2. The model can perform analysis at    |
|                            | different geographical                  |
|                            |                                         |
|                            | levels with ease.                       |
|                            |                                         |
|                            | 3. The model covers various aspects of  |
|                            | the energy system,                      |
|                            |                                         |
|                            | such as demand, supply, and emissions.  |
|                            |                                         |
|                            | 4. The model is free to use,            |
|                            | open-source, and available for          |
|                            |                                         |
|                            | EU countries, municipalities, and many  |
|                            | other regions.                          |
+----------------------------+-----------------------------------------+
| What are the important     | 1. The model does not consider the      |
| limitations of             | complex interactions                    |
|                            |                                         |
| the model?                 | within the energy system                |
|                            |                                         |
|                            | 2. Social interaction and impacts       |
|                            | missing                                 |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | 1. The governments at different levels  |
| model was                  | within the Netherlands                  |
|                            |                                         |
| used for its intended      | have used the model for regional and    |
| purpose                    | national energy                         |
|                            |                                         |
|                            | transition analysis.                    |
|                            |                                         |
|                            | 2. The model has been applied/used in   |
|                            | collaboration with                      |
|                            |                                         |
|                            | industries and universities to          |
|                            | understand sectoral energy              |
|                            |                                         |
|                            | demands, energy supplies from different |
|                            | technology options,                     |
|                            |                                         |
|                            | and energy balances.                    |
+----------------------------+-----------------------------------------+
| Cases/examples where the   | The model has been pushed to achieve a  |
| model was                  | given political                         |
|                            |                                         |
| *not* used for its         | agenda/goal (the assumptions/input is   |
| intended purpose; are      | an input, which is                      |
|                            |                                         |
| there any examples of      | the user’s responsibility) and          |
| model abuse or             | interpretation of the result.           |
|                            |                                         |
| misuse?                    |                                         |
+----------------------------+-----------------------------------------+

The next set of questions is related to model documentation,
accessibility, and type. The model documentation is not complete but
adequate. The documentation is available online and is in English. The
graphical user interface (GUI) and Application Programming Interface
(API) are online. The model is static, deterministic, and continuous.

+--------------------------+----------------------------------------------------+
| Questions to ask         | Answers/Explanation                       		|
+==========================+====================================================+
| Is the model             | The documentation is not complete but     		|
| documentation            | adequate.                                 		|
|                          |                                           		|
| complete?                |                                           		|
+--------------------------+----------------------------------------------------+
| Is the documentation     | Yes                                       	       	|
| accessible?              |                                           	       	|
|                          | https://docs.energytransitionmodel.com/main/intro/	|
| If so, how?              | 					 		|
+--------------------------+----------------------------------------------------+
| Is the documentation in  | Yes                                       		|
| English?                 |                                           		|
+--------------------------+----------------------------------------------------+
| Does the model have a    | Yes, the GUI is online.                   		|
|                          |                                           		|
| GUI? If so, how to       | https://energytransitionmodel.com/        		|
| access                   |                                           		|
|                          |                                           		|
| it?                      |                                           		|
+--------------------------+----------------------------------------------------+
| Does the model have an   | Yes, APIs are also online.                		|
| Application              |                                           		|
|                          | https://docs.energytransitionmodel.com/api/intro   |
| Programming Interface    |  							|
| (API) ? If so,           |                                           		|
|                          |                                           		|
| how to access it?        |                                           		|
+--------------------------+----------------------------------------------------+
| Is the model static or   | Static                                    		|
| dynamic?                 |                                           		|
|                          | **Additional comments/remarks**:          		|
|                          |                                           		|
|                          | The model has a static start-to-end date  		|
|                          | calculation. Energy                       		|
|                          |                                           		|
|                          | storage and market principles are dynamic 		|
|                          | time steps.                               		|
+--------------------------+----------------------------------------------------+
| Is the model continuous  | continuous                                		|
| or discrete?             |                                           		|
+--------------------------+----------------------------------------------------+
| Is the model stochastic  | Deterministic                             		|
| or                       |                                           		|
|                          |                                           		|
| deterministic?           |                                           		|
+--------------------------+----------------------------------------------------+
| Is it an optimization    | No                                        		|
| model? If so, what       |                                           		|
|                          |                                           		|
| type of algorithms it    |                                           		|
| uses?                    |                                           		|
+--------------------------+----------------------------------------------------+

The next set of questions are regarding the modeling paradigm,
implementation environment, and license. The model applies multiple
formalisms, such as mathematical equations, object-oriented programming,
etc. Multiple general-purpose programming languages, such as Python,
JAVA, SQL, etc., are used. The model is implemented in an Excel
spreadsheet and does not require any license to run.

+--------------------------+-------------------------------------------+
| Questions to ask         | Answers/Explanation                       |
+==========================+===========================================+
| What modeling paradigm   | Mathematical equations (translation of UI |
| or formalism             | input to model                            |
|                          |                                           |
| does the model use?      | input; graph query), procedural (mostly)  |
|                          | and functional                            |
|                          |                                           |
|                          | (some), Object-oriented, etc.             |
+--------------------------+-------------------------------------------+
| Is it implemented in a   | Python, JAVA, Ruby (mostly), SQL          |
| General                  | database, and C++ for                     |
|                          |                                           |
| purpose programming      | optimized/memory-intensive activity       |
| language?                |                                           |
+--------------------------+-------------------------------------------+
| Does it use a            | No                                        |
| modeling/Simulation      |                                           |
|                          |                                           |
| environment/package?     |                                           |
+--------------------------+-------------------------------------------+
| Is it implemented in a   | Excel                                     |
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
system integration and scope. The model represents an integrated energy
system.

Essential elements and concepts included in the model are
energy-demanding sectors, energy-supplying options, energy
infrastructure, and fuel feedstock. The model covers a wide range of
flexibility options, for example, technologies accommodating large
fluctuations in volume such as power-to-gas (P2G) or gas storage and
large sudden fluctuations in capacities such as heat and power plants.

+------------------------------+---------------------------------------+
| Questions to ask             | Answers/Explanation                   |
+==============================+=======================================+
| Does the model represent an  | Yes                                   |
| integrated                   |                                       |
|                              |                                       |
| energy system?               |                                       |
+------------------------------+---------------------------------------+
| What important elements and  | 1. Covers the entire energy system of |
| concepts                     | the Netherlands                       |
|                              |                                       |
| are included in the model?   | 2. Content-wise coverage:             |
|                              | Energy-demanding sectors              |
|                              |                                       |
|                              | (built environment, industries,       |
|                              | agriculture, and mobility),           |
|                              |                                       |
|                              | energy supply options (for example,   |
|                              | wind, solar, biomass,                 |
|                              |                                       |
|                              | geothermal, and non-renewable         |
|                              | sources), energy                      |
|                              |                                       |
|                              | infrastructure (electricity, heat,    |
|                              | gas, hydrogen, and CO2),              |
|                              |                                       |
|                              | and fuel feedstock                    |
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
| Specific attention to        | A wide range of flexibility options   |
| flexibility options:         | are included:                         |
|                              |                                       |
| What type of flexibility     | a. large fluctuations in volume (P2G, |
| options are                  | Import/export or                      |
|                              |                                       |
| included in the model?       | storage of gas/hydrogen, and seasonal |
|                              | storage of heat)                      |
|                              |                                       |
|                              | b. large or sudden fluctuations in    |
|                              | capacity (storage in                  |
|                              |                                       |
|                              | batteries, dispatchable heat and      |
|                              | power plants, and                     |
|                              |                                       |
|                              | demand side response)                 |
|                              |                                       |
|                              | c. Volume and capacity fluctuations   |
|                              | (import/export of                     |
|                              |                                       |
|                              | electricity, P2H, curtailment of      |
|                              | renewable electricity                 |
|                              |                                       |
|                              | production, and large-scale           |
|                              | electricity storage)                  |
+------------------------------+---------------------------------------+

The next set of content-related questions included scale and resolution.
The spatial scale of the model is the national level. The model has a
long-term temporal scale till 2050; however, the emphasis is till 2050.
The spatial resolution is at the city or municipality level. Temporal
resolution is an hour.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| What spatial (or            | National                               |
| geospatial) scale does the  |                                        |
|                             |                                        |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| What temporal (or time)     | Long-term (till 2070)                  |
| scale does the              |                                        |
|                             | However, the emphasis is till 2050.    |
| model have?                 |                                        |
+-----------------------------+----------------------------------------+
| Spatial resolution          | Municipality                           |
+-----------------------------+----------------------------------------+
| Temporal resolution         | hourly                                 |
+-----------------------------+----------------------------------------+

The next set of questions is related to model assumptions, model inputs,
parameters, and outputs, and data sources related to the model. Most
energy balances happen annually, allowing the model to provide quick
results for different scenarios. The model does not differentiate
between different temperature levels, which others might contest as
industries require high-temperature heat, and the built environment uses
low-temperature heat. The input is through sliders at the GUI, and the
output results are graphs visualized through the GUI. Some important
model inputs are sectoral energy and services demand, supply options,
and profiles. Important model outputs are final energy demands and
supplies, investments in technology options, yearly cost of energy
production, etc. Links to some of the data sources have been provided.
Data can be shared, and some links for that are provided.

+-----------------------------+-------------------------------------------------+
| Questions to ask            | Answers/Explanation                    		|
+=============================+=================================================+
| What critical assumptions   | 1. Most energy balances happen         		|
| does the                    | annually, which allows                 		|
|                             |                                        		|
| model have?                 | the model to provide quick results for 		|
|                             | different scenarios                    		|
|                             |                                        		|
|                             | 2. Multiple versions of the II3050     		|
|                             | scenario are considered                		|
|                             |                                        		|
|                             | in the model.                          		|
+-----------------------------+-------------------------------------------------+
| Which ones are likely to be | 1. No differentiation between          		|
| contested by                | temperature levels; only               		|
|                             |                                        		|
| others? Why?                | one type of heat, which is not         		|
|                             | realistic. Industry uses               		|
|                             |                                        		|
|                             | high-temperature heat, and the built   		|
|                             | environment uses                       		|
|                             |                                        		|
|                             | low-temperature heat                   		|
|                             |                                        		|
|                             | 2. In dispatchable power plants, there 		|
|                             | is no ramping                          		|
|                             |                                        		|
|                             | speed                                  		|
+-----------------------------+-------------------------------------------------+
| What is/are the model input | Input is through sliders at the GUI.   		|
| format(s)?                  |                                        		|
+-----------------------------+-------------------------------------------------+
| What is/are the model       | Output results are graphs visualized   		|
| output format(s)?           | at the GUI.                            		|
+-----------------------------+-------------------------------------------------+
| What are the important      | 674 input variables                    		|
| model inputs?               |                                        		|
|                             | Examples: sectoral energy and services 		|
|                             | demand                                 		|
|                             |                                        		|
|                             | (households, buildings,                		|
|                             | transportation, industry,              		|
|                             |                                        		|
|                             | agriculture, etc.), supply             		|
|                             | (electricity, district heating,        		|
|                             |                                        		|
|                             | hydrogen, transport fuels, etc.),      		|
|                             | profiles (demand,                      		|
|                             |                                        		|
|                             | supply, prices, etc.), etc.            		|
+-----------------------------+-------------------------------------------------+
| What important parameters   | Technology- and process-related        		|
| does the                    | parameters (for example,               		|
|                             |                                        		|
| model have?                 | efficiency), emission factors, etc.    		|
+-----------------------------+-------------------------------------------------+
| What are the important      | Final energy demands and supply,       		|
| model outputs?              | investment in                          		|
|                             |                                        		|
|                             | technology options, hourly electricity 		|
|                             | prices, yearly                         		|
|                             |                                        		|
|                             | energy system cost, production, etc.   		|
+-----------------------------+-------------------------------------------------+
| What are the data sources   | Some links to data sources:            		|
| used by the                 |                                        		|
|                             | https://data.energytransitionmodel.com/         |
| model?                      |  						|
|                             | https://github.com/quintel/etsource    		|
+-----------------------------+-------------------------------------------------+
| Any data that can be        | Yes                                    		|
| shared? If so, what         |                                        		|
|                             | https://refman.energytransitionmodel.com/       |
| and how to access them?     |  						|
|                             |                                        		|
|                             | https://github.com/quintel/etdataset-public	|
+-----------------------------+-------------------------------------------------+

Continuing with the model content, there were questions regarding
verification, validation, and test, and uncertainty descriptions. The
model works in a test-driven development environment. Unit testing is
done for low-level functions. Model inputs, model structure, and data
consistency are verified, tested, and validated. The effect of policies
on the inputs is tested. The qualitative method of validating is expert
consultation. One of the quantitative methods deployed by the model is a
comparison with other models and pilot runs. No systematic uncertainty
verification methods exist, though sensitivity analyses are performed on
various input parameters.

+-----------------------------+----------------------------------------+
| Questions to ask            | Answers/Explanation                    |
+=============================+========================================+
| Can you comment on the test | Test-driven development, unit testing  |
| coverage of                 | for low-level                          |
|                             |                                        |
| the model?                  | functions, integration test            |
+-----------------------------+----------------------------------------+
| What is being verified,     | 1. Input, model structure, data        |
| validated, or tested        | consistency, etc..                     |
|                             |                                        |
| in the model?               | 2. The possible effect of policies is  |
|                             | given as input to                      |
|                             |                                        |
|                             | the model                              |
+-----------------------------+----------------------------------------+
| What methods are used for   | 1. Qualitative method: expert          |
| the model                   | validation                             |
|                             |                                        |
| verification, validation,   | 2. Quantitative method: comparison     |
| and testing, if any?        | with other models                      |
|                             |                                        |
|                             | with more significant details, pilot   |
|                             | runs                                   |
|                             |                                        |
|                             | 3. Simulate a user of the model        |
|                             |                                        |
|                             | 4. Incremental, iterative              |
|                             |                                        |
|                             | Etc.                                   |
+-----------------------------+----------------------------------------+
| Can you comment on the      | Sensitivity analyses; no systematic    |
| uncertainty in              | uncertainty                            |
|                             |                                        |
| model parameters?           | verification method                    |
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

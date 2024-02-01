=====================================================
Requirements for the Multi-Model Infrastructure (MMI)
=====================================================

28 November 2023

At the start of the MMviB project, two requirement workshops were
organised with the consortium. The goals were threefold: first, to
generate ideas for desired features of the MMI as a long-term vision;
second, to reach a consensus on the objective of this project within
that vision; and third, to promote trust and enhance understanding among
partners through a collaborative and co-created effort.

To gain a solid understanding of the overarching issues, namely the WHY
(needs) and WHAT (features) of MMI, the following key questions guided
our discussion in the workshops:

-  What kind of use cases do we envisage?

   -  What cannot be done now by individual models, and what is MMI's
      added value?

   -  What kind of decisions to make with the multi-models?

-  What features or services are required in the MMI?

   -  What the MMI will need to connect multi-models?

   -  What kinds of models are to be coupled? What is their operational
      principle (e.g., AMB, optimisation)?

   -  In what manner should the models interoperate?

   -  What information do the models exchange? How often?

We used a five-step brainstorming process (i.e., idea generation,
pruning, grouping, defining features, and prioritisation) to elicit,
organise and summarise the needs and features. They are summarised and
reviewed in five categories and explained in this MMI requirement
document.

 `1. Infrastructure deployment`_
  
 `2. Model description and alignment`_
  
 `3. Model connection and multi-model set-up`_
  
 `4. Model interoperation`_
  
 `5. Model experimentation and output`_

1. Infrastructure deployment
============================

This category addresses the issues to avoid or reduce vendor- or other
types of lock-in.

+-----+---------------------------+-----------+-----------------------+
|     | Features                  | Priority  | Comments related to   |
|     |                           |           | Needs                 |
+=====+===========================+===========+=======================+
| 1.1 | The infrastructure should | Critical  |                       |
|     | be deployable on a single |           |                       |
|     | computer or within an     |           |                       |
|     | organisation.             |           |                       |
+-----+---------------------------+-----------+-----------------------+
| 1.2 | The infrastructure shall  | Critical  |                       |
|     | not depend on a single    |           |                       |
|     | party.                    |           |                       |
+-----+---------------------------+-----------+-----------------------+

2. Model description and alignment
==================================

This category addresses prerequisites for multi-model connection: what
the models need to adhere to and what the MMI need to provide to allow
model participation.

+-----+---------------------------+-----------+-----------------------+
|     | Features                  | Priority  | Comments related to   |
|     |                           |           | Needs                 |
+=====+===========================+===========+=======================+
| 2.1 | Provide a generic format  | Critical  | The model description |
|     | for model description.    |           | shall include, e.g.,  |
|     |                           |           | objectives, data      |
|     |                           |           | requirements, time    |
|     |                           |           | scales, to help       |
|     |                           |           | general understanding |
|     |                           |           | of a model. It shall  |
|     |                           |           | be human readable,    |
|     |                           |           | and ideally also      |
|     |                           |           | machine readable.     |
|     |                           |           | This feature is       |
|     |                           |           | needed to support     |
|     |                           |           | model selection.      |
+-----+---------------------------+-----------+-----------------------+
| 2.2 | Provide a common data     | Critical  | Consistent synthetic  |
|     | model/format for          |           | representation of     |
|     | input/output data         |           | data exchanged in     |
|     |                           |           | multi-models          |
+-----+---------------------------+-----------+-----------------------+
| 2.3 | Allow model connection    | Critical  | Alignment of multiple |
|     | across multiple           |           | levels of model       |
|     | geographic, time and      |           | granularity. Example  |
|     | other scales              |           | of applications:      |
|     |                           |           | evaluation of         |
|     |                           |           | macro-level decisions |
|     |                           |           | on a micro-level;     |
|     |                           |           | couple high-level     |
|     |                           |           | energy scenario       |
|     |                           |           | models to detailed    |
|     |                           |           | dynamic simulation    |
|     |                           |           | models; couple        |
|     |                           |           | economic market       |
|     |                           |           | models to technical   |
|     |                           |           | models.               |
+-----+---------------------------+-----------+-----------------------+
| 2.4 | Provide a common energy   | Important | data sharing,         |
|     | system database/dataset   |           | alignment,            |
|     | for model input and       |           | consistency           |
|     | configuration             |           |                       |
+-----+---------------------------+-----------+-----------------------+
| 2.5 | Explicit description of   | Important | Understanding and     |
|     | model assumptions         |           | potential alignment   |
|     |                           |           | of model assumptions  |
+-----+---------------------------+-----------+-----------------------+
| 2.6 | Queryable model           | Nice to   | Support transparency  |
|     | assumptions               | have      | and understanability  |
|     |                           |           | among other           |
+-----+---------------------------+-----------+-----------------------+
| 2.7 | Allow inclusion of        | Nice to   | Alignment of          |
|     | external ontologies in    | have      | conceptual            |
|     | addition to the standard  |           | representations       |
|     | model description         |           |                       |
|     | provided by MMI           |           |                       |
+-----+---------------------------+-----------+-----------------------+

3. Model connection and multi-model set-up
==========================================

This category addresses how to connect individual models and to set up a
multi-model

+------+----------------------+-----------------+---------------------+
|      | Features             | Priority        | Comments related to |
|      |                      |                 | Needs               |
+======+======================+=================+=====================+
| 3.1  | Provide interfaces   | Critical        | Reusable interfaces |
|      | for model connection |                 | between models,     |
|      | to allow multi-model |                 | that allow for easy |
|      | creation and         |                 | multi-model         |
|      | connection           |                 | creation in future  |
|      |                      |                 | API and/or UI; to   |
|      |                      |                 | easily add and      |
|      |                      |                 | remove models       |
+------+----------------------+-----------------+---------------------+
| 3.2  | The interface shall  | Critical        | Support multiple    |
|      | support different    |                 | "interaction        |
|      | types of model       |                 | schemes" (of        |
|      | interaction          |                 | different types of  |
|      |                      |                 | models, e.g.,       |
|      |                      |                 | agent-based model,  |
|      |                      |                 | excel model,        |
|      |                      |                 | optimization model) |
|      |                      |                 | and to minimize     |
|      |                      |                 | required            |
|      |                      |                 | adaptations to the  |
|      |                      |                 | individual models   |
+------+----------------------+-----------------+---------------------+
| 3.3  | Provide a method to  | Critical        | Statical or         |
|      | configure the models |                 | dynamical           |
|      | that uses the        |                 | configuration of    |
|      | infrastructure       |                 | models              |
+------+----------------------+-----------------+---------------------+
| 3.4  | Provide a method to  | Critical        | Communicate the     |
|      | communicate          |                 | uncertainty of      |
|      | uncertainties and    |                 | model results       |
|      | source thereof       |                 |                     |
|      | (model inputs and    |                 |                     |
|      | outputs)             |                 |                     |
+------+----------------------+-----------------+---------------------+
| 3.5  | Provide a model      | Important       | For model search    |
|      | repository           |                 | and selection       |
|      |                      |                 | capabilities        |
+------+----------------------+-----------------+---------------------+
| 3.6  | Secure and           | Important       | Manage access and   |
|      | authorized           |                 | communication       |
|      | connection and       |                 | rights, possibly    |
|      | communication when   |                 | also for paid use   |
|      | needed               |                 |                     |
+------+----------------------+-----------------+---------------------+
| 3.7  | Identification or    | Important       | Support model       |
|      | flagging of          |                 | selection           |
|      | potential            |                 | capabilities and    |
|      | multi-model          |                 | model               |
|      | interaction problems |                 | interoperation      |
+------+----------------------+-----------------+---------------------+
| 3.8  | Model                | Nice to have    |                     |
|      | repository/catalogue |                 |                     |
|      | with "app store"     |                 |                     |
+------+----------------------+-----------------+---------------------+
| 3.9  | Model discovery and  | Nice to have    | Find the right      |
|      | selection based on   |                 | model(s) that fit   |
|      | requirements         |                 | the purpose         |
+------+----------------------+-----------------+---------------------+
| 3.10 | Dashboard/GUI for    | Nice to have    | Model selection     |
|      | multi-model          |                 | capabilities by     |
|      | selection,           |                 | human               |
|      | connection and       |                 |                     |
|      | configuration        |                 |                     |
+------+----------------------+-----------------+---------------------+


4. Model interoperation
=======================

This category addresses what is needed for model interoperation (i.e. interaction) after a multi-model is set up 

+------+-----------------------+--------------+-----------------------+
|      | Features              | Priority     | Comments related to   |
|      |                       |              | Needs                 |
+======+=======================+==============+=======================+
| 4.1  | Allow for             | Critical     |                       |
|      | human-in-the-loop     |              |                       |
|      | control of model      |              |                       |
|      | interaction           |              |                       |
+------+-----------------------+--------------+-----------------------+
| 4.2  | Allow for             | Critical     |                       |
|      | fully-automated model |              |                       |
|      | interaction           |              |                       |
+------+-----------------------+--------------+-----------------------+
| 4.3  | Standardized          | Critical     | Informing, e.g.,      |
|      | communication         |              | assumptions of one    |
|      | protocol              |              | model with outputs    |
|      |                       |              | from another model    |
+------+-----------------------+--------------+-----------------------+
| 4.4  | Provide an            | Critical     | This includes, e.g.   |
|      | orchestration         |              | start, stop, pause,   |
|      | mechanism that allows |              | continue, reset,      |
|      | for control of models |              | error report and      |
|      |                       |              | handling, have        |
|      |                       |              | keep-alive pings.     |
+------+-----------------------+--------------+-----------------------+
| 4.5  | The orchestration     | Critical     |                       |
|      | mechanism shall be in |              |                       |
|      | a decentralized way   |              |                       |
+------+-----------------------+--------------+-----------------------+
| 4.6  | Provide logging and   | Critical     |                       |
|      | tracing               |              |                       |
+------+-----------------------+--------------+-----------------------+
| 4.7  | Provide debugging     | Critical     |                       |
|      | capabilities          |              |                       |
+------+-----------------------+--------------+-----------------------+
| 4.8  | Provide backward      | Nice to have |                       |
|      | compatible            |              |                       |
|      | communication         |              |                       |
|      | protocol              |              |                       |
+------+-----------------------+--------------+-----------------------+
| 4.9  | Support dynamic       | Nice to have | Fit for real-time     |
|      | real-time model       |              | applications          |
|      | interaction           |              |                       |
+------+-----------------------+--------------+-----------------------+
| 4.10 | Support               | Nice to have | Fit for Digital twin  |
|      | hardware-in-the-loop  |              | applications          |
+------+-----------------------+--------------+-----------------------+

5. Model experimentation and output 
===================================

This category addresses what is needed for model interoperation (i.e.
interaction) after a multi-model is set up

+-----+------------------------+--------------+-----------------------+
|     | Features               | Priority     | Comments related to   |
|     |                        |              | Needs                 |
+=====+========================+==============+=======================+
| 5.1 | Provide experiment     | Critical     | For documenting model |
|     | management             |              | set-up, version,      |
|     |                        |              | scenarios,            |
|     |                        |              | parameters, runs,     |
|     |                        |              | etc.                  |
+-----+------------------------+--------------+-----------------------+
| 5.2 | Provide multi-model    | Critical     | Link result to        |
|     | output result          |              | experimental setups;  |
|     | management             |              | who saved the result  |
|     |                        |              | and where             |
+-----+------------------------+--------------+-----------------------+
| 5.3 | GUI MM output analysis | Nice to have | Output analysis with  |
|     |                        |              | respect to MM         |
|     |                        |              | experimental set-up   |
+-----+------------------------+--------------+-----------------------+
| 5.4 | Provide a set of       | Nice to have | To assist             |
|     | experiment scenarios   |              | experimental set-up;  |
|     | for a given energy     |              | Case study repository |
|     | system configuration   |              |                       |
+-----+------------------------+--------------+-----------------------+


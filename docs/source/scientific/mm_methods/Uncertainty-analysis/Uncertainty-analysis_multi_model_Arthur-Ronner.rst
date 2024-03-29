======================================
Multi-model uncertainty analysis tool
======================================


The multi-model uncertainty analysis tool connects the Orchestrator
(Apache airflow) with the EMA (Exploratory Modeling and Analysis)
workbench. It is proof of concept that such a tool can assist in
uncertainty analyses on multi-models. Figure 1 shows the structure of
the uncertainty analysis tool.

.. image:: images/image1.png
   :width: 6.43125in
   :height: 2.1875in

*Figure 1: Uncertainty analysis tool structure*

A user provides information about the system in a settings file. This
information includes which uncertainties to include in generating
scenarios and which outcomes to consider. This file is then used to
create the scenarios of the EMA workbench, which are subsequently
transferred to the input of the model as ESDL files. With one ESDL file
per scenario, the model is run once for every scenario. The outcomes (as
specified in the settings file) are finally collected from the different
model runs and can be analyzed using the tools from the EMA workbench. A
more detailed explanation of the workflow is provided in the readme
document in the repository.

A mock-up example was created to demonstrate the functionality of the
tool. To this end, the meso use case ESDL file was used, and three input
and output parameters were chosen for test runs. We created a mock-up
model function that generates output data. This resulted in the
following pair plot that shows the variations of input and output in
relation to the different scenario runs.

.. image:: images/image2.png
   :width: 5.65625in
   :height: 5.95486in

*Figure 2: Pair plot based on the PV investment (solar panels investment
costs), total costs of the system, and the total energy production of
the municipality of Tholen. The data in this figure is mock-up data.*

The work could show with the mock-up example that uncertainty analysis
of a multi-model is possible with such a supporting tool that links the
EMA workbench with the Orchestrator. Future work can expand the
functionality of this proof-of-concept tool and integrate the tool with
the multi-model use cases.

-  Link to the tool repository:
   https://github.com/MultiModelling/Multi-Model-Uncertainty-Analysis-tool
   (accessed November 20, 2023).

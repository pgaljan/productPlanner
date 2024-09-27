# About
[Download (github)](https://github.com/pgaljan/structurePlanner/archive/refs/heads/main.zip)


#### Structure Planner is...
- "project quantification in a box" - a simple, powerful, 4-tier project planner with support for up to 12 workstreams 
- appropriate for use with two-pizza planning teams
- designed for early project phase ideation, cost sizing, and visualzation
- capable of handling an arbitrary number of work periods and project timespan
- configurable to handle work periods of days, weeks, quarters, or years
- delivered in a VB and PowerQuery-free excel workbook, with sheets protected (without password) for error-free authoring
- Excel for web compatible and mobile friendly

#### Use Structure Planner for...
- project estimation and quick iteration during the ideation, planning, and contract bid phases
- early identification of "big rocks" in the project plan
- generating "what-if" analyses and business cases unconstrained by existing project management structures
- parallel analysis (red/blue team)
- cross-organizational collaboration efforts with no shared data structures or nomenclatures
- auditing operational project plans produced in enterprise project management (EPM) software
- modeling and simulation of notional project structures for operational implementation in EPM software
- producing predictable and structured otuput for deeper or comparative analysis

#### Structure Planner delivers...
- simple, 5-parameter data entry for resources
- fluid, user-defined task and resource definition with prompts for reduction/deduplication
- key measures and financials summarized and aggregated by up to 12 workstreams
- real-time visual feedback on data entry
- variable phase support to account for time-linked tasks
- filterable workstream views
- anyrow placement of tasks, subtasks and resources
- cost estimates by resource type, with capex and opex flags

#### In the future, Structure Planner will...
- increase the number of resource entries per workstream and deliver warnings and errors when exceeded
- include forecast measures like revenue and margin
- feature visuals displaying revenue/margin against project expenditure
- allow the user to create milestones and associate them with measures elsewhere
- deliver a nice roadmap chart of phases with milestones and financials
- deliver mermaid markup for hierarchy visualization
- fix the harmless but limiting display of errored values in the enum sheet associated with prepopulated workstreams

#### Structure planner does not...
- support sorting rows in the workstream view
- support more than 100 subtasks/resources per workstream (action blocked)

## Usage
##### Describing tasks
Use the workstream tabs and enter any values you'd like in Task, Subtask, Resource, and assign a base quantity.  Use the enum page to add or remove workstreams.  Workstreams are automatically summarized by task.

<img src="https://github.com/user-attachments/assets/4361a1dd-9c0a-4a33-a2f8-e90d59dc8b2a" alt="workstream summary" width="200"/>


##### Managing Workstreams
structurePlanner supports up to 12 workstreams.  To add a workstream:
  1. copy one of the existing sheets
  2. Assign it a name (Cell $B$2)
  3. Add the worksheet name to the workstream table in the enum worksheet

##### Cost Modeling (optional)
- resources described in the workstream tabs must be defined in the resource tab
- resource definition is NOT required if you do not need cost modeling
- the default list is populated by chatGPT query for fully loaded United States OTE for the job roles

##### Phasing Resources (optional)
- multiplier is a phase-specific head or tailwind applied to the **base declared value**, not the previous phase
- when phased values are manipulated, they are no longer tied to either the **base** or the **multiplier** and will be flagged as blue to indicate non-calucated value
- phasing is set on a per-workstream basis

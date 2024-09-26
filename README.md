## Usage

### Project Setup
<img src="https://github.com/user-attachments/assets/131e8ba8-3901-41bc-85ab-ac0af90787f1" alt="img" width="300"/>

- establish a start date, periodicity (month, quarter, year, etc)
- number of periods determines project duration
- multiplier is a phase-specific head or tailwind applied to the **base declared value**, not the previous phase

### Creating Tasks, Subtasks and Resources
<img src="https://github.com/user-attachments/assets/240e0fce-41f7-4588-aa62-52c254d5fcff" alt="img" width="200"/>

- columns j-k are completely user-defined
- the dropdowns are unenforced - to enter a new task, subtask or resource type the value
- values you enter will be reflected in the list
- newly declared resources will be flagged as red until added in the resources table (see [editing resources and costs](#resources))

### Resources
<img src="https://github.com/user-attachments/assets/240e0fce-41f7-4588-aa62-52c254d5fcff" alt="img" width="300"/>

- change the default resource types to those appropriate for your project
- add as many rows as you need, keeping everying in the table, and the calculated columns (gray font) untouched
- the default list is populated by chatGPT query for fully loaded United States OTE for the job roles
  
<img src="https://github.com/user-attachments/assets/918942ad-ed9b-4fa8-9497-8eb3a3a28906" alt="img" width="200"/>

Data are summarized by task in real time

#### Phasing Resources
<img src="https://github.com/user-attachments/assets/1c1ea617-93ff-4a6d-9600-70f25c3db87b" alt="img" width="400"/>

- when resources are variable depending on the phase, switch "phased" to "on"
- when values are manipulated, they are no longer tied to either the **base** or the **multiplier** and will be flagged as blue to indicate non-calucated value
### Adding a workstream

<img src="https://github.com/user-attachments/assets/0da27e30-2837-44bc-b7e4-ef0aa9a1c58c" alt="img" width="200"/>

- duplicate the template worksheet, rename the Excel worksheet and the workstream (Cell $B$2)

<img src="https://github.com/user-attachments/assets/e4270825-b050-443c-b87f-e3038daa86c4" alt="img" width="200"/>

- go to the enum worksheet and enter the name of the _Excel worksheet_ where the workstream is defined.  The workstream name will be automatically populated




# FAQ & roadmap

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

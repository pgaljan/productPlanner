  ## Usage
  ### Project and Phase Setup
<img src="https://github.com/user-attachments/assets/fd072a93-3e5e-41cf-867e-c9cde862de4e" alt="img" width="600"/>
  
- Set a Name and start date (defaults to today)
- Select a planning periodicity (from day to year)
- Name the four phases as you prefer
- establish the number of periods for each phase (Start/End automatically adjust)
- Select a percentage uplift to be applied to all resources present in the phase

### Workstream authoring and editing
<img src="https://github.com/user-attachments/assets/70e2622c-297c-47f3-a33a-b776fb8a2e51" alt="img" width="200"/>

- assign a workstream name to be used in visuals and reporting.  It can be different from the Excel worksheet name
<img src="https://github.com/user-attachments/assets/912ab02b-2e13-4d4f-865b-86dc804352a6" alt="img" width="600"/>

- dropdowns are pre-populated with previous values, and you are free to enter your own
- when you create your own resource types, they will be added to the dropdown, and flagged in red until you define the resource
- assign a quantity to each resource.  This will be multiplied by the estPerUnit calculated value in the resources table

#### Phasing the resources
<img src="https://github.com/user-attachments/assets/01a99b96-d23c-4d68-8422-750152a417a4" alt="img" width="600"/>

- when you select "On" for phased resources, additional columns appear aligning to the phases you've defined
- by default, each phase carries the base qty value via formula.  Edit the phases as you see fit.
- Manually changed values will be marked in blue font, and will not reflect changes to the base quantity.

Refer to phase setup for application of project-wide variables aligned to phases

### Defining Resources
<img src="https://github.com/user-attachments/assets/14d3ed7e-412b-4098-bfd7-21e4fb50b709" alt="img" width="200"/>

- Resources you create or edit in this table will be present in the resource drop down
- note the resources in red on each tab and enter them on this table
- cost estimates are optional

### Workstream results
<img src="https://github.com/user-attachments/assets/5efe4729-ee6c-4a08-b0ea-5ea83cfdf97e" alt="img" width="200"/>

- key measures are summarized by workstream
- tasks are listed with key measures summarized by task within the workstream
<img src="https:/github.com/user-attachments/assets/fff16dbe-07a2-449e-97db-a269310a1f1d" alt="img" width="200"/>

- in the workstream you see a real time summary of the tasks, with number of subtasks and associated resource types, along with base quantity cost
  
### Adding a workstream
there are ten hidden workstream templates for a total of 12 supported workstreams in the workbook
<img src="https://github.com/user-attachments/assets/611acfaf-5917-41b9-821a-bd2969df2c92" alt="img" width="200"/>

- to add a workstream, unhide one of the templates and rename the worksheet and the workstream ($B$2)
- go to the enum worksheet and enter the name of the Excel worksheet where the workstream is defined.  The workstream name will be automatically populated
- if you enter an invalid worksheet name, you'll be prompted to fix it.
- optionally enter the order that you would like the workstreams displayed

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

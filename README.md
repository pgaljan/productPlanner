[Download (github)](https://github.com/pgaljan/structurePlanner/archive/refs/heads/main.zip)

# Structure Planner
1. [Overview](#Overview)
2. [Usage](#Usage)
3. [FAQ](#FAQ)

# Overview

Structure Planner is a lightweight Excel-based project quantification tool that provides powerful, simple, and structured project planning with up to 12 workstreams. It is designed for agile, small (two-pizza) teams to facilitate early project phase ideation, cost estimation, and task visualization. The tool offers independently configurable work periods and project phases, so it can be used for very small consisting of a few sprints, to wide-ranging projects spanning decades.  It works seamlessly across platforms, including mobile and web, and does not rely on macros or external plugins, making it ideal for small teams lacking a commonly accessible Enterprise Project Management (EPM) system.

#### Key Features:
- 4-tier project planner for structured project planning.
- Support for up to 12 workstreams.
- Up to 12 progressively exposable project phases of arbitrary length, with configurable headwinds or tailwinds
- A wide range of work periods from days, weeks, months, quarters or years.
- Designed for Excel for web and mobile compatibility.
- Delivered in a VB- and PowerQuery-free workbook with protected sheets for error-free authoring (without passwords).

# Usage

### 1. Describing Tasks
To describe and organize tasks within Structure Planner:
- Use the **workstream tabs** (one for each workstream) to enter values in the following columns:
  - **Task**: Name or description of the task.
  - **Subtask**: Break down the task further into specific actions.
  - **Resource**: Identify resources associated with the task or subtask.
  - **Base Quantity**: Assign the quantity of each resource needed for the task or subtask.
- For workstream management, navigate to the **enum page** to add or remove workstreams.
- Each workstream is automatically **summarized by task**, showing the aggregate effect of your input.

<img src="https://github.com/user-attachments/assets/4361a1dd-9c0a-4a33-a2f8-e90d59dc8b2a" alt="workstream summary" width="400"/>

### 2. Managing Workstreams
Structure Planner supports up to **12 workstreams**. To add a new workstream:
1. **Copy an existing sheet**: Duplicate one of the existing workstream sheets.
2. **Rename the worksheet**: to a string starting with **"ws"**
3. **Name your workstream**: Change the sheet name by editing **Cell $B$2** with your chosen name.
4. **Register the new workstream**: Go to the **Setup worksheet** and add the new worksheet name (_"ws[your string]"_) in the **workstream table**.
5. Include or exclude the workstream in the dashboard views by toggling "include"

### 3. Cost Modeling (Optional)
Structure Planner provides **cost modeling** based on resource definitions.
- Each **resource** described in the workstream tabs must be defined in the **Resource Tab** for cost calculations.
- **Cost modeling is optional**: You can skip resource definitions if you don’t need cost calculations.
- The default resource list is populated using **fully loaded United States OTE (On-Target Earnings)** for typical job roles (pre-populated via a ChatGPT query).

### 4. Phasing Resources (Optional)
Structure Planner allows you to phase resources over time, applying specific multipliers to resource values for each phase.
<img src="https://github.com/user-attachments/assets/21b64792-d5ab-4a69-8f00-d3fb14b77cd1" alt="workstream summary" width="400"/>

- **Phase-specific multipliers**: You can apply a phase-specific headwind or tailwind applied against the **first phase** of a resource for each phase. Uplifts do not accumulate
- **Non-calculated values**: If you manually adjust the resource values in a phase, they will no longer be linked to the base or multiplier.  Non-calculated values are flagged **blue**.



# FAQ

### 1. **What is Structure Planner?**
Structure Planner is a simple yet powerful, 4-tier project planning tool designed for agile, small teams. It helps with early project phase ideation, cost sizing, and task visualization, supporting up to 12 workstreams, giving rich, real-time visual feedback to the author. It is designed to handle different time periods and works without macros (VB- and PowerQuery-free).

---

### 2. **What type of projects is Structure Planner suitable for?**
Structure Planner is ideal for:
- Early-stage project ideation and planning
- Quick cost estimation and iteration during contract bidding phases
- Projects that need to identify major milestones ("big rocks") early on
- Running "what-if" analyses, business case development, and parallel analysis (e.g., red/blue teams)
- Cross-organizational collaboration where different teams may use diverse data structures
- Auditing and modeling operational project structures for implementation in Enterprise Project Management (EPM) software

---

### 3. **How many workstreams can I manage with Structure Planner?**
Structure Planner supports up to **12 workstreams**, making it suitable for managing multiple task flows within a project.

---

### 4. **Can I customize the length of the project timespan and work periods?**
Yes, Structure Planner can handle an arbitrary number of work periods and timespans. It can be configured to work with different time periods such as **days, weeks, quarters, or years**.

---

### 5. **Is Structure Planner compatible with Excel for web and mobile devices?**
Yes, Structure Planner is designed to be **Excel for web compatible** and mobile-friendly, making it accessible across various devices and platforms without any dependencies on VBA or PowerQuery.

---

### 6. **What kind of data entry is required?**
Structure Planner requires a **simple, 5-parameter data entry** for defining resources. You can add tasks, subtasks, and resources freely and receive **real-time visual feedback** as you populate data.

---

### 7. **Does Structure Planner include financial estimates and cost modeling?**
Yes, Structure Planner provides **cost estimates by resource type** and allows you to flag expenses as either **CapEx (Capital Expenditure)** or **OpEx (Operational Expenditure)**. It summarizes financials and key measures across all workstreams.

---

### 8. **What are some key features delivered by Structure Planner?**
- Simple data entry for tasks and resources
- Automatic aggregation and summarization of key metrics across workstreams
- Support for variable project phases and time-linked tasks
- Filterable workstream views and real-time feedback on data entry
- Flexible task placement anywhere within the worksheet
- Quickly identify when the cost impact of a resource has changed between analyses using **resource hash**

---

### 9. **What are the current limitations of Structure Planner?**
- **No sorting support** for rows within the workstream view.
- **Resource limits**: Currently, it supports up to 100 subtasks/resources per workstream for a total of 1,200 resources, 12 workstreams, and 12 planning phases spanning an arbitrary number of years.
  
---

### 10. **What future features are planned for Structure Planner?**
- Workstream hashing
- Forecast measures like revenue and margin
- Visuals comparing **revenue/margin against project expenditure**
- Milestone creation and tracking within phases
- Roadmap charts for project phases and milestones
- Mermaid markup support for project hierarchy visualization
- Fix for minor display errors in the workstream enum sheet

---

### 11. **Does Structure Planner require VBA or macros to run?**
No, Structure Planner is a **VBA and PowerQuery-free** tool, ensuring that it runs smoothly across all Excel environments without relying on macros or additional dependencies.

---

### 12. **Can I use Structure Planner to audit Operational Project Plans?**
Yes, Structure Planner can be leveraged to perform high-level analyses in parallel to those produced and managed in Enterprise Project Management (EPM) tools, as well as simulating notional project structures for future implementation in those tools.

---
### 13. **What is the purpose of hashing?**
Hashes aid in change tracking and drift detection.  They are pseudo-unique hex values assigned to resources by applying a lambda function against a combination of critical attributes.  As mutliple users may do perform changes independently and asynchronously, hashes allow users to quickly visually and programmatically idenitfy which elements have changed.  They can be also be used in downstream processing to create changelogs and facilitate comparative analysis in red/blue team analysis scenarios.

Because they are computationally intensive, hashes are not calculated and thus not present in any functions or named arrays.  Be aware of this if you plan to leverage them in a downstream repository.  Also note that although financials behave similarly in that toggling the cost planning flag will remove the resource cost multiplier, the resources table will hold default values populated for merging into downstream analysis. 

---

### 14. **Is there a way to model phases or variable time-linked tasks?**
Yes, Structure Planner supports **phasing resources**, which allows you to apply phase-specific adjustments to resources over time and manage tasks linked to specific phases within the project.

---

### 15. **How do I know when I've exceeded resource limits?**
Structure Planner will deliver **warnings and errors** when the number of resource entries exceeds the current limits per workstream.

---
### 16. **What are Structure Planner's cost and license terms?**

Structure Planner is licensed under the MIT License. You are free to use, modify, and distribute the tool, provided that the original authorship and license remain attributed. For the full license text, refer to the attached LICENSE file or visit [MIT License](https://opensource.org/licenses/MIT).

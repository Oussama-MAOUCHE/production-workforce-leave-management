# Production Workforce Leave & Absence Management Application

Windows desktop application I designed and developed in-house while working in a gas-production department at **AMC (later SAIEG — Sonelgaz Group)**.

The department covered gas-meter and gas-regulator production and had a workforce of roughly 100 people. With a lean supervisory structure, keeping employee records, annual leave, sick leave and other absences consistent and easy to review was time-consuming. I built this application on my own initiative to centralize that follow-up and give the production team a clearer view of workforce availability and absence history.

The application supported human decision-making; it did not automatically allocate leave or calculate a fairness score.

## At a glance

| Area | Details |
|---|---|
| Professional context | Gas production department — AMC / later SAIEG (Sonelgaz Group) |
| My contribution | Independently initiated, designed and developed the application |
| Application type | Windows desktop business application |
| Technologies | WINDEV / WLanguage, HFSQL |
| Main modules | Employees, leave/absence records, monthly calendar |
| Main capabilities | CRUD workflows, search/filtering, date-range tracking, calendar visualization |
| Workforce context | Roughly 100 production employees |

## Why I built it

Employee follow-up was only one part of the production-engineering workload. The same small management structure also had to monitor products, production activity and production lines.

Tracking leave and absences manually across roughly 100 employees made it difficult to maintain a clear history and review requests consistently across teams.

I created the application to:

- centralize employee records;
- keep a structured leave/absence history;
- make records easier to search and filter;
- provide a monthly visual overview of workforce absences;
- support more consistent review of leave and absence history across teams.

## Employee management

The employee module supports:

- employee listing;
- add, modify and delete workflows;
- employee number and section information;
- filtering by name;
- filtering by employee number;
- filtering by production section.

![Employee management screen](assets/employee-list.png)

## Leave & absence management

The absence module supports:

- leave/absence records linked to employees;
- add, modify and delete workflows;
- multiple absence/leave categories;
- start and end dates;
- displayed duration in days;
- filtering by date range;
- search by employee name.

![Leave and absence records](assets/absence-list.png)

## Monthly calendar

The calendar provides a visual overview in addition to the tabular records.

Employees are displayed as rows and days as columns, while recorded absence periods appear as colored ranges across the month. This makes overlapping leave and workforce availability easier to review at a glance.

![Monthly workforce absence calendar](assets/monthly-calendar.png)

## Technical design

The application uses a small relational model with two main entities:

**Employee**
- employee ID;
- name;
- employee number;
- section.

**Absence**
- absence ID;
- employee ID;
- absence type;
- start date;
- end date.

Each absence record is linked to an employee through the employee ID.

## Portfolio scope

This is a focused internal production-support application, not a payroll system or full HRIS.

The project demonstrates:

- multi-screen desktop development;
- CRUD business workflows;
- relational data modeling;
- search and filtering;
- date-range handling;
- employee-to-absence relationships;
- calendar-style data visualization;
- translating an operational production need into an internal software tool.

The screenshots use test/demo data. Raw HFSQL files, WINDEV project files and internal development artifacts remain private.

See:

- [Technical Notes](docs/technical-notes.md)
- [Evidence & Confidentiality](evidence/README.md)

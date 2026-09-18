# Technical Notes

## Application structure

The application is organized around three primary areas:

1. employee management;
2. leave/absence management;
3. monthly calendar visualization.

Dedicated add/modify dialogs support employee and absence record workflows.

## Project chronology

Surviving project artifacts begin in January 2020.

Core employee/absence screens and query artifacts were developed during 2020, with later project/environment artifacts continuing into 2021.

The portfolio therefore records the evidence span as **2020–2021** without inventing a single exact release date.

## Employee workflow

The employee area supports:

- listing employees;
- employee ID/number and production section;
- add and modify dialogs;
- delete action;
- filtering by name;
- filtering by employee number;
- filtering by section.

Observed production-section values include gas-meter and gas-regulator areas.

## Leave & absence workflow

The absence area supports:

- employee-linked absence records;
- add and modify dialogs;
- delete action;
- date-range filtering;
- search by employee;
- absence type;
- start/end dates;
- displayed duration.

Observed categories include annual leave, sick leave, special leave and irregular absence.

## Calendar visualization

The monthly calendar presents employees as rows and calendar days as columns.

Absence periods are represented as colored horizontal ranges across the selected month. The view complements the standard record list by making workforce availability easier to scan visually.

## Data model

The WINDEV analysis exposes two main entities.

### Employee

- employee ID;
- name;
- employee number;
- section.

### Absence

- absence ID;
- employee ID;
- absence type;
- start date;
- end date.

The employee ID links absence records to the employee entity.

## Technology

Surviving project/runtime artifacts support:

- WINDEV / WLanguage;
- WINDEV 23 runtime components;
- local HFSQL data storage.

The public repository documents the verified application design and workflow without republishing proprietary native project/database files.

## Scope boundary

The application is presented as a focused production-workforce support tool.

It does not claim:

- payroll processing;
- automated leave approval;
- entitlement-balance calculation;
- statutory HR compliance;
- a fairness-scoring algorithm;
- a quantified absenteeism-reduction percentage;
- enterprise HRIS scope.

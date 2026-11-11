# ROADLINK – Road Disruption Reporting and Transport Coordination System

## 1. Project Information

| Item | Description |
|---|---|
| Project Title | ROADLINK |
| Full Name | Road Disruption Reporting and Transport Coordination System |
| Student Name | Sano Gervais |
| Student ID | 20251SEN160 |
| Project Type | Final-Year Software Engineering Project |
| Development Status | Proposed – Not Yet Started |
| Application Type | Web-Based System |
| Database | Oracle Database / PL/SQL |
| AI Integration | Not Included |

## 2. Project Overview

ROADLINK is a proposed web-based transport management system designed to improve the reporting and sharing of road disruption information.

The system will allow drivers and other road users to report problems such as road accidents, flooding, road construction, vehicle breakdowns and blocked roads. Transport officers will be responsible for reviewing submitted reports, verifying information and updating road conditions.

Other drivers and passengers will be able to view verified road information and available alternative routes.

The main purpose of ROADLINK is to improve communication between road users and transport officers, reduce unnecessary travel delays and support better transport coordination.

## 3. Problem Statement

Road users sometimes experience unexpected transport disruptions, including accidents, flooding, road construction and vehicle breakdowns. In some situations, drivers and passengers may not receive information about these problems before reaching the affected locations.

This can result in unnecessary travel delays, additional transport costs, wasted fuel and difficulties in planning journeys.

ROADLINK proposes a centralized platform where road users can report disruptions and authorized transport officers can verify and share updated road information.

## 4. Project Objectives

### Main Objective

To design and develop a web-based system that enables road users to report transport disruptions and allows authorized officers to verify reports and share updated road information.

### Specific Objectives

1. To develop a user registration and login system for drivers, passengers and transport officers.
2. To provide a platform for reporting road disruptions with their locations and descriptions.
3. To implement a report verification process that allows transport officers to approve or reject submissions.
4. To provide updated road conditions and alternative routes to road users.
5. To design and implement a relational database using Oracle Database.
6. To apply PL/SQL programming concepts for database operations, validation and report management.

## 5. Data Sources

The project will use public geographic data to support road location identification and map display.

### Primary Data Source

**Rwanda Transport Development Agency (RTDA) – Road Network**

This geographic data source provides information about Rwanda's road network, including road categories and geographical information.

Link: https://infrastructure.space.gov.rw/server/rest/services/Road_Network/FeatureServer/0

### Supporting Data Source

**Geofabrik – OpenStreetMap Rwanda Extract**

This source provides downloadable OpenStreetMap geographic data for Rwanda. It can be used to support road mapping and location identification.

Link: https://download.geofabrik.de/africa/rwanda.html

### Planned System Data

In addition to public geographic data, I plan to create sample records for:

- Road disruption reports.
- Accident and flooding reports.
- Road construction information.
- Vehicle breakdown reports.
- Road status updates.
- Alternative routes.
- User and administrator information.

**Note:** The project has not started development. The sample records will be created during implementation and will not be presented as actual reported incidents.

## 6. Planned Innovation

The planned innovation of ROADLINK is to combine community-based road disruption reporting with an official verification process.

Unlike a simple reporting platform, the proposed system will allow authorized transport officers to review submitted reports, approve or reject them, maintain report history and update road conditions.

It will also provide a centralized way to share verified information and alternative routes with other road users.

The system will use conventional software development, database management and predefined business rules. It will not involve Artificial Intelligence (AI).

## 7. Planned Database Tables

The system will use a relational database to organize and manage information.

| Table | Purpose |
|---|---|
| USERS | Stores user accounts and personal information. |
| ROAD_REPORTS | Stores submitted road disruption reports. |
| LOCATIONS | Stores affected road names and geographical locations. |
| PROBLEM_CATEGORIES | Stores disruption types such as accidents, flooding and roadworks. |
| ROAD_STATUS | Stores road condition information and status changes. |
| ALTERNATIVE_ROUTES | Stores alternative routes provided by transport officers. |
| NOTIFICATIONS | Stores notifications sent to users. |
| VERIFICATION_LOG | Stores report verification decisions and officer information. |

### Planned Database Relationships

- One user can submit multiple road reports.
- Each road report belongs to a problem category.
- Each road report is associated with a location.
- A road report can have multiple verification records or status updates.
- A road report can have alternative route information.
- Users can receive multiple notifications.

Primary keys (PK) and foreign keys (FK) will be used to maintain relationships between tables.

## 8. Planned Oracle PL/SQL Features

I plan to apply Oracle PL/SQL concepts to manage database operations and enforce system rules.

### Procedures

- `REGISTER_USER` – Registers new users.
- `SUBMIT_ROAD_REPORT` – Saves road disruption reports.
- `VERIFY_REPORT` – Approves or rejects reports.
- `UPDATE_ROAD_STATUS` – Updates road conditions.
- `ADD_ALTERNATIVE_ROUTE` – Saves alternative routes.

### Functions

- `GET_ROAD_STATUS` – Returns the current status of a road report.
- `COUNT_ACTIVE_REPORTS` – Counts active disruption reports.
- `GET_REPORT_SUMMARY` – Returns a summary of road reports.

### Cursors

- Implicit cursors for checking database operations and affected records.
- Explicit cursors for retrieving and processing pending road reports.

### Triggers

- Record road status changes.
- Create notification records when reports are approved or rejected.

### Packages

- `PKG_ROAD_REPORTS` – Manages road report operations.
- `PKG_USER_MANAGEMENT` – Manages user accounts and roles.

### Exception Handling

I plan to handle errors such as:

- Report not found.
- Invalid location.
- Duplicate report submission.
- Unauthorized operations.
- Unexpected database errors.

## 9. Planned Project Structure

The project will initially follow this folder organization. Additional folders and implementation files will be introduced during later development phases.

```text
ROADLINK/
│
├── docs/
│   ├── research/
│   │   └── README.md
│   │
│   ├── proposal/
│   │   └── README.md
│   │
│   └── presentation/
│       └── README.md
│
├── data/
│   └── README.md
│
└── README.md
```

### Folder Responsibilities

- `docs/research/` – Contains research materials, existing system analysis and references.
- `docs/proposal/` – Contains the project proposal, problem statement, objectives and planned design.
- `docs/presentation/` – Contains project presentation materials.
- `data/` – Contains public geographic datasets and sample data used during development.
- `README.md` – Provides the main project description and documentation.

## 10. Expected Results

After completing development, I expect ROADLINK to provide:

1. A working user registration and login system.
2. A road disruption reporting platform.
3. An administrator and transport officer dashboard.
4. A report verification and approval process.
5. Road condition information.
6. Alternative route management.
7. Database records and PL/SQL implementation.
8. Reports showing road disruption information.

These are expected results, not completed features.

## 11. References

1. City of Kigali. (n.d.). *Rwanda Urban Mobility Improvement Project (RUMI).* https://www.kigalicity.gov.rw/rwanda-urban-mobility-improvement-rumi-project

2. Geofabrik GmbH. (n.d.). *Rwanda: OpenStreetMap data.* https://download.geofabrik.de/africa/rwanda.html

3. Google. (n.d.). *Report traffic incidents in Google Maps.* Google Maps Help. https://support.google.com/maps/answer/9770907

4. Google. (n.d.). *Report road hazards.* Waze Help. https://support.google.com/waze/answer/13739290

5. Rwanda Transport Development Agency. (n.d.). *Road Network [Feature Layer].* Rwanda Spatial Data Infrastructure. https://infrastructure.space.gov.rw/server/rest/services/Road_Network/FeatureServer/0

6. World Bank. (2025, June 25). *Transforming Kigali's urban mobility to improve commutes and create jobs.* https://www.worldbank.org/en/news/press-release/2025/06/25/transforming-afe-kigali-urban-mobility-to-improve-commutes-and-create-jobs

---

## 12. Project Development Commitment

ROADLINK is a proposed final-year project that I intend to develop as part of my software engineering studies. I am committed to putting effort into its research, planning, database design, implementation and testing.

My goal is to transform this idea into a functional system that addresses a practical transport challenge in Rwanda while strengthening my software engineering and database development skills.

**Project Status: PROPOSED – DEVELOPMENT NOT YET STARTED.**

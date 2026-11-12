# ROADLINK – Research Log

**Project title:** ROADLINK – Road Disruption Reporting and Transport Coordination System
**File:** `research_log.md`
**Research purpose:** To investigate road disruption reporting, transport coordination, existing systems, available datasets, and technologies that can support the proposed ROADLINK system.

---

## 1. Introduction

ROADLINK is a proposed system that will allow road users to report road disruptions such as:

- Road accidents
- Flooding
- Road construction
- Blocked roads
- Vehicle breakdowns

Authorized transport officers will be able to review submitted reports, approve or reject them, and update their status. Users will be able to view verified road conditions and alternative routes entered by authorized officers.

This research will help identify the problem, understand existing solutions, and select suitable data sources and technologies for developing the system.

## 2. Research Objectives

The research aims to:

1. Understand how road disruptions affect transport and road users.
2. Study how crowdsourcing can help collect road incident information.
3. Identify existing road reporting systems and their limitations.
4. Find reliable road-network and transport information for Rwanda.
5. Identify technologies that can support the proposed database and application.
6. Identify a possible gap that ROADLINK can address.

## 3. Research Methods and Sources

The research uses academic publications, official government information, existing transport applications, public datasets, and technical documentation.

The following platforms and sources were considered:

- **Google Scholar:** To identify academic research about crowdsourcing and road incident reporting.
- **IEEE Xplore:** To find research about smart mobility and transport safety systems.
- **ScienceDirect:** To find research about the reliability of crowdsourced traffic reports.
- **National Institute of Statistics of Rwanda (NISR):** To find official Rwanda transport and road accident statistics.
- **World Bank:** To understand transport and urban mobility challenges in Rwanda.
- **Oracle Documentation:** To understand the database programming technologies required for the project.

## 4. Research Sources and Findings

### 4.1 Research Paper One – Reliability of Crowdsourced Road Reports

**Authors:** Salamanis, A., Drosou, A., Michalopoulos, D., Kehagias, D., and Tzovaras, D.
**Year:** 2016
**Title:** *A Probabilistic Framework for the Reliability Assessment of Crowd Sourcing Urban Traffic Reports.*
**Journal:** Transportation Research Procedia, Volume 14, pages 4552–4561.
**DOI:** [https://doi.org/10.1016/j.trpro.2016.05.378](https://doi.org/10.1016/j.trpro.2016.05.378)
**Source:** ScienceDirect.

**Research findings:**

This research explains how road users can submit traffic incident reports and share information with other travellers. It also identifies an important problem: reports submitted by users may not always be correct.

The researchers propose a method for estimating the reliability of submitted reports using information such as the reporting user's location and speed.

**Relevance to ROADLINK:**

This paper shows why road reports should be checked before they are shared with other users. ROADLINK will address this issue through a human verification process where authorized transport officers review reports before they become verified.

**Limitation for our project:**

The research uses a probabilistic model. ROADLINK will not implement this model or AI-based verification. It will use an officer-based approval process.

### 4.2 Research Paper Two – Crowdsourcing Incident Data for Urban Mobility

**Authors:** Chavez, C. V., Ruiz, E., Rodriguez, A. G., Pena, I. R., Larios, V. M., Villanueva-Rosales, N., Mondragon, O., and Cheu, R. L.
**Year:** 2019
**Title:** *Towards Improving Safety in Urban Mobility Using Crowdsourcing Incident Data Collection.*
**Conference:** 2019 IEEE International Smart Cities Conference (ISC2), pages 626–631.
**DOI:** [https://doi.org/10.1109/ISC246665.2019.9071714](https://doi.org/10.1109/ISC246665.2019.9071714)
**Source:** IEEE Xplore.

**Research findings:**

This paper presents a Safe Commuting System that collects safety information from users through mobile devices. The system uses historical and real-time reports to inform commuters about incidents and areas that may be unsafe.

It also discusses user notifications and the possibility of providing alternative routes.

**Relevance to ROADLINK:**

The research supports the idea of collecting incident information from road users and making useful information available to other travellers.

ROADLINK will apply a related idea to road disruptions, including accidents, flooding, roadworks, and blocked roads.

**Difference:**

The research focuses mainly on commuter safety incidents. ROADLINK will focus on road disruptions and coordination between road users and authorized transport officers.

### 4.3 Report and Statistics – Rwanda Transport Information

**Organization:** National Institute of Statistics of Rwanda (NISR).
**Publication:** *Rwanda Statistical Yearbook 2025.*
**Source:** [https://www.statistics.gov.rw/sites/default/files/documents/2026-01/RWANDA_STATISTICAL_YEARBOOK_2025_0.pdf](https://www.statistics.gov.rw/sites/default/files/documents/2026-01/RWANDA_STATISTICAL_YEARBOOK_2025_0.pdf)

**Research findings:**

The 2025 Statistical Yearbook includes road accident information for Rwanda. Its road accident table reports the following figures:

| Indicator                   |       2023 |  2024 |
| --------------------------- | ---------: | ----: |
| Fatal accidents             |        761 |   692 |
| Serious injury accidents    |        262 |   228 |
| Minor injury accidents      |      5,037 | 3,097 |
| Property damage accidents   |      3,935 | 3,341 |
| Road traffic accident total | Not stated | 6,688 |

The report also provides information about transport and vehicle inspections. The figures are reported by the Rwanda National Police.

**Relevance to ROADLINK:**

This information provides a Rwanda-specific background for understanding road safety and transport challenges. It can support the problem background and research justification.

**Important note:**

These are official road accident statistics, not live road disruption reports. They should not be used as real-time incident records in the application.

### 4.4 Report – World Bank Rwanda Urban Mobility

**Organization:** World Bank.
**Date:** 25 June 2025.
**Title:** *Transforming Kigali’s Urban Mobility to Improve Commutes and Create Jobs.*
**Source:** [https://www.worldbank.org/en/news/press-release/2025/06/25/transforming-afe-kigali-urban-mobility-to-improve-commutes-and-create-jobs](https://www.worldbank.org/en/news/press-release/2025/06/25/transforming-afe-kigali-urban-mobility-to-improve-commutes-and-create-jobs)

**Research findings:**

The World Bank explains that Kigali faces several urban mobility challenges, including traffic congestion, inadequate public transport services, limited pedestrian and cycling infrastructure, and road safety concerns.

The report also describes the Rwanda Urban Mobility Improvement Project, which aims to support safer and more accessible transport.

**Relevance to ROADLINK:**

The report provides context about transport challenges in Kigali. ROADLINK is proposed as a supporting information system that could help road users and transport officers share information about disruptions and road conditions.

### 4.5 Existing System – Waze

**System:** Waze
**Official website:** [https://www.waze.com/](https://www.waze.com/)
**Official help page:** [https://support.google.com/waze/answer/13739290?hl=en](https://support.google.com/waze/answer/13739290?hl=en)

**System description:**

Waze is a navigation application that allows users to report road hazards and share information with other drivers.

Users can report different types of hazards, including:

- Road construction
- Vehicles stopped on the roadside
- Broken traffic lights
- Potholes
- Objects on the road

Waze also supports road closure reporting.

**Relevance to ROADLINK:**

Waze demonstrates that user-generated road information can help drivers understand road conditions.

**Identified difference and opportunity:**

ROADLINK will not attempt to replace Waze or become a full navigation application. Its proposed focus is a structured reporting and officer-verification process, with report status history and transport coordination.

### 4.6 Dataset – Rwanda Road Network

**Dataset provider:** Rwanda Transport Development Agency (RTDA) / Ministry of Infrastructure.
**Dataset name:** Road_Network Feature Layer.
**Dataset link:** [https://infrastructure.space.gov.rw/server/rest/services/Road_Network/FeatureServer](https://infrastructure.space.gov.rw/server/rest/services/Road_Network/FeatureServer)

**Dataset description:**

This dataset contains road-network information for Rwanda. It represents roads as geographic line features and includes different road categories, such as:

- National roads
- District road class 1
- District road class 2
- Other roads, streets, and paths

The road layer provides information that can help identify and display road locations.

The service supports data formats such as JSON, GeoJSON, and PBF.

**Relevance to ROADLINK:**

The dataset can provide the road-network reference needed to connect submitted reports with road locations.

For example, when a user reports flooding or an accident, the application could associate the report with a road or location.

**Important dataset limitation:**

This is a road-network dataset, not a live road accident or disruption dataset. It does not automatically provide current accidents, flooding, road closures, or traffic conditions.

**Planned use:**

1. Examine the available road attributes.
2. Query or export suitable road features.
3. Check the geographic data and coordinate reference system.
4. Prepare the data for use in the application.
5. Connect road reports to the relevant road locations.

The service's `MaxRecordCount` of 2,000 is a query response limit, not the total number of roads in the dataset. The actual number of records should be checked when the data is downloaded.

### 4.7 Technical Source – Oracle Database PL/SQL

**Organization:** Oracle.
**Year:** 2024.
**Documentation:** *Oracle Database PL/SQL Language Reference (21c).*
**Official documentation:** [https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/index.html](https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/index.html)

**Technical findings:**

Oracle PL/SQL provides database programming features that allow developers to create procedures, functions, cursors, triggers, packages, and exception-handling routines.

These features can help developers manage database operations and business rules.

**Relevance to ROADLINK:**

Oracle PL/SQL can support important database operations, including:

- Registering road reports.
- Updating report statuses.
- Approving or rejecting reports.
- Retrieving reports for users and officers.
- Recording verification history.
- Handling invalid data and database errors.

**Planned implementation:**

The project will use Oracle Database and PL/SQL to manage data and implement selected database operations.

## 5. Summary of Research Sources

| No. | Source category          | Source                         | Main contribution                                  |
| --- | ------------------------ | ------------------------------ | -------------------------------------------------- |
| 1   | Research paper           | Salamanis et al. (2016)        | Reliability of crowdsourced traffic reports        |
| 2   | Research paper           | Chavez et al. (2019)           | Crowdsourced incident reporting for urban mobility |
| 3   | Rwanda report/statistics | NISR Statistical Yearbook 2025 | Rwanda road accident statistics                    |
| 4   | Mobility report          | World Bank (2025)              | Kigali urban mobility challenges                   |
| 5   | Existing system          | Waze                           | Real-world road hazard reporting                   |
| 6   | Dataset                  | RTDA Road_Network              | Rwanda road-network information                    |
| 7   | Technical source         | Oracle PL/SQL Documentation    | Database programming and management                |

## 6. Identified Research Gap

The reviewed research and existing systems demonstrate that collecting road information from users can support transport and road safety.

However, the proposed ROADLINK project will focus on a specific workflow:

1. A road user submits a disruption report.
2. The system stores the report and its location.
3. An authorized transport officer reviews the report.
4. The officer approves or rejects it.
5. The system records the verification decision and status history.
6. Verified road conditions are displayed to users.
7. Authorized officers can enter alternative routes where necessary.

The project will focus on connecting road users with authorized transport officers through a structured reporting and verification process.

This is the proposed focus of ROADLINK, not a claim that other systems do not provide verification or reporting features.

## 7. Planned Data Collection and Preparation

The project will use the RTDA road-network dataset as a geographical reference.

Additional sample incident records will be created for development and testing if real incident data is not publicly available.

Possible report information includes:

- Report ID
- User ID
- Incident category
- Description
- Road name or location
- Date and time reported
- Report status
- Verification officer
- Verification date
- Alternative route information

**Data quality considerations:**

- Avoid duplicate reports where possible.
- Validate required fields.
- Store accurate dates and locations.
- Keep rejected and approved reports distinguishable.
- Maintain a history of verification decisions.
- Clearly identify sample records as test data.

## 8. Conclusion

The research shows that road disruption reporting can benefit from crowdsourced information, reliable road-network data, and structured management of submitted reports.

The NISR and World Bank publications provide Rwanda-specific transport context. The reviewed academic papers explain the importance of crowdsourcing and report reliability. Waze provides an example of an existing road hazard reporting system, while the RTDA dataset can provide road-network information.

Oracle PL/SQL provides the technical features needed to manage the proposed database operations.

Based on these findings, ROADLINK is proposed as a road disruption reporting and transport coordination system that will connect road users and authorized transport officers through report submission, verification, status tracking, and alternative route information.

## 9. References

1. Chavez, C. V., Ruiz, E., Rodriguez, A. G., Pena, I. R., Larios, V. M., Villanueva-Rosales, N., Mondragon, O., & Cheu, R. L. (2019). *Towards improving safety in urban mobility using crowdsourcing incident data collection*. 2019 IEEE International Smart Cities Conference (ISC2), 626–631. [https://doi.org/10.1109/ISC246665.2019.9071714](https://doi.org/10.1109/ISC246665.2019.9071714)

2. National Institute of Statistics of Rwanda. (2026). *Rwanda Statistical Yearbook 2025*. [https://www.statistics.gov.rw/sites/default/files/documents/2026-01/RWANDA_STATISTICAL_YEARBOOK_2025_0.pdf](https://www.statistics.gov.rw/sites/default/files/documents/2026-01/RWANDA_STATISTICAL_YEARBOOK_2025_0.pdf)

3. Oracle. (2024). *Oracle Database PL/SQL Language Reference (21c)*. [https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/index.html](https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/index.html)

4. Rwanda Transport Development Agency. (n.d.). *Road_Network Feature Layer*. [https://infrastructure.space.gov.rw/server/rest/services/Road_Network/FeatureServer](https://infrastructure.space.gov.rw/server/rest/services/Road_Network/FeatureServer)

5. Salamanis, A., Drosou, A., Michalopoulos, D., Kehagias, D., & Tzovaras, D. (2016). *A probabilistic framework for the reliability assessment of crowd sourcing urban traffic reports*. Transportation Research Procedia, 14, 4552–4561. [https://doi.org/10.1016/j.trpro.2016.05.378](https://doi.org/10.1016/j.trpro.2016.05.378)

6. Waze. (n.d.). *Report road hazards*. Waze Help. [https://support.google.com/waze/answer/13739290?hl=en](https://support.google.com/waze/answer/13739290?hl=en)

7. World Bank. (2025, June 25). *Transforming Kigali’s urban mobility to improve commutes and create jobs*. [https://www.worldbank.org/en/news/press-release/2025/06/25/transforming-afe-kigali-urban-mobility-to-improve-commutes-and-create-jobs](https://www.worldbank.org/en/news/press-release/2025/06/25/transforming-afe-kigali-urban-mobility-to-improve-commutes-and-create-jobs)

---

## 10. Research Completion Checklist

- [x] At least two research papers identified.
- [x] Rwanda report/statistics identified.
- [x] Existing road reporting system reviewed.
- [x] Rwanda road-network dataset identified.
- [x] Oracle technical documentation identified.
- [x] Research findings connected to the ROADLINK project.
- [x] Research gap described.
- [ ] Download and inspect the RTDA road-network data.
- [ ] Record the actual dataset download date and number of extracted features.
- [ ] Save copies of the research papers and reports where access permits.
- [ ] Add any additional sources discovered during project development.

**End of Research Log**


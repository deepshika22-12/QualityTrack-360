# QualityTrack 360
### Manufacturing Quality Inspection & Defect Tracking System

QualityTrack 360 is a manufacturing quality inspection management solution built using Microsoft Power Platform. It helps manage equipment inspections, record defects, track inspection results, and automate notifications for failed inspections.

## Project Overview

The solution aims to streamline quality inspection processes by providing a centralized platform for recording inspection details and identifying equipment quality issues.

## Technologies Used

- Microsoft Power Apps – Canvas application interface
- Microsoft Dataverse – Structured data storage
- Power Automate – Workflow automation and email notifications
- Microsoft Outlook – Automated email alerts
- GitHub – Project documentation and version control

## Key Features

### 1. Equipment Inspection Management
- Record equipment inspection details.
- Maintain inspector information.
- Store inspection results.
- Record remarks and corrective actions.

### 2. Inspection Result Tracking

Inspection results use the following options:
- Pass
- Fail
- Needs Review

### 3. Defect Management

The system supports:
- Defect category classification
- Severity selection
- Corrective action documentation
- Inspection status tracking

### 4. Automated Failed Inspection Alerts

Power Automate is configured to:
- Trigger when a Dataverse row is added, modified, or deleted.
- Evaluate the inspection result.
- Identify failed inspections.
- Send an email notification through Microsoft Outlook.

### 5. Centralized Data Management

Microsoft Dataverse stores inspection records and related information, supporting structured data management.

## Dataverse Structure

| Column | Data Type |
|---|---|
| InspectionResult | Choice |
| DefectCategory | Choice |
| Severity | Choice |
| CorrectiveAction | Multiple lines of text |
| InspectionStatus | Choice |
| Remarks | Multiple lines of text |

## Workflow

1. Inspector enters equipment inspection information.
2. Inspection details are stored in Dataverse.
3. Power Automate monitors Dataverse records.
4. The inspection result is evaluated.
5. If the result is Fail, an automated email alert is sent.
6. Quality personnel can review the defect and corrective action.

## Project Status

Core data structure and failed-inspection notification workflow have been configured. Further development and validation of the application are ongoing.

## Future Enhancements

- Power BI quality inspection dashboards
- Defect trend analysis
- Equipment-wise inspection reports
- Role-based access management
- Advanced corrective action tracking

## Author

Developed as a Microsoft Power Platform project to demonstrate low-code application development, data management, and workflow automation.

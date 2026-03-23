# Purview Sensitivity Label Framework for Healthcare
### Microsoft Purview Portfolio | Luis Macias

## Scenario
Regional Health System (RHS) is a mid-sized non-profit health system headquartered in the Midwest. It operates 3 acute care hospitals totaling 850 licensed beds, 14 outpatient specialty clinics across 4 counties, and an academic medical center with a university research division that has data sharing agreements with 2 European academic partners in the Netherlands and Germany.

RHS employs 4,200 staff including 620 physicians, 1,400 nurses and clinical staff, 280 administrative staff, and 320 corporate and support staff. All staff operate within a single Microsoft 365 E5 tenant. The IT environment includes 47 active SharePoint site collections, 312 active Teams, and all mailboxes in Exchange Online. Microsoft Intune is deployed to corporate laptops. BYOD is not permitted for clinical staff.

Current Purview state at time of engagement: no sensitivity labels configured, unified audit log disabled, no DLP policies, no retention policies.

Phase 1 scope: design and deploy a sensitivity label framework that addresses all three findings within a 3-week delivery window. Phases 2 and 3 cover DLP policies, retention labels, and insider risk configuration and are out of scope for this project.

## Deliverables
- Sensitivity label taxonomy aligned to HIPAA, HITECH, HITRUST r2, NIST CSF 2.0, and ISO 27001
- All labels deployed and published to the correct Azure AD groups
- Service-side auto-labeling policy validated in simulation mode against RHS content
- Container labels enforcing privacy and external sharing controls on clinical Teams and SharePoint sites
- Access control matrix documenting each group's permissions, justification, and review cadence
- Configuration evidence package suitable for the OCR audit response and HITRUST assessment

## What Was Built
- Created and setup the proper AD security groups in Entra
- Sensitivity labels and sublabels adhering to the relevant compliance frameworks

## Label Hierarchy
[write out of full label list in the Purview portal]
See /screenshots folder
## Key Configurations
- X sensitivity labels across Y levels
- Auto-labeling configured for PHI data types
- Mandatory labeling enforced via two scoped policies
- Container labels applied to Teams and SharePoint sites

## Design Decisions
[Section 3.2]

## Compliance Framework
HIPAA, PHI DSS, HITRUST CSF r2, ISO 27001

## Environment
Microsoft 365 E5 Developer Tenant

## Screenshots
See /screenshots folder

## Author
Luis Macias

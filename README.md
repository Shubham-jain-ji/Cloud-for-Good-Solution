# Cloud-for-Good-Solution
Volunteer Program Management Solution
Salesforce CFG_Shubham - Volunteer Management Solution (CFG Case Study) Overview
Salesforce CFG_Shubham is a point-and-click Volunteer Management Solution tailored for Nonprofit Cloud (NPSP), designed in alignment with OmniStudio CFG Case Study.
It allows Experience Cloud users (Volunteers) to browse volunteer opportunities, select appropriate shifts, and register - all with built-in eligibility validation and confirmation notifications.
The solution leverages the Salesforce Volunteer Management (VMS) data model and OmniStudio tools to provide a streamlined user experience within Experience Cloud.

Included Components
Salesforce Metadata
Custom fields and record types added to standard NPSP/Volunteer objects


Configured page layouts and compact layouts


A dedicated custom Volunteer Management app


OmniStudio Assets
FlexCards: Present available volunteer programs and shifts


OmniScripts: Step-by-step registration process


Integration Procedures / DataRaptors: Retrieve and create volunteer-related records


OmniStudio Functions: Perform eligibility checks (e.g., minimum age, required training)


Experience Cloud Configuration
A public portal for volunteers to browse and register for the event


Custom branding and site navigation


OmniStudio components embedded in Experience Cloud pages


Apex Code
Utility classes to handle data operations and eligibility logic


Support classes for Integration Procedures, if needed



Prerequisites Before Deployment
Ensure the following are set up in the target Salesforce org:
OmniStudio Managed Package is installed (from AppExchange or internal link)


OmniStudio Metadata API is enabled
 → Go to: Setup → OmniStudio Settings → Enable OmniStudio Metadata API


Experience Cloud is enabled with at least one live site



Deployment Workflow
1. Metadata Deployment
 Install custom fields, record types, and page layouts for Volunteer objects.
 Check API names and field-level security settings.
2. App Deployment
 Deploy the Salesforce CFG_Shubham custom application for managing volunteers.
3. Apex Classes Deployment
 Push all relevant Apex classes for processing logic and eligibility validation.
 Ensure they compile successfully post-deployment.
4. OmniStudio Component Deployment
 Deploy FlexCards, OmniScripts, DataRaptors, and Integration Procedures.
 Confirm all dependencies are resolved.
5. Profile Setup
 Deploy profiles for System Admin and Experience Users.
 Verify correct access to objects, fields, and OmniStudio tools.
6. Experience Cloud Site Deployment
 Push site metadata including network, site, and experienceBundle.
 Ensure site branding and domain settings are correct.
7. Activate OmniStudio Components
 Open each OmniScript and click Activate
 Open each FlexCard, then Activate & Publish
8. Publish the Experience Site
 From Experience Builder, click Publish
 Check that all OmniStudio components display as expected for users

Post-Deployment Checklist
Login as an Experience (Volunteer) user and:
Go to the Volunteer Opportunities page


Confirm available shifts and programs are visible


Test the "Apply to Volunteer" button → OmniScript should launch


Ensure eligibility checks work, and registration completes


FlexCard should refresh to display a success message



Additional Notes
If using Customer Community Plus licenses, you may need a custom object (Program__c) to replicate Campaign data


Set Integration Procedures to run in System Context to avoid sharing rule conflicts


All OmniStudio components must use LWC Runtime for compatibility


Always Activate OmniScripts and Publish FlexCards post-deployment



Version Details
Author: Shubham Jain


Project: Salesforce CFG_Shubham - CFG Volunteer Program Management Solution


Version: 1.0


Date: October 2025

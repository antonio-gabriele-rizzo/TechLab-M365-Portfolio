# SharePoint

## Overview

This project demonstrates the creation and administration of a SharePoint Online Team Site within Microsoft 365. The exercise covered site creation, document libraries, folder management, document storage, permissions, sharing controls, version history, and troubleshooting.

## Objectives

- Create a SharePoint Team Site
- Understand the difference between Team Sites and Communication Sites
- Create and manage a Document Library
- Organise content using folders
- Upload and manage documents
- Configure site membership
- Review permissions and sharing controls
- Explore version history
- Troubleshoot common SharePoint issues

---

## Accessing SharePoint

Locating SharePoint was not immediately obvious through the Microsoft 365 Admin Center navigation menu.

The most reliable method was:

1. Open Microsoft 365 Admin Center.
2. Use the search bar at the top of the page.
3. Search for **SharePoint**.
4. Open the SharePoint application.

### Observation

Using the search bar proved more reliable than navigating through the Admin Centers menu.

### Screenshot

- `sharepoint-start-page.png`

---

## Troubleshooting: SharePoint Admin Center

When attempting to open the SharePoint Admin Center, an error was displayed.

Despite the Admin Center error, SharePoint Online itself remained fully operational and accessible through the SharePoint application.

### Learning Point

```text
Admin Center unavailable
≠
SharePoint unavailable
```

Administrative portals and services should be tested independently during troubleshooting.

---

## Team Site vs Communication Site

SharePoint provides multiple site types.

| Team Site | Communication Site |
|------------|------------|
| Designed for collaboration | Designed for information sharing |
| Supports team document management | Supports news and announcements |
| Connected to Microsoft 365 Groups | Usually managed by content publishers |
| Members actively contribute content | Primarily used to distribute information |
| Suitable for departments and project teams | Suitable for intranet and corporate communication |

### Why a Team Site Was Chosen

A Team Site was selected because the objective was to demonstrate:

- Document Libraries
- Folder Structures
- Permissions
- Sharing Controls
- Collaboration

---

## Creating the Team Site

A Team Site was created using the Standard Team template.

### Configuration

| Setting | Value |
|----------|----------|
| Site Name | Company Documents |
| Description | SharePoint Team Site created for Project 5 – SharePoint administration |
| Privacy | Private |
| Template | Standard Team |

### Screenshot

- `create-team-site.png`

---

## Site Membership

The following users were added during site creation:

### Members

- John Smith
- Sarah Jones

### Screenshots

- `add-site-members.png`
- `team-site-created.png`

---

## Troubleshooting: User Membership Issue

During Team Site creation, Sarah Jones could not initially be added as a site member.

Investigation revealed that the account had **Blocked Sign-In** enabled from a previous user administration exercise.

After restoring sign-in access, Sarah Jones became available for selection and was successfully added to the site.

### Learning Point

When users cannot be added to Microsoft 365 resources, account status should be verified before investigating service-specific issues.

---

## Document Library

The default SharePoint Document Library was used to store organisational content.

A SharePoint Document Library provides:

- Centralised file storage
- Web-based access
- Permissions integration
- Collaboration capabilities
- Version management

### Screenshot

- `document-library.png`

---

## Folder Structure

A departmental folder structure was created.

```text
Documents
│
├── HR
├── Finance
└── Operations
```

### Screenshot

- `folder-structure.png`

---

## Document Creation and Storage

A sample document was created within the HR folder.

### Document

`Employee-Handbook.docx`

### Initial Content

```text
Sample HR document for SharePoint Project 5.
```

### Screenshot

- `document-uploaded.png`

---

## Auto-Save Functionality

The document was created using Word Online.

After renaming the file and adding content, changes were automatically saved to SharePoint without requiring manual intervention.

### Benefits

- Reduced risk of data loss
- Real-time collaboration
- Automatic version creation
- Cloud-based document storage

---

## Version History

The Employee-Handbook document was edited multiple times.

SharePoint automatically generated:

- Version 1.0
- Version 2.0
- Version 3.0

Version History recorded:

- Modification date and time
- User responsible for the change
- File size changes
- Previous document versions

### Screenshot

- `version-history.png`

### Learning Point

Version History allows organisations to:

- Audit document changes
- Restore previous versions
- Recover from accidental edits
- Track document development over time

---

## Permissions and Sharing Controls

Site permissions were reviewed through the SharePoint permissions interface.

### Site Owners

- Company Documents Owners
- Full Control permissions

### Site Members

- Company Documents Members
- Edit permissions

### Site Visitors

- No visitors configured

### Sharing Controls

The permissions page also provided controls for managing how members can share content and collaborate within the site.

### Screenshot

- `site-permissions.png`

---

## Troubleshooting: Site Visibility

After the Team Site was created, it did not immediately appear in the SharePoint Recent Sites list.

The site was verified through:

- Direct access
- Site Information settings
- Membership configuration

After further interaction with the site, it eventually appeared in Recent Sites.

### Learning Point

The Recent Sites view should be treated as a convenience feature rather than a complete inventory of available SharePoint sites.

---

## Reopening an Existing Site

Several methods were tested for reopening the Team Site.

### Methods Used

1. SharePoint application from the Microsoft 365 App Launcher.
2. SharePoint Recent Sites.
3. Direct site URL.
4. Site Information verification.

### Observation

Understanding multiple navigation paths is important because users may not always find sites immediately through Recent Sites.

---

## Skills Demonstrated

- SharePoint Online administration
- Team Site creation
- Microsoft 365 integration
- Site membership management
- Document Library administration
- Folder structure design
- Document management
- Version History management
- Permissions management
- Sharing control review
- Troubleshooting and problem solving

---

## Screenshots

- `sharepoint-start-page.png`
- `create-team-site.png`
- `add-site-members.png`
- `team-site-created.png`
- `document-library.png`
- `folder-structure.png`
- `document-uploaded.png`
- `version-history.png`
- `site-permissions.png`

---

## Conclusion

This project demonstrated the deployment and administration of a SharePoint Online Team Site. Key activities included site creation, membership management, document organisation, document storage, permissions review, version management, and troubleshooting. The exercise provided practical experience with SharePoint Online and its integration within the Microsoft 365 ecosystem.

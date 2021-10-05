---
title: Data dictionary
nav_order: 5
---

# Data dictionary

This page contains details about what information is available for developments and components in the Development Pipeline Data Inspector.

## Developments

The development records provide a small amount of information about each development in the region. CMAP currently only tracks developments that consume at least one acre of land *OR* consist of at least 10 residential units *OR* consist of 10,000 square feet of non-residential space. Additionally, only expansions, new construction, and renovations with a change in land use are tracked (so, for example, condo-to-apartment conversions or vice versa are *not* included).

| **Attribute Name** | **Description**                                              |
| ------------------ | ------------------------------------------------------------ |
| Development ID     | A unique numeric development identifier assigned to each development by CMAP |
| Development Name   | The name of the development                                  |
| Primary Developer  | The name of the developer responsible for the project        |
| Municipality       | The community in which the development is located            |
| Acreage            | The acreage of the entire development (including all components) |
| Former Use         | For redevelopment projects, the land use of the prior development that is being replaced |
| Notes              | Miscellaneous information about the project added by CMAP staff |
| Corrections?       | A user-editable field for [submitting corrections](./submitting-corrections.html) to CMAP when inaccurate information about a development is discovered |

## Components

CMAP divides developments into distinct components, with land use and phasing being the primary differentiators. The component records contain the bulk of the information that CMAP tracks for a given development. Many smaller developments have only a single component, but all of them have at least one, and larger developments may have many.

| **Attribute Name**  | **Description**                                              |
| ------------------- | ------------------------------------------------------------ |
| Component ID        | A unique numeric development identifier assigned to each component by CMAP |
| Component Name      | The name of the component. (When a component doesn’t have an official name, such as a phase, this will often be either an address range or a description of the component’s land use.) |
| Development ID      | The unique numeric ID of the overarching development         |
| Development Name    | The name of the overarching development                      |
| Address             | The street address or intersection of the component          |
| Municipality        | The community in which the overarching development is located |
| Action              | Development action for the component. Possible values:<br />- **New Construction**<br />- **Rehab**<br />- **Rehab - New Use**<br />- **Rehab & Expand**<br />- **Rehab & Expand - New Use**<br />- **Expansion** |
| Land Use            | Detailed land use classification for the component. Possible values:<br />- **Airport**<br/>- **Auto**<br/>- **Business Park**<br/>- **Church**<br/>- **Commercial**<br/>- **Congregate Housing**<br/>- **Distribution**<br/>- **Energy Utility**<br/>- **Entertainment**<br/>- **Fleet Maintenance**<br/>- **Golf**<br/>- **Government**<br/>- **Hospital**<br/>- **Hotel**<br/>- **Industrial**<br/>- **Manufacturing**<br/>- **Marina**<br/>- **Mobile Homes**<br/>- **Multi Family**<br/>- **Nonhospital Medical**<br/>- **Nursing Home**<br/>- **Office**<br/>- **Open Space**<br/>- **Parcel Distribution**<br/>- **Parking**<br/>- **Public Library**<br/>- **Public Storage**<br/>- **Recreation**<br/>- **Research**<br/>- **Residential General**<br/>- **Retail**<br/>- **School**<br/>- **Shopping Center**<br/>- **Single Family Attached**<br/>- **Single Family Detached**<br/>- **Social Service**<br/>- **Transit Station**<br/>- **Warehouse**<br/>- **Water Treatment** |
| Major Land Use      | Generalized land use classification for the component. Possible values:<br />- **Commercial**<br />- **Residential**<br />- **Industrial**<br />- **Institutional**<br />- **Medical**<br />- **Recreation**<br />- **Transportation**<br />- **Open Space**<br />- **Utilities** |
| Square Footage      | Square footage of the component                              |
| Units               | Used for residential and hotel land uses. Total housing units (or hotel rooms) in the component. |
| Rental Units?       | Will the housing units in a residential component be rentals? |
| Age-Targeted Units? | Will the housing units in a residential component be age-targeted? |
| Construction Start  | Date on which component’s construction began, if known       |
| Construction End    | Date on which component’s construction concluded, if known   |
| Notes               | Miscellaneous notes from CMAP staff about the component in general |
| Known Status        | The most recent known status of the development. Possible values:<br />- **Proposed**: formal proposal presented to municipal board<br/>- **Committed**: village board/elected authority (not plan commission) has approved<br/>- **Under Construction**: ground has been broken on component<br/>- **Open**: primarily for residential components, when a number of houses have been completed but not all<br/>- **Completed**: construction completed and open to public<br/>- **Suspended**: development activity has stalled but has not yet been abandoned |
| Status Date         | Date on which *Known Status* was updated                     |
| Completed Units     | Number of housing units in a residential component that had been built as of *Status Date* |
| Status Notes        | Miscellaneous notes from CMAP staff pertaining in particular to the most recent *Known Status* |
| Corrections?        | A user-editable field for [submitting corrections](./submitting-corrections.html) to CMAP when inaccurate information about a component is discovered |


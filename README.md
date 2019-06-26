# PWS to Water Sources

## Context
The State Water Board’s Division of Drinking Water (DDW) regulates approximately 7,500 public water systems (PWS) in California. A PWS is defined as a system that provides drinking water for human consumption to 15 or more connections or regularly serves 25 or more people daily for at least 60 days out of the year. The DDW allocates permits for PWS, and collects an annual report from each system.

## Problem
Although each PWS has a unique identifier (PWSID), the current or former sources(s) of water each system uses are not as easy to identify. The full PS Code includes the sampling location within the system, not the source identification (well, etc.). 

Often, the water source(s) are not simply just “upstream” of or within their boundaries, and in some cases we don’t even know the exact location of the source. The DDW would like the ability to select a location within a PWS boundary and see which current and past sources of water are utilized (think time machine for source water data).

## Resources
What is a public water system? Find out here: https://www.waterboards.ca.gov/drinking_water/certlic/drinkingwater/documents/waterpartnerships/what_is_a_public_water_sys.pdf

This project will build new datasets or share tools used to integrate source data with PWS facility information found here: https://data.ca.gov/dataset/drinking-water-public-water-system-information

Some of our Public Water Systems (about 300 out of the 7500?) completed a stress test a few years ago and provided some detailed information as a result of that effort. The stress test submittals, as received, are posted with self-certification material; the pinpoint link to compiled submittals is here: https://www.waterboards.ca.gov/water_issues/programs/conservation_portal/docs/emergency_reg/uw_self-cert_submittals.xlsx  

If you go into that worksheet and find Column X you see a clickable link the field: click on Column X link and get something like this…
https://drinc.ca.gov/DNN/Portals/0/SelfCert/63457002-98f4-4482-9b89-31fcd43234da.xlsx

SFPUC is a wholesaler, so someone may have to figure out some other way where thie wholesaler gets their water from. Looking up the wholesaler ID in SDWIS reveals this: https://sdwis.waterboards.ca.gov/PDWW/JSP/WaterSystemDetail.jsp?tinwsys_is_number=13798&tinwsys_st_code=CA&wsnumber=CA3810008

The self-certification material section contains a link to a PDF Wholesale Urban Water Supplier Web Addresses that points to the information wholesalers submitted to us under the emergency regulation.  Hopefully this is what you are looking for.  For instance, Zone 7 information should be here: http://www.zone7water.com/index.php/conservation-rebates/water-conservation/36-public/content/203-drought 

The wholesaler files may have been posted on the DRINC portal before transition from the DDN platform; we asked all those files to be ported over to the new .net platform. Unfortunately, there may still be some links that point to DNN files.

Here is the raw PWS facility info to be integrated with source data/information: https://data.ca.gov/dataset/drinking-water-public-water-system-information/resource/0f7743e9-2777-4bbe-a3d4-fe4c9a704c18#{view-graph:{graphOptions:{hooks:{processOffset:{},bindEvents:{}}}},graphOptions:{hooks:{processOffset:{},bindEvents:{}}}}

This paper has some LA water sources: https://www.tandfonline.com/doi/full/10.1080/17445647.2018.1473815
 
Visualizing water infrastructure with Sankey maps: a case study of mapping the Los Angeles Aqueduct, California: Journal of Maps: Vol 14, No 1: www.tandfonline.com
- Creating resilience for urban water supply systems requires innovative thematic visualizations of the interface between infrastructure, ecology, and culture to viscerally engage lay audiences in the policy making process. Sankey maps (a hybrid Sankey diagram/flow map) embed the systemic accounting ...

Internet wayback machine: https://web.archive.org/

## 2019 California Water Boards Science Symposium: Water Science Datathon
### Challenge Questions
DATA MODEL: 
- What information is needed to make decisions about where water comes from?
- Surface water vs. groundwater
- How are sources identified?
- How do we assign unique IDs to sources? 
- Do we know where all sources are?
- What sources of data are available to track current and former water sources? 
- How do we link these datasets? 
- What information do we need to move forward?

INTERFACE: 
- What would the interface look like?
- What features would it have? 
- What would it be able to tell the user? 
- How would it communicate results (graphics, figures, tables, maps, text)?

### Potential Challenge Tasks
Develop list of relevant datasets

Add to or revise the Berkeley Discovery Research Student data model. 
- Develop a list of elements to add, and how to link them to the rest of the data model. 
- Develop a list of elements to remove from data model, if necessary. 
- Define organization, relationships, and dependencies among data elements.

Develop a list of data gaps. What data do we need to move forward on this project? E.g. Missing well locations for X wells., Location and well ID mismatched for X wells.

Provide an update on the project. How far did you get? What challenges did you face? How did you overcome these challenges or what do you need to do so?

### Relevant Datasets/Resources
- https://data.ca.gov/dataset/drinking-water-public-water-system-information
- https://data.ca.gov/dataset/drinking-water-laboratory-water-quality-results
- https://data.ca.gov/dataset/drinking-water-public-water-system-annually-reported-water-production-and-delivery
- https://dev.trackingcalifornia.org/water-systems/water-systems-landing
- UC Berkeley Spring 2019 PWS Project (also see uploaded files in UC Berkeley Project Folder): https://github.com/richardnnn/PWS_Water_Integration
- UC Berkeley Spring 2019 Scraping SDWIS Project: https://gist.github.com/fndari/963ce91659950a8b64e833ca004f3f79


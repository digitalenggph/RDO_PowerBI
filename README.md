# RDO_Viz_Rizz 🗺️🍰
Hola! 👋🙋‍♀️ <br>
This repository serves as a mini-documentation of my experimental dashboard for BIR RDO (Regional District Offices) in the Philippines. <br>
As per BIR's website, RDO's general function is as follows: 

> Administers and enforces internal revenue laws including the assessment and collection of all internal revenue taxes, charges and fees from taxpayers within the region's jurisdiction, as well as ensures proper and effective implementation of National Office's policies and programs within the Regional Office.

In my POV, this is where you pay your taxes.

## The inspiration 🌈🌈
I had two employees last fiscal year of 2023 so I have to file for my own BIR Form 1700. <br>
So if you are like me and you had more than one employer in the previous year, then you must file your own ITR (BIR form 1700). <br>

I am not an accountant so I am not going to elaborate the taxation part haha. <br>
But after following both my company and BIR guidelines, I discovered I have tax dues oh noeeess. Here are some tools I used. <br>
> This is where I downloaded the e-BIR form app: https://www.bir.gov.ph/index.php/eservices/ebirforms.html <br>

Look for this as you are not going to see a download bar. <br>
> ![image](https://github.com/digitalenggph/RDO_PowerBI/assets/101250873/ee8c5651-ee3f-4e3a-855e-d92054000166)

In addition, I'd like to quote this blog that also cites a BIR memorandum (Revenue Memorandum Order No. 37-2019) regarding which RDO you should be in.
> https://sprout.ph/blog/onboarding-101-employee-registration-philippines-2023/

My case falls under case II.7. Have a read on it (it's on the link) 😉 <br>
It states that my RDO should be where my place of residence is. <br>

To cut the personal anecdote short, I have to pay this, but do not know exactly where I should process this kind of stuff. <br>
Hence, my quest for RDO office mapping begins. <br>

## What I visualized



## Sources used:
 Here are some data that I used:  <br>
 
**RAW DATA:**
| Data                  | Type of source          | Link                                                                                              |    
| --------------------- | ----------------------- | ------------------------------------------------------------------------------------------------- |
| RDO offices list      | Website                 | https://www.bir.gov.ph/index.php/zonal-values.html                                                |
| RDO offices address   | Website                 | https://www.bir.gov.ph/index.php/contact-us/directory/regional-district-offices.html#22162        |
| RDO offices latlon    | Website                 | https://www.google.com/maps/                                                                      |
| Philippine shp file   | shapefile               | https://github.com/altcoder/philippines-psgc-shapefiles                                           | <!--Just updated super recently may need to check sometime-->


**PROCESSED DATA:**
| Data                  | Type of source          | Link                                                                                              |    
| --------------------- | ----------------------- | ------------------------------------------------------------------------------------------------- |
| RDO offices info      | geojson                 | [DS_rdo_latlon](https://github.com/digitalenggph/RDO_PowerBI/blob/main/DS_rdo_latlon.geojson)     |     
| RDO X shp file        | geojson                 | [RDO_jurisdiction_simplified](https://github.com/digitalenggph/RDO_PowerBI/blob/main/RDO_jurisdiction_simplified.json)  /   [RDO_jurisdiction_metros](https://github.com/digitalenggph/RDO_PowerBI/blob/main/RDO_jurisdiction_metros.geojson)   |

## Tools used:


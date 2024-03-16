# [RDO_Viz_Rizz](https://app.powerbi.com/view?r=eyJrIjoiNWQzZTA4OWItZmRlZi00ZGZlLWE3NjMtNTdlMWYwYWQyZTM5IiwidCI6ImJkMDNhNzM1LTJhYTMtNGNjYS05NzIyLTJhZTQ5MjlhYjNlYyIsImMiOjEwfQ%3D%3D) 🗺️🍰
Hola! 👋🙋‍♀️ <br>
This repository serves as a mini-documentation of my experimental dashboard for BIR RDO (Regional District Offices) in the Philippines. <br>
As per BIR's website, RDO's general function is as follows: 

> Administers and enforces internal revenue laws including the assessment and collection of all internal revenue taxes, charges and fees from taxpayers within the region's jurisdiction, as well as ensures proper and effective implementation of National Office's policies and programs within the Regional Office.

In my POV, this is where you pay your taxes. Cha-ching! 💸💸💸

## The inspiration 🌈🌈
I had two employees last fiscal year of 2023 so I have to file my BIR Form 1700. <br>
So if you are like me and you had more than one employer in the previous year, then you must file your own ITR (BIR form 1700). <br>

I am not an accountant so I am not going to elaborate the taxation part haha. <br>
But after following both my company and BIR guidelines, I discovered I have tax dues oh noeeess. Here are some tools I used. <br>
> This is where I downloaded the e-BIR form app: https://www.bir.gov.ph/index.php/eservices/ebirforms.html <br>

Look for this as you are not going to see a download bar ⏸️. <br>
> ![image](https://github.com/digitalenggph/RDO_PowerBI/assets/101250873/ee8c5651-ee3f-4e3a-855e-d92054000166)

In addition, I'd like to quote this blog that also cites a BIR memorandum (Revenue Memorandum Order No. 37-2019) regarding which RDO you should be in.
> https://sprout.ph/blog/onboarding-101-employee-registration-philippines-2023/

My case falls under case II.7. Have a read on it (it's on the link) 😉 <br>
It states that my RDO should be where my place of residence is. <br>

To cut the personal anecdote short, I have to pay this tax dues 🥹, but do not know exactly where I should process this kind of stuff. <br>
Hence, my quest 🚵‍♀️🚵‍♀️ for RDO office mapping 📌 begins. <br>

## How it should be used:
So open the dashboard that is in this [link](https://app.powerbi.com/view?r=eyJrIjoiNWQzZTA4OWItZmRlZi00ZGZlLWE3NjMtNTdlMWYwYWQyZTM5IiwidCI6ImJkMDNhNzM1LTJhYTMtNGNjYS05NzIyLTJhZTQ5MjlhYjNlYyIsImMiOjEwfQ%3D%3D). <br>
You may also click the first line of this documentation if you want :) 

Users who will find this useful are: 
* Fellas like me who has transferred to new job or planning hahahhaha (mostly employees or freelancers, for business peepz - dunno)
* Curious people :'> 

Best way to use it is to search your barangay in the dedicated search bar especially if you are living in crowded areas aka Metro Cities 🚇 (NCR, Cebu City, and Davao City). <br>
![image](https://github.com/digitalenggph/RDO_PowerBI/assets/101250873/917550d2-5817-4ada-9256-f28ffd6b7ca3)

If you live in a chill place, say Tagaytay or Palawan then you can still search for your barangay or you can try searching for your province/municipality instead 🗾 <br>
![image](https://github.com/digitalenggph/RDO_PowerBI/assets/101250873/52f66b6e-1c5c-43e2-bcbe-90064658be90)


The dashboard should show you the RDO of that barangay is office location. <br>
So....click away! 🔘🔼🔽✅🔳🔲


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
🌍 QGIS - this is where I processed the shapefiles aka the clickable polygons you see in the dashboard. <br>
🈸 PowerBI - its where I load and transform my data to that very interactive dashboard you saw :D Comes with tons of visualization tools! <br>
🗺️ [Mapshaper](https://mapshaper.org/) - geojson file output from QGIS can be bloated if the boundaries are 'too exact' so I used the simplified function of this tool to **compress** the geojson file since free GitHub accounts only allows 25MB file size per file hihi. <br>
📌 [Mapbox](https://www.mapbox.com/) - free stuff again! I stored my basemap here that contains the 📍 pin locations of the offices.

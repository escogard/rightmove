# RightMove Scrapper
rightmove.co.uk is one of the leading rent and sale property listing websites in the UK.

Here you will find some simple scripts that will retrieve properties for rent or sale based on a defined area. 
The data will be saved in .xlsx (excel format)

## Instructions
### Add location(s) to search
* Create a locations_dict.py file
* In locations_dict.py create a dictionary "boroughs" that has any name descriptor as key and the area identifier from rightmoves's URL as value<img width="1187" alt="RM_location_dict_py_file" src="https://user-images.githubusercontent.com/49518098/114043496-407a7300-987e-11eb-9744-34f43e8c2493.png">
  * The area indetifier can be found in rightmove's URL after you make a property search
  * e.g
    * https://www.rightmove.co.uk/property-for-sale/map.html?areaSizeUnit=sqft&channel=BUY&currencyCode=GBP&locationIdentifier=USERDEFINEDAREA%5E%7B%22polylines%22%3A%22whkyHnrf%40oKugAnr%40sZlJha%40%7CH~l%40ky%40%7C%5E_A%7DJ%22%7D&mustHave=&propertyTypes=&radius=0.0&sortType=2&viewType=MAP
    * Copy everything from "locationIdentifier" until the next "&". 
    * _LocationIdentifier=USERDEFINEDAREA%5E%7B%22polylines%22%3A%22whkyHnrf%40oKugAnr%40sZlJha%40%7CH~l%40ky%40%7C%5E_A%7DJ%22%7D_

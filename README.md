# HousingDataClean
## Nashville Housing: SQL Data Cleaning 
Nashville Housing company needs their data cleaned and organized, to have clearer data on their customers they have sold homes to. So they can expand on company services. 

<img src="cd_img/SQLHousing1.png" width="600">
Software used: 

<li>Microsoft Excel: Dataset file to import into SQL Server. 
<li>Microsoft SQL Server: To clean the data. 

Standardize Date Format

<img src="cd_img/housingDcv.png" width="600">
  <br>
 The date was with the time, so I removed the time part and just keep the date.
 
Populate Property Address data
  
<img src="cd_img/populateAdd.png" width="600">
<br>
There was two parcel ids, two property addresses and one unique id. The null property address will combine with a newly created column of the property addresses that don’t contain more than one of each. Next to join to the original property address and this will create an updated version of property address with only one unique id each.

Breaking out Address into Individual Columns (Address, City, State)

Break property addresses 
  
<img src="cd_img/breakadd.png" width="600">
 <br>
I used the substring and len methods to break up the property address.
  
Break the owner address.
  
<img src="cd_img/breakoadd.png" width="600">
 <br>
I used the parsename and replace methods. 


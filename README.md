# NetSuite Sublist Update using Boomi

## Problem Statement:
When we perform Create/Update/Upsert operation in a NetSuite object such as Invoice/SalesOrder, which has sublist fields like AddressList/ItemList/InventoryList, we may encounter an error like - "Adding new line to sublist item is not allowed".
This error occurs when we send values to a few fields/elements of the sublist instead of sending values to all the fields/elements of that sublist.

## Resolution:
Add value of "FALSE" in "@replaceAll" attribute of the field AddressList/ItemList/InventoryList, as per below screenshot. 

![image](https://user-images.githubusercontent.com/12267939/177548220-d49bf19a-cbd7-4f91-81c0-db76063c5177.png)

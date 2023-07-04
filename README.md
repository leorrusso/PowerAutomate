# Power Automate - SharePoint HTTP requests

## Get Items
### Method: Get
### Use ?$select= to get the desired columns
>_api/web/lists/getbytitle('ListName')/items?$select=ID,Title

### Use top=30 to get the first 30 items
>_api/web/lists/getbytitle('ListName')/items?$top=30&$select=ID,Title

### Use the following header to get rid of metadata
>{
  "Content-Type": "application/json;odata=nometadata",
  "Accept": "application/json; odata=nometadata"
}

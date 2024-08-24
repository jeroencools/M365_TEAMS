



### edu_parents.ps1

This script updates the "related contacts" based on the information from a csv-file (data.csv). 
Default value for relationship = "parent" - choosing another relationship value is currently WIP

### Working with:
 * 1.19.0               Microsoft.Graph

### Some extra information:
* GRAPH: https://learn.microsoft.com/en-us/powershell/microsoftgraph/get-started?view=graph-powershell-1.0
* https://learn.microsoft.com/en-us/graph/api/relatedcontact-update?view=graph-rest-beta&tabs=http
* https://learn.microsoft.com/en-us/graph/api/resources/relatedcontact?view=graph-rest-1.0


### data.csv

7  headers: UPN,rc1name,rc1phone,rc1mail,rc2name,rc2phone,rc2mail

* UPN = UPN of user
* rc1name = Display name for related contact 1
* rc1phone = Phone number for related contact 1
* rc1mail = mail for related contact 1
* rc2name = Display name for related contact 2
* rc2phone = Phone number for related contact 2
* rc2mail = mail for related contact 2





### edu_parents_gui.ps1

### TO DO
* add the function to choose how many related contacts an edu user has (1, 2, 3 ...)

### Working with:
 * 1.19.0               Microsoft.Graph

### Some extra information:
* GRAPH https://learn.microsoft.com/en-us/powershell/microsoftgraph/get-started?view=graph-powershell-1.0
* https://learn.microsoft.com/en-us/graph/api/relatedcontact-update?view=graph-rest-beta&tabs=http
* https://learn.microsoft.com/en-us/graph/api/resources/relatedcontact?view=graph-rest-1.0


![GUI - parents](https://user-images.githubusercontent.com/113233490/211123292-a0d21d54-93b6-4ef5-9648-99877e2f0acf.PNG)


By executing this file, you will open a simple GUI. This will allow you to search for an edu user in your tenant by providing the email address. The tool will then search for the corresponding information of the related contacts of that user. You can adjust the information and then update it. Sometimes it can take a while before the adjustments become visible in the parents app. You can adjust the display name, email address, phone number and relationship.

!!! Only "parent" and "guardian" selections will be visible in the parents app within Teams. Other selections will not work at the moment. See: https://learn.microsoft.com/en-us/MicrosoftTeams/edu-parents-app  However, it is possible they will become available in the future, so these values are already added in this tool. See: https://learn.microsoft.com/en-us/graph/api/resources/relatedcontact?view=graph-rest-beta


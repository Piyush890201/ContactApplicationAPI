
# Contact Application 
Contact application - simple .Net core Web Api for managing contacts using .Net core Web API and EntityframeworkCore ans SQL server as database


## Database Setup

```bash
Run command using Package Manger console 

Add-Migration -Context ContactWebAPI.Data.ContactDbContext -Name ContactInfo

update-database

above commands will generate DB at localMSSQLSERVER
```

# Run API using postman tool

# Add Contact
```bash
https://localhost:443/api/Contact/AddContact -  

adding conatct need to provide details in body in Json format
Input parameter
{
	"FirstName":"Piyush",
	"LastName":"Bhole",
	"Email":"Piyush.Bhole@gmail.com",
	"ContactNumber":"9890398207"
}
```
# List Contacts
```bash
https://localhost:443/api/Contact/GetAllContacts

```
# Get a Contact
```bash
https://localhost:443/api/Contact/GetContact?criteria=9890398207 -

fetching a conatct need to provide details in body in Json format
passing parameter criteria and value either FirstName or ContactNumber or Email
```
# Edit Contact
```bash
https://localhost:443/api/Contact/UpdateContact-

update conatct need to provide details in body in Json format
{
	"FirstName":"Piyush",
	"LastName":"Bhole",
	"Email":"Piyush.Bhole@gmail.com",
	"ContactNumber":"9890398207"
}
```
# Delete Contact
```bash
https://localhost:443/api/Contact/DeleteContact?criteria=9890398207 - 

Delete conatct need to provide details in body in Json format
passing parameter criteria and value either FirstName or ContactNumber or Email
```


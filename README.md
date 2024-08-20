Spataro-App
=
---
It is an application which aims to relay the drivers' route sheets to the boss, so that he can receive them more easily.
-
A first version already exists, but it was done at the same time as my training on django, and I had difficulty finding my way as I progressed, here I will have a little more time to improve myself and do a little less code repetition.

---
### The main content to have the roadmaps

- [ ] Accounts
  - First name
  - Last name
  - Truck --> by data (*Trucks)
  - City
  - Email
  - Password
  - is delete
- [ ] Trucks
  - License plate
  - Brand
  - Model
  - Technical control
  - Tachograph
  - Maintenance
  - Adr validation
  - is delete
- [ ] Factory
  - Sector --> by data
  - Name
  - Address
  - Zip code
  - City
  - Country --> by data
  - GPS
  - Phone
  - Email
  - Hourly
  - Language
  - Specification
  - Factory plan
  - Description
  - is delete
- [ ] Station
  - Name
  - Address
  - Zip code
  - City
  - Country --> by data
  - is delete
- [ ] Roadmaps
  - Name driver --> by data (*Accounts)
  - Truck driver --> by data (*Accounts, *Trucks)
  - Trailer
  - Departure date
  - Departure time
  - Departure location
  - Starting kilometer
  - End date
  - End time
  - End location
  - End kilometer
  - Total hours --> by calculate (second)
  - Total kilometer --> by calculate
  - Dislodge --> by comparison (*To accounts city and end location)
- [ ] Haltings roadmaps
  - Name driver --> by data (*Accounts)
  - Name factory --> by data (*Factory - *Sector)
  - Date
  - Arrival time
  - Arrival kilometer
  - Start work
  - End work
  - Cmr
  - Order
  - Weight
  - Departure time
  - Noticed
- [ ] Fuel stop
  - Name driver --> by data (*Accounts)
  - Name station
  - Date
  - Arrival time
  - Arrival kilometer
  - Liter diesel
  - Liter blue
  - Departure time
- [ ] Change trailer
  - Name driver --> by data (*Accounts)
  - Name factory --> by data (*Factory - *Sector)
  - Date
  - Arrival time
  - New trailer --> add to trailer in roadmaps
  - Date technical control
  - If adr
    - Adr validity date
    - Code tank
  - Tire condition
  - State light
  - Departure time
  - Noticed
- [ ] Data center
  - Month year
  - Name driver --> by data (*Accounts)
  - Total kilometer
  - Total hours (second)
  - Total works (second)
  - Total weight
  - Total diesel
  - Total blue
  - Number day work
  - Number loading
  - Number unloading
  - Number change

> For the country and the sector, a database will be set up to be selected in the factory and station forms, all calculations will be done 
when saving the form as well as the comparison, finally for the data center, will be completed according to the data requested when saving 
the form for which the data is needed.

What is the page ?
-
- Base
- Navigation
- Accounts
  - Dashboard for user and staff (Index)
  - Signup/modify user and truck
  - Connection
  - Detail day
  - Profile
- Factory and station
  - List of factories and stations (Index)
  - Create/modify factory and station
  - Detail factory
- Roadmaps
  - Day (Index)
  - Create/modify roadmaps, halting, change, fuel



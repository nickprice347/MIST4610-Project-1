# MIST4610-Project-1

## Team Name: 
61608 Group 5 

## Team Members:

1. Nicholas Price [@nicholasprice](https://www.github.com/nickprice347)
2. Albert Sun [@albertsun](https://www.github.com/Glockgeta)
3. Haley Ford [@haleyford](https://www.github.com/HaleyFord)
4. Sydney Seid [@sydneyseid](https://www.github.com/sydneyseid)
5. Avanish Thota [@avanishthota](https://www.github.com/avanish-thota27)
6. Manafie Kabir [@manafiekabir](https://www.github.com/manafiekabir)

## Problem Description:

The current scenario involves creating a relational database for a tennis club to ensure all data is properly allocated, and the business runs smoothly and efficiently. The majority of the model is centered around the entity “Members”. Members are at the forefront of the business since they determine which transactions take place, what divisions and leagues to join, what courts to reserve in conjunction with the coaches, which coaching programs to be a part of, and more. In addition to members, the club also employs a variety of general staff employees who can fulfill maintenance requests on various courts. The goal of the model is to accurately use and generate data, show the relationships between the various entities, and allow for queries to promptly be asked and solved to easily allow the analysis of data.


## Explanation of our data model: 

![ourClientsResponseimage](https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/ac31fd9e-b18b-409f-bef1-92db0003b880)

*Numbers Match Up With Our Client’s Points*
Our model is structured around a tennis club and its various entities are representative of key daily functions. The members entity is a key aspect of our model, and therefore is present in multiple different relationships. 
& 2. 
Starting with entities one and two from our client, we created a many to many relationship between members and courts. Members can reserve many courts and courts can have multiple members present on them. The many to many relationship resulted in an associative entity, court reservations. 
3.
Next, members can belong to many coaching programs and coaching programs have multiple members present in them. These two entities form an associative entity, sessions. Coaching programs and members may also at times have no sessions. 
Additionally, the coaching programs are led by coaches. Coaches have a one to many relationship with coaching programs, as one coach can teach many coaching programs, but a coaching program can only be led by one coach at a time. 
Additionally, the coaches entity has a one to many relationship with the court reservation entity as a coach can make multiple court reservations, but a reservation can only belong to one coach.  
4. 
 Members can belong to many tennis leagues, and a tennis league is made up of many members. These two entities have a many to many relationship, which results to an associative entity divisions. 
5.
	The Pro Shop Inventory entity can belong to many transactions, and the transactions can consist of multiple pro shop items. These two entities resulted in an associative entity, transaction details. 
	Additionally, members can make multiple transactions from the proshop, but a singular transaction can only belong to one member. 
6. & 7. 
	Our general staff entity can perform maintenance on multiple courts, and each court can have multiple faculty working on its upkeep. Thus an associative entity maintenance request is created to symbolize this many to many relationship. 

<img width="660" alt="finalGroupDM" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/8a685da1-c35e-4a3d-a987-919c2e855365">



## Data Dictionary:

<img width="521" alt="coachingprograms" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/f4a7c03f-5774-4bd5-9c5b-9ebd96393c7f">

<img width="521" alt="coaches" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/ee58d532-33d9-4435-bd41-e2f862629e5a">

<img width="521" alt="courtreservations" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/94e3fae8-699c-4d80-9620-691e7eacaafc">

<img width="521" alt="courts" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/a8437356-5131-4eb3-b04f-35b7fae73bd2">

<img width="521" alt="generalstaff" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/335d16f8-82b8-4aa5-86fa-96f28ab49ac4">

<img width="521" alt="leagues" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/fc90c7f3-d017-4d19-b314-3ccb9d960a0c">

<img width="521" alt="maintenancerequest" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/afed42cc-eb1e-4fe8-9d0c-614261bb46d9">

<img width="521" alt="members" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/cf57082e-c707-49bd-ba90-eba1fa1345f5">

<img width="521" alt="proshopinv" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/9df5c742-d384-44eb-92ff-98724a55ce27">

<img width="521" alt="session" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/cf615fdd-0777-42e3-b9fb-eac4a687d5f3">

<img width="521" alt="transactiondetails" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/dee313f5-5a2a-48ff-bdd4-4ce215c08c3b">

<img width="521" alt="transactions" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/824b9845-0bbe-4329-b5c1-a2008e4a9dbf">

<img width="521" alt="divisions" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/79abd6de-8f63-4bae-8bdc-af5981993b06">


## Queries:



## Database information:

Name of the database: ns_21479_1

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: 
CALL TP_Q1();

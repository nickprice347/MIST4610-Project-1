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
<img width="269" alt="generalstaff" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/335d16f8-82b8-4aa5-86fa-96f28ab49ac4">

<img width="273" alt="leagues" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/fc90c7f3-d017-4d19-b314-3ccb9d960a0c">

<img width="266" alt="maintenancerequest" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/afed42cc-eb1e-4fe8-9d0c-614261bb46d9">

<img width="263" alt="members" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/cf57082e-c707-49bd-ba90-eba1fa1345f5">

<img width="266" alt="proshopinv" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/9df5c742-d384-44eb-92ff-98724a55ce27">

<img width="269" alt="session" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/cf615fdd-0777-42e3-b9fb-eac4a687d5f3">

<img width="277" alt="transactiondetails" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/dee313f5-5a2a-48ff-bdd4-4ce215c08c3b">

<img width="268" alt="transactions" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/824b9845-0bbe-4329-b5c1-a2008e4a9dbf">

<img width="521" alt="coachingprograms" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/f4a7c03f-5774-4bd5-9c5b-9ebd96393c7f">

<img width="272" alt="coaches" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/ee58d532-33d9-4435-bd41-e2f862629e5a">

<img width="270" alt="courtreservations" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/94e3fae8-699c-4d80-9620-691e7eacaafc">

<img width="268" alt="courts" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/a8437356-5131-4eb3-b04f-35b7fae73bd2">

<img width="266" alt="divisions" src="https://github.com/nickprice347/MIST4610-Project-1/assets/163012519/79abd6de-8f63-4bae-8bdc-af5981993b06">


## Queries:

![Screen Shot 2023-03-31 at 6 37 36 PM](https://user-images.githubusercontent.com/128402101/229244775-f60ebfa8-49b5-4dc1-95f4-ae027192c111.png)

1. Query 1 lists the number of reservations at each dining establishment that were made for between 6 and 8pm as well as the name of each dining establishment these reservation were made for. The results are also ordered by number of reservations in descending order.

![Screen Shot 2023-03-31 at 5 50 12 PM](https://user-images.githubusercontent.com/128402101/229239154-7637136b-5ddd-400c-9335-f3e571507ed7.png)

Query 1 allows allows managers to see which establishments have received the most number of reservations during their busiest time (6-8pm) which is typically dinner time. These establishments likely need more support, resources, and personnel around dinner time. Therefore, this query allows managers to identify which establishments to allocate this extra help to. Listing the results in descending order of number of reservations makes it easier to see which establishment to prioritize.

2. Query 2 lists the number of dining reservations made by guests on each floor. The results are ordered in ascending order of floor number.

![Screen Shot 2023-03-31 at 5 50 39 PM](https://user-images.githubusercontent.com/128402101/229239237-725cac35-598a-49e5-9b5d-bfc96fb18714.png)

Query 2 allows managers to see whether there is a trend between what floor a guest stays on and how much they reserve tabes at the resort's dining establishments. If managers were to find that dining reservations decreased as the floor number increased, it would have possibly indicated that guests were not dining at dining establishments because they felt the distance of the dining establishment from their room was too far and inconvenient.

3. Query 3 lists the information for all the guests who have not made an activity reservation.

![Screen Shot 2023-03-31 at 5 52 01 PM](https://user-images.githubusercontent.com/128402101/229239403-19acc956-7345-406e-b7ba-a6eaf1c8db88.png)

Query 3 allows the resort to market toward specific customers and contact them (e.g. promotional emails/coupons) about must-try activities. This helps to maximize revenue and increase efficiency by specifically targeting those who are not engaging in activities, rather than wasting time and resources to advertise to those who are already aware of and partaking in these activities.

4. Query 4 lists the names and phone numbers of dining employees who work in the highest rated dining establishment.
 
![Screen Shot 2023-03-31 at 5 53 30 PM](https://user-images.githubusercontent.com/128402101/229239730-7f5416bd-0aff-4c4a-b64d-7f365f246a36.png)

A restaurant with a high star rating is a large source of revenue for the resort and management may want to know the names of the employees who work there and how to contact them to reward them for maintaining such a high achieving restaurant (e.g. via a bonus, raise, awards, recognition) or to know which employees to target for continuous training and supervision in order to keep service within the establishment in top shape.

5. Query 5 lists the guests’ names and the hotel they are checking into if their reservation is during the PM, their room is a single or suite, their check in dates are between 2023-04-01 and 2023-04-10, and their hotel rating is above a 4.

![Screen Shot 2023-03-31 at 5 54 41 PM](https://user-images.githubusercontent.com/128402101/229239947-e3c0ab47-c77c-474b-81c1-1b187548b89c.png)

Query 5 allows the resort to manage how busy their check in will be during the PM hours of early April in their better hotels where the check in rooms are singles or suites. This can help the resort determine how many employees need to be working the check in desks to check in single or suite reservations in the afternoon of these dates in these specific hotels.

6. Query 6 lists the names of guests who have over 10 activity reservations and the activities that they have those reservations in.

![Screen Shot 2023-03-31 at 5 55 37 PM](https://user-images.githubusercontent.com/128402101/229240045-10ca60c7-1cb2-49e2-a224-256c841e5fd8.png)

Query 6 allows the resort to determine what guests are contributing the most to each activity’s revenue. The resort may use this information to reward guests who spend the most on activities by offering special prizes and promotions, creating guest loyalty and creating an incentive to reserve even more.

7. Query 7 lists the the amount of dining reservations per guest and the average amount of guests these reservations have.

![Screen Shot 2023-03-31 at 5 56 06 PM](https://user-images.githubusercontent.com/128402101/229240108-152740f1-4c85-4a38-9194-c981cf33fc42.png)

Query 7 allows the resort to see how many guests they should plan to seat, how the tables should be set up, and can lead to the resort figuring out how much revenue should be expected for the average visit.

8. Query 8 lists the guestID, guest name, and the number of room reservations per guest.

![Screen Shot 2023-03-31 at 6 34 05 PM](https://user-images.githubusercontent.com/128402101/229244470-c29f68b3-f837-4a18-97bb-f86345b84431.png)

Query 8 allows the resort to identify their frequent customers and how many times they have stayed. This could lead to a card system down the line. If a guest reaches 5 or 10 visits, there could be a platinum card which would gift the user reservation priority, food discounts, and other perks.

9. Query 9 lists all the rooms along with their average room view rating if the rating is above a 4 star. Additionally, the query is sorted by the view rating and arranged in descending order.

![Screen Shot 2023-03-31 at 5 56 31 PM](https://user-images.githubusercontent.com/128402101/229240166-bb0bc849-08dd-4521-8608-7a85ff53ae46.png)

Query 9 allows the employees and customers to see which rooms have an average view rating of 4 or more. Rooms with extravagant views are huge attractions to customers and can be a deciding factor when picking which room to stay in. This will help employees find which rooms have the best views fast and efficiently when asked.

10. Query 10 lists the names and prices of all activities offered by the resort that have not yet been booked by any guests and that are less than or equal to $50. Additionally, the results of the query are ordered by price in ascending order.

![Screen Shot 2023-03-31 at 5 57 00 PM](https://user-images.githubusercontent.com/128402101/229240218-c01fb32b-5f71-4562-b014-b656bfe051bb.png)

Query 10 allows the employees and customers to see what activities have not been booked yet, and the prices for these activities. The price is sorted in ascending order to make it easier to find the most affordable activities which most people are looking for. Activities are a huge part of the resort experience and using this script will make it easy for employees to find which activities are available as well as the prices for these activities.

## Database information:

Name of the database: ns_21479_1

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: 
CALL TP_Q1();

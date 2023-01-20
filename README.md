## Requirements for Group Project
[Read the instruction](https://github.com/STIW3054-A221/class-activity-soc/blob/main/GroupProject.md)


## Group Info:
1. Matric Number & Name & Photo & Phone Number
1. Mention who is the leader.
1. Other related info (if any)

| Matric Number    |Name           | Photo         | Phone Number    |
| :----:        |    :----:          |  :----: | :----:        |
| 281231      | Lim Jia Jun (Leader) |      <img src="https://user-images.githubusercontent.com/29892279/201517012-34d0ac1f-c549-4afc-a8b8-3c3507301673.JPG" width=20% height=20%>| 011-28797556 |
| 279590      | Chong Qi Jun       |<img src="https://user-images.githubusercontent.com/96851943/201516573-bc176bea-a75d-40d1-8d39-ef0707da0714.jpeg" width=20% height=20%>| 016-4926695 |
| 278985      | Teoh Ern Sheng     |<img src="https://user-images.githubusercontent.com/73087963/213664887-3d9a077d-2166-481c-a250-c4071f463d15.jpg" width="20%" height="20%"/>|011-20619201 |
| 277585      | Leong Qing Yun     |<img src="https://user-images.githubusercontent.com/73087963/201590357-090f120c-a014-45e5-971a-7c4a78c9d15f.jpg" width=20% height=20%>| 019-7108853 |
| 279437      | Tan Jia Kee        |<img src="https://user-images.githubusercontent.com/73268400/201550653-30b6cb6e-9509-4239-a820-2b7f9aef1853.jpg" width=20% height=20%>| 018-4055998 |

## Title of your application
A  Meeting Room Booking Systam  (@STIW3054_bugbug_bot)

## Introduction
This Meeting Room Booking System is for the user who wants to book the meeting room for their purpose. For our system, we have already done 3 parts. 
 
The first is that the System Admin. For this, the system admin can use this system to approve the school admin and display the list of school admin that have already been approved to manage the room.
 
After that, the user can use our system to register them as school admin by providing their information. After that, the school admin can log in to the system. The school admin can manage the booking of meeting rooms, such as registering rooms, updating room information, and displaying a list of rooms.
 
Besides that, the user who wants to book the meeting rooms can use our system to book the room. The user needs to provide their information to register as a user. Then, they can use the PIN that is generated after registering. They can use the PIN to book the meeting room. They can also update the booking details or cancel the booking. The user can use the specific command to display the user list and the available room list.

## Flow Diagram of the requirements
![STIW3054_BugBug_Diagram-FlowChart drawio](https://user-images.githubusercontent.com/72723643/201614006-92bc369d-8d84-4b08-87ac-aabd1d1c7893.png)

## User manual for installing your application on Heroku Server

 

## User manual/guideline for testing the system
1. User can start using our telegram bot by searching the @STIW3054_bugbug_bot .
2. After the click into this bot, they can enter **/start** to start this system.
3. After **/start**, the system will prompt up a mesaage
> Hello! Welcome to Meeting Room Booking System! <br/><br/>
> What is your position ? 
> 1. /systemAdmin
> 2. /schooladmin
> 3. /user

that let user choose their role.<br/><br/>
**System Admin** <br/>
> Step 1: Users can choose their role as System Admin by entering **/systemAdmin**. 
>> After that, a message and available command will be display.
>
> Step 2: Login to the system
>> The users need to choose **/loginSystemAdmin** and enter their **staff_id** and **password** to login. So, that they can get for more commands.
>
> Step 3: **/approvedSchoolAdmin**
>> After the users login into the system, some commands will be display. The users can reply **/approvedSchoolAdmin** to approve the request of register School Admin. 
>> <br/><br/>After the users reply **/approvedSchoolAdmin**, the system will requst users to enter their specific PIN. 
>> <br/><br/>If the users give the correct PIN, the system will display a list of School Admin which status is "pending". The users will be request to enter the **staff_id** that they want to approve.
>
> Step 4: **/displaySchoolAdmin**
>> After the users succeful approve the school admin, so they can reply **/displaySchoolAdmin** to check the school admin that already approve.
>

<br/>**School Admin**

> Step 1: Users can choose their role as School Admin by entering **/schooladmin**. 
>> After that, a message listing available commands will be displayed.
>
> Step 2: Register as School Admin
>>  The user can choose **/registerAdmin** and enter their **staff_id**, **name**, **phonenumber**, **email**, **password** and **schoolId** to register as a School Admin.
>
> Step 3: Create New Room
>>  The user can choose **/createNewRoom** and enter the **RoomId**, **RoomDescription**, **RoomStatus**, **RoomType**, **MaximumCapacity** and **SchoolId** to insert a new room into the system.
>
> Step 4: Update Room
>>  The user can choose **/updateRoom** and enter the **RoomId** of the room they want to edit then edit the details of the room.
>
> Step 5: Display Room
>>  The user can choose **/displayRoom** to display details of all the rooms in the system

<br/>**User**

> Step 1: Room Selection and User Registration
>
>>When the user receives a booking message, they are presented with the option to select a room. Before they can make a selection, however, they must first register their details by using the command /registerUser. The system will prompt them to provide their personal information, such as ICNO, UserID, Name, Mobile_TelNo, and Email. Once the user submits their details, the system generates a unique pin for them to use to access the booking system and make a reservation.
>
> Step 2: Booking and Management
>
>> After the user has registered and received their pin, the system will display available rooms for selection. The user can then provide the purpose, date, and time for their booking, as well as check their booking information by using the command /checkingUser and entering their UserID. They can also update their booking information and booking by using the commands /updateInfo and /updateBooking respectively, and cancel their booking by using the command /cancelBooking and entering their UserID.
>
> Step 3: Additional Features
>
>> In addition to the aforementioned functionality, the user can also view a list of all users and their room and booking information by using the command /displayUserList. They can view available rooms by using the command /displayAvailableRooms, and check their PIN by using the command /checkingPin and entering their UserID.


**Command**
> System Admin<br/>
>> 👉/loginSystemAdmin
>> - Allows the system admin to login to his/her account.
>> 
>> 👉/approvedSchoolAdmin
>> - Allows the system admin to approve the request of the register school admin.
>> 
>> 👉/displaySchoolAdmin
>> - Allows the system admin to display the list of school admin that the status is "Approved".
>>
>
> School Admin<br/>
>> 👉/registerAdmin
>> - Allows the School admin to register to his/her account.
>> 
>> 👉/createNewRoom
>> - Allows the School admin to create a new room ny providing the details.
>> 
>> 👉/updateRoom
>> - Allows the School admin to update the details of existing room by entering the RoomID and continue with the details.
>>
>> 👉/displayRoom
>> - Allows the School admin to display the information of the room.
>
> <br/>User Rights<br/>
>> 👉/received
>> - Allows the user to receive a booking message and select a room
>>
>>👉/registerUser
>>  - Allows the user to provide their details for booking a meeting room
>>
>>👉/checkingUser
>>  - Allows the user to check their booking information by entering their UserID
>>  
>>👉/updateInfo
>>  - Allows the user to update their booking information by entering their Pin
>>  
>>👉/checkingPin
>>  - Allows the user to check their PIN by entering their UserID
>> 
>>👉/updateBooking
>> - Allows the user to update their booking by entering their UserID
>>
>>👉/cancelBooking
>> - Allows the user to cancel their booking by entering their UserID
>>
>>👉/displayUserList
>> - Displays a list of users and their room and booking information
>>
>>👉/displayAvailableRooms
>> - Allows the user to view available rooms by selecting
 
## Result/Output (Screenshot of the output)
**Introduction  ,  /start**

<img src="https://user-images.githubusercontent.com/73087963/213394042-8047584f-65b3-413a-8e3a-19a846ae2435.png" width=25% height=25% >  <img src="https://user-images.githubusercontent.com/73087963/213394054-1602e566-d92c-4ef5-be47-d055fdf0a8e8.png" width=25% height=25% >

**/systemAdmin**

<img src="https://user-images.githubusercontent.com/73087963/213394346-6079f513-7d73-4979-acfd-13c5ca32d099.png" width=25% height=25% >  <img src="https://user-images.githubusercontent.com/73087963/213394379-146cc510-771b-4995-abf8-ea2e81345fd3.png" width=25% height=25% >  <img src="https://user-images.githubusercontent.com/73087963/213394289-cdb8ddfb-caa4-44d1-b509-85641e07bcbb.png" width=25% height=25% >

**/schoolAdmin**

<img src="https://user-images.githubusercontent.com/96851943/213610258-54b26b5c-a8c2-4889-8713-27334f77a955.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/96851943/213610271-cb139065-9cac-4e0c-825b-1ae3baffefab.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/96851943/213610277-ae24f95f-88b9-445d-b001-8b5b262fde92.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/96851943/213610282-25064504-5afc-4484-aa17-e45acd3097be.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/96851943/213610288-03b4d394-b064-40cf-a0d2-fba09590fed6.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/96851943/213610246-ccbd7cc8-67c1-41cc-8a7b-5f599af7881b.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/96851943/213610254-162164e8-86c3-4e87-acd2-8fce1b255fe1.jpg" width=25% height=25% > 

<img src="https://user-images.githubusercontent.com/72723643/213436410-b6429241-2d53-45c0-be58-61e75bea4454.JPG" width=25% height=25% > <img src="https://user-images.githubusercontent.com/72723643/213436874-937cff87-2035-4d77-b10f-4fa25a518f35.JPG" width=25% height=25% >


**/user**

<img src="https://user-images.githubusercontent.com/73268400/213635946-8b8dd86b-5f80-46ae-9c4d-666a74d863c1.jpg" width=25% height=25% > </br>
<img src="https://user-images.githubusercontent.com/73268400/213636005-64aa0c7c-59b8-4004-a691-242589950976.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/73268400/213640803-dec46977-b2f8-40ba-ac9d-30d905561d3d.jpg" width=25% height=25% > <img src="https://user-images.githubusercontent.com/73268400/213640949-5695e20e-9dbc-4d7b-b798-f5f95889972c.jpg" width=25% height=25% >

## Use Case Diagram!
<img src="https://user-images.githubusercontent.com/29892279/210562818-f341e8da-d170-4147-98ef-588aefd0a188.png" width=70% height=70% >

## UML Class Diagram


## Database Design
<img src="https://user-images.githubusercontent.com/29892279/211260314-e12d4668-c9a1-43d4-8ebc-1a9ddd310a32.png" width=70% height=70% >

## Youtube Presentation

## References (Not less than 20)
| Number | Reference                                                                                                                                                                                                                                                                                                             |
|:------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   1.   | Bots: An introduction for developers. (n.d.). Telegram. Retrieved December 8, 2022, from https://core.telegram.org/bots |
|   2.   | Code Java. (2020, October 25). Java Connect to SQLite Database Example [Video]. YouTube. Retrieved December 8, 2022, from https://www.youtube.com/watch?v=293M9-QRZ0c |
|   3.   | Creating SQLite database in intellij. (2020, June 1). Stack Overflow. https://stackoverflow.com/questions/62139581/creating-sqlite-database-in-intellij |
|   4.   | Fizz. (2020, June 23). Configuration JDBC drive with intlij IDEA || No suitable driver found for jdbc [Video]. YouTube. Retrieved December 8, 2022, from https://www.youtube.com/watch?v=duHgwpYLKZE |
|   5.   | Hartman, J. (2022, November 5). Split() String Method in Java: How to Split String with Example. Guru99. https://www.guru99.com/how-to-split-a-string-in-java.html |
|   6.   | How do I split a string in Java? (2010, August 14). Stack Overflow. Retrieved December 14, 2022, from https://stackoverflow.com/questions/3481828/how-do-i-split-a-string-in-java |
|   7.   | How to connect to SQLite with IntelliJ Community Version? (2021, October 11). If Not Nil. Retrieved December 8, 2022, from https://ifnotnil.com/t/how-to-connect-to-sqlite-with-intellij-community-version/2107 |
|   8.   | how to get an input from user from telegram bot in java? (2021, June 11). Stack Overflow. https://stackoverflow.com/questions/67941871/how-to-get-an-input-from-user-from-telegram-bot-in-java |
|   9.   | Inserting a string in a SQLite database. (2017, December 21). Stack Overflow. https://stackoverflow.com/questions/47923369/inserting-a-string-in-a-sqlite-database |
|  10.   | Java SQLite Example - javatpoint. (n.d.). JavatPoint. Retrieved December 8, 2022, from https://www.javatpoint.com/java-sqlite |
|  11.   | Prof. Vanselow. (2019, October 12). IntelliJ Database Connection [Video]. YouTube. https://www.youtube.com/watch?v=XCVbQgy_y90 |
|  12.   | riz can. (2018, May 13). IntelliJ - Connecting to SQLite [Video]. YouTube. Retrieved December 8, 2022, from https://www.youtube.com/watch?v=w5BeDoOn_l8 |
|  13.   | SQL error or missing database (near “?”: syntax error). (2014, November 20). Stack Overflow. https://stackoverflow.com/questions/27041163/sql-error-or-missing-database-near-syntax-error |  14.   | SQLite INNER JOIN with Examples. (2022, April 3). SQLite Tutorial. https://www.sqlitetutorial.net/sqlite-inner-join/ |
|  15.   | SQLite Java: Deleting Data. (2022, August 28). SQLite Tutorial. https://www.sqlitetutorial.net/sqlite-java/delete/ |
|  16.   | SQLite Java: Select Data. (2022, August 28). SQLite Tutorial. https://www.sqlitetutorial.net/sqlite-java/select/ |
|  17.   | SQLite Java: Update Data. (2022, August 28). SQLite Tutorial. https://www.sqlitetutorial.net/sqlite-java/update/ |
|  18.   | SQLite JDBC. (2022, November 22). Mvnrepository. Retrieved December 8, 2022, from https://mvnrepository.com/artifact/org.xerial/sqlite-jdbc/3.40.0.0 |
|  19.   | Sqlite, UPDATE with JOINs with 3 tables. (2020, April 20). Stack Overflow. https://stackoverflow.com/questions/61316781/sqlite-update-with-joins-with-3-tables |
|  20.   | Telegram Bot API. (n.d.). https://core.telegram.org/bots/api |
|  21.   | Telegram Bot Platform. (2015, June 24). Telegram. https://telegram.org/blog/bot-revolution |
|  22.   | Zaur Hasanov. (2018, February 10). How to create Telegram Bot in Java [ Tutorial ] [Video]. YouTube. https://www.youtube.com/watch?v=xv-FYOizUSY |

## JavaDoc

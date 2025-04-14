# Welcone to Tomato
This repository contains the task submission of the Lord of the chains task by Prathamesh Kukade 240573

What I understood : __
    - We have to create a CLI for a food delivery app like Zomato ! __
    - Customer should be able to order food and check its status 
    - Restaurants should be able to accept or reject orders 
    - Delivery boys should be selected on the basis of time required to deliver the order 
    - Priority orders should be delivered first 
What I did :
    - Designed a CLI using python in which you can login with three different ways : Admin , Restaurant , Customer 
    - Admin can control the app : He can add deliverey boys , Add restaurants . (We can also add options to delete them ) . He can see their status 
    - Customer : A customer can order food and check its status . (We can add a option to cancel the order) . 
    - Restaurant : A restaurant can access its orders and edit its menu . (We can add other features like they can take some time to prepare order )
    I created this basic functionalities and added few customization stuff from gpt 
    We can also create an interface for Delivery Boys where they can see where they have to go later 
    Also if a delivery boy reaches some house I updated his location as the location of the customer 
    I've added two restaurants and two delivery boys for basic testing 

Basic Workflow :
    Note : Everything is case sensitive .
           Password is 1234 wherever asked .
    First a customer will order his dish . 
    He will get a customer id . (Using this he can login again to check the status of his order)
    Then we have to login as restaurant 
    Then the request will be sent to the desired restaurant .
    Then the restaurant might accept or reject the order :
        - If rejected the customer will see the status as rejected .
        Note : There might be multiple requests pending in the restaurant . So if the number of orders outnumbers the number of delivery persons then we will accept priority orders first and keep others pending .
        Note : You have to enter list as : 6,2,3,5,7 to accept orders as restaurant . And the order first accepted by restaurant will be given more priority . Obviously if it is normal then it will have lower priority than priority .
        - If accepted : 
    A delivery boy will be autoassigned for the delivery 
    Then when will you check the status again as customer . You'll see real time similar simulation of the delivery of the order 
    Note : I've used time.sleep when customer logins to check status . I know this is wrong but this is near perfect simulation as we know customer will immedietly check the order status . 
    Once all orders delivered
    Restaurants will accept the later order and will deliver them !

Drawbacks and thier solutions : 
    - I've not added the feature to place multiple orders . We can do this easily by considering order as list rather than string and by using loops.
    - I've not created an interface of drivers . We can create that by thinking of some features later .
    - Real time simulation starts when customer checks the status . As soon as restaurant accepts the order we can start the real time simulation of delivery boy picking up the order but as we wanted to show our customer the stautuses seperately I started it later
    - Everything is case sensitive . We can use toupper something . 
    - Also I don't know threading so I havent used it .
    
    

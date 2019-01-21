# Front-end code assessment

> The following document describes the front-end assessment and all the requirements of it.

You will build two pages for a Lottery. Both pages have a different usage, but both require to fetch data and display it.   
- A user page displaying minimal data and the option to buy a ticket
- An admin page displaying some data and the option to generate a winner

## User page
The user page, or visitor page, can be seen for people willing to buy a lottery ticket. They should be able to see how many tickets already were sold, the average price and how many tickets are left. When a user has bought a ticket it shouldn't be able to buy another one. The client side should disable the possibility to do a request. 

## Admin page
The admin page acts like an administration panel for the lottery organizers. They need to see all the ticket sales, the average ticket price, how many tickets are left as well the posibility to generate a winner. The display of all tickets should be clean and sortable by price. When a winner has been chosen the administrator should be able to share the result on social media.

## API
[//]: # (Start --- TODO: API location should be changed with the description of the endpoints)
There's an API ready to use at: https://github.com/underscoretech/lottery-api/    
The endpoints are listed below with a little description of possible query parameters. Make sure the application can handle errors and communicate these in a clear manner to the user.

### Users
The endpoints below relate to the users page.

#### Get ticket information
Request
```
GET /tickets-info
```
Response
```
{
    "sold": 122,
    "average_price": 20,
    "tickets_left": 28
}
```

#### Buy a ticket
Request
```
POST /ticket
Body (form-data):
- price: "<price>"
```
Response
```
{
    id: 121
}
```

### Admin
The endpoints below relate to the admin page.


[//]: # (End --- TODO: API location should be changed with the description of the endpoints)

## Requirements
You can use any frontend framework (Angular, React, Bootstrap) possible or choose to do this assessment without one. Provide documentation about the application with possible build steps and/or explanation how to run the app. Below you'll find some limitations and extra credits.

### Limitations
- No jQuery

### Extra credits
- Starting page
- Setup for task runners (Gulp, Grunt)
- SEO optimisation
- Own design (additions)
- Animations
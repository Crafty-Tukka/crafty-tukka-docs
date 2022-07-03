# **Crafty Tukka**

## **T3A2-A - Full Stack App (Part A)**

### An application created by Simon Tanna and Jason Sandeman

***

### **[Click here](https://github.com/Crafty-Tukka/CraftyTukkaDocs)** to access the GitHub Repository for this file

***

### **Purpose**

In recent years, the city of Brisbane has seen the rise of numerous independent craft breweries whose locations range from the inner-city through to the outer-suburbs. Many of these breweries serve as community hubs where people can go to enjoy a locally produced beverage and quite often, purchase culinary offerings from one of the fantastic food trucks that operate in this great city.

A challenge faced by breweries wishing to book a food truck has been the inability for them to instantly view the availability of a truck before making a booking request directly to the business operator. Quite often, this results in a brewery having to contact numerous food truck operators before they find one that is available for a particular day and time.

Customers who wish to know what food truck will be at a particular brewery location at a given date and time can struggle to easily find this information. Usually it is achieved by trawling through the breweries or food truck businesses' social media channels in hope that they have posted their upcoming events for the week.

Crafty Tukka is a web application that aims to solve these problems by facilitating bookings between breweries and food truck operators and then displaying them with an easy to navigate user interface.

***

### **Functionality / Features**

Crafty Tukka features 2 types of user accounts that require an initial sign-up and secure login credentials: *Venue and Food Truck*.

Upon creating a new account, both brewery venues and food truck operators will be required to enter general information such as the *business name, description, email and phone number* with an option to include a *website and social media links*. Unique fields exist for each type of account with breweries being required to provide an *address* and food trucks a *cuisine category*.

Once registered and logged in, a brewery venue will be able to search for food trucks that are available on a given day while having the option to filter the list of food trucks by cuisine type. When the venue has found a food truck that they wish to book, they will be able to send a booking request to the truck operator who will be alerted of the request and then able to either accept or reject the request. Both user types are able to view, edit and cancel bookings.

When a booking between a venue and a food truck is confirmed, the details of the booking are added to the Crafty Tukka main page. This page features a map with pins showing the location of food truck events happening today with a list of upcoming events displayed adjacent to the map.

Any member of the public can view the map and event list. They also have the ability to view the individual details of all food trucks and venues.

***

### **Target Audience**

The Crafty Tukka application was created for use by food truck and brewery businesses in Brisbane. It also aims to serve members of the general public who wish to find out which breweries are hosting food trucks on a given day.

***

### **Tech Stack**

#### **Front-End**

- React.js
- HTML5
- CSS3
- Javascript
- JSX

#### **Back-End**

- Ruby on Rails
- Ruby

#### **Database**

- Postgresql

#### **Libraries and Utilities**

- Axios
- Material UI
- Draw.io
- Whimsical

#### **Deployment**

- Heroku
- Netlify

#### **Testing**

- Rspec Rails
- Jest

#### **Project Management**

- Notion
- Discord

#### **Version Control**

- Git
- GitHub

***

### **User Stories**

#### **Concept Personas**

The developers of Crafty Tukka created four personas whose needs have guided how the application looks and functions:

1. **The Craft Brewery Patron**
    - Visits craft breweries on a regular to semi-regular basis.
    - Is happy to make a journey across town to visit a particular brewery or attend an event held at one.
    - Enjoys the social environment created by a craft brewery and will often visit one with family and friends.
    - Choice of visited brewery sometimes dictated by the choice of food or entertainment on offer.

1. **The Food-Truck Foodie**
    - A culinary adventurer who is seeking the best food truck fare that Brisbane has to offer.
    - Has favourite food trucks that they will seek out on a regular basis.
    - Will actively search for trucks and cuisines which they have not tried yet.

1. **The Brewery Operator**

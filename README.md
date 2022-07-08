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
- AWS - S3

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

The developers of Crafty Tukka created **four** personas whose needs have guided how the application looks and functions:

1. **The Craft Brewery Patron**
    - Visits craft breweries on a regular to semi-regular basis.
    - Is happy to make a journey across town to visit a particular brewery or attend an event held at one.
    - Enjoys the social environment created by a craft brewery and will often visit one with family and friends.
    - Choice of visited brewery sometimes dictated by the choice of food or entertainment on offer.

1. **The Food-Truck Foodie**
    - A culinary adventurer who is seeking the best food truck fare that Brisbane has to offer.
    - Has favourite food trucks that they will seek out on a regular basis.
    - Will actively search for trucks and cuisines which they have not tried yet.

1. **The Brewery Events Coordinator**
    - Responsible for organising and marketing events to be held at the brewery.
    - Looks for unique and innovative themes concepts to attract patrons to the venue.
    - Is time-poor as this role is often part-time or shared with other brewery duties.
    - Handles social media posts and online promotion of the venue.
    - Requires tools to make the performace of their role more efficent and effective.

1. **The Food Truck Operator**
    - A small business owner/operator whose existence depends of securing ongoing locations in which to trade.
    - Responsible for their own marketing, social media accounts and brand awareness.
    - Takes great pride in creating high-quality food.
    - Cost margins are often razor-thin so having a full operating schedule with access to adequate patronage is essential to the viability of the business.
    - Is looking for ways to make the operation of the business more cost and time efficient.

#### **User Story Development**

Following the creation of the four concept personas, the development team determined which functions each user would want to perform in the application. If was determined that the *Craft Brewery Patron* and *Food Truck Foodie* personas shared overlapping needs and were therefore amalgamated into a single *General Public* user type. The joining of these personas into the one user story was possible due to the fact that they did not require authentication to use the application.

Amendments to the actions a *Food Truck* user type could perform were also made after consideration of real-world requirements. An example of this occurred where, in the original user story, a *Food Truck* user could request a booking from a *Brewery Venue* user. Upon consultation with brewery venues, it was determined that this feature would not be desired by breweries and add unnecessary complexity to the application. As a result, the feature of food trucks requesting bookings from a venue was scrapped from their story.

#### **User Story Management**

In order to manage the application user stories, the developers created a kanban board dedicated to tracking their changes and implementation. The board categorises each user story as *Minimum Viable Product* (MVP) or *Sprinkles* (optional features). Within each of these categories, the stories are tagged with the attriutes *Epic* (User Type) and *Priority* for ease of identification and are assigned a unique number identifier for referencing in the development phase. Stories that have been removed from either MVP and Sprinkles shifted into a Backlog list.

![User Story Kanban Board ScreenShot](./docs/user-stories/user-stories-07072022.png)

#### **Final User Stories**

Using the concept personas a guide, the developers of Crafty Tukka created clear stories for the **three** user types that will interact with the application. The aim of creating a streamlined *Minimum Viable Product* (MVP) guided what was to be initially included and excluded from each user story. A committment to constantly seek feedback from users during development and production means that these stories are subject to change.

#### **General Public User**

As a General Public user type:

| **I want to...** | **So I can...** | **Related Feature** |
| --- | --- | --- |
| View today's operating food trucks on a map | See a visual location of today's events | Home page map with venue pins |
| View today's operating food trucks in a sidebar list next to the map | Quickly reference each event's details | Home page map sidebar |
| View a list of all registered food trucks | Select a food truck to find out more about them | Access via a *view trucks* navbar link |
| View a list of venues | Select a venue to find out more about them | Access via a *view venues* navbar link |
| View the details of a particular food truck | View their bookings, website and socials | Access via a clickable link on each truck |
| View the details of a particular venue | View their website and socials | Access via a clickable link on each venue |
| Filter food trucks by cuisine type | Narrow down my search results to help me make a choice | Access via a dropdown menu in the *view trucks* component |
| Filter venues by event date | Narrow down my search results to help me make a choice | Access via a dropdown menu in the *view venues* component |

#### **Food Truck Operator**

As a Food Truck Operator user type:

| **I want to...** | **So I can...** |**Related Feature** |
| --- | --- | --- |
| Be able to do everything that a General Public user can do | Keep up to date on the status of current venues and competitors | |
| Sign up as a food truck user type | Have venues contact me to make a booking | Sign up page accessible from navbar |
| Receive booking requests from venues | Grow my business revenue | A booking request alert in which the truck can accept or reject booking |
| Define my primary cuisine category | Have users find my food truck by cuisine |  |
| Log in and out using secure credentials | Be confident that my private information is secure | Created using brcrypt and knock authentication |
| View my existing bookings | Be aware of my upcoming obligations | Access via clickable link in the user dashboard |
| View my pending bookings | Approve or reject them | Access via clickable link in the user dashboard |
| Upload my business image as an avatar | Have recognisable branding on the map | Required at the time of sign up and can be edited by the user in the edit profile page |

#### **Venue**

As a Venue user type:

| **I want to...** | **So I can...** |**Related Feature** |
| --- | --- | --- |
| Be able to do everything that a General Public user can do | Keep up to date on the status of current food trucks and competitors | |
| Sign up as a venue user type | Make bookings with food trucks | Sign up page accessible from navbar |
| Log in and out using secure credentials | Be confident that my private information is secure | Created using brcrypt and knock authentication |
| View available food trucks | Target food truck bookings appropriately | Access via a date select tab in the *create booking* page |
| Request bookings from a food truck whose availability on a particular day and time is displayed | Have confidence that I am not wasting my time by requesting a booking from an unavailable truck | Trucks who have existing bookings on a day are excluded from list of trucks |
| Submit a request to edit a booking | Make changes if necessary | Access via clickable link in the *my existing bookings page* |
| Submit a request to delete a booking | Make changes if necessary | Access via clickable link in the *my existing bookings page* |
| View my existing bookings | Be aware of my upcoming obligations | Access via clickable link in the user dashboard |
| View my pending bookings | See if a food truck has approved or rejected them | If a booking is rejected, the venue has the ability to request a new truck without having to create a new booking |
| Upload my business image as an avatar | Have recognisable branding on the map | Required at the time of sign up and can be edited by the user in the edit profile page |

***

### **Application Architecture Diagram**

![Crafty Tukka Application Architecture Diagram](./docs/aad/aad-crafty-tukka.png)

***

### **Dataflow Diagram**

***

### **Wireframes**

#### Landing Page Views

Referencing **[MVP User Story #1](https://jwsandeman.notion.site/View-today-s-operating-food-trucks-on-a-map-9d7e0e18537246aba2c5683e42fff3e6)**
![General User Story #1 Wireframes](./docs/wireframes/general-user-wireframes/landing-page-mvp-1.png)

#### Map View With Event Details

Referencing **[MVP User Story #2](https://jwsandeman.notion.site/View-today-s-operating-food-truck-events-in-a-sidebar-list-next-to-the-map-f8a9edd85c7144cdb8c60cc018c325fa)**
![General User Story #2 Wireframes](./docs/wireframes/general-user-wireframes/mvp-user-story-2.png)

#### Food Truck List and Details Views

Referencing **[MVP User Story #3](https://www.notion.so/jwsandeman/View-a-list-of-food-trucks-37be7a3edf824e7c8427f4456af1c5a2)** and **[MVP User Story #7](https://jwsandeman.notion.site/View-the-details-of-a-particular-food-truck-402c2caa83cf4414a16a9c3264ec3b61)**

![General User Stories #3 ane #7](./docs/wireframes/general-user-wireframes/mvp-user-stories-3-7.png)

#### Venue List and Details Views

Referencing **[MVP User Story #4](https://www.notion.so/jwsandeman/View-a-list-of-venues-54307186ee1741c5890f92c000045038)** and **[MVP User Story #8](https://www.notion.so/jwsandeman/View-the-details-of-a-particular-venue-6e8ab0c0e1274c6e880116d8dba2b25a)**

![General User Stories #3 ane #7](./docs/wireframes/general-user-wireframes/mvp-user-stories-4-8.png)

***

### **Project Management**

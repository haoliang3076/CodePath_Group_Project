Original App Design Project - README Template
===

**MATCHMAKER**

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description

tired of Tinder? We are developing the best matchmaking iOS application to pair you with the best. Similar idea like Tinder but with different design and matched algorithms. A slightly different approach consisting of features including matching peer study groups, gaming partner like Animal Crossing, and the better way to make a match. 

### App Evaluation
[Evaluation of your app across the following attributes]

- **Category**: Social Networking/Lifestyle
- **Mobile:** iOS mobile device 
- **Story:** User will match/pair of their interest
- **Market:** 16+ 
- **Habit:** This app can be used at any time, but requires use from other users to make match
- **Scope:** People will be able to match like/dislike on other users profile to make their best pair. Map features will give user best experience to get to know each other.

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* Login/Register 
* Create profile
* Show matches with similar interests
* Chat with people
* Geolocator to decide on places for meetups

**Optional Nice-to-have Stories**

* Maybe show a pop-up everytime there is a match

### 2. Screen Archetypes

* Login/Register
   * User registers or logs in into the app
   
* Detail
   * User can create his/her profile accordingly
   * They can also answer certain questions to filter out their matches
   
* Profile
  * Users can view others profiles before they match with them and the profile will also show them how far do they live from each other

* Maps
  * Users (after finding their matches) can decide to meet up through our geolocator map within a certain distance
  
### 3. Navigation

**Tab Navigation** (Tab to Screen)

* <img src="https://i.imgur.com/nevXhFo.png" width=600>
* Home
* Profile

**Flow Navigation** (Screen to Screen)

* Launch Screen [MatchMaker]
   * Launch Screen --> Login/Register Screen
   
* Login/Register Screen
   * Login/Register Screen --> Create Profile Screen --> Profile Screen
   
* Profile Screen
  * Edit profile --> Save it --> Start looking for matches
  
## Wireframes
<img src="https://github.com/haoliang3076/CodePath_Group_Project/blob/main/AppWF.jpg" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 
### Models

- Login Screen

| Property | Type | Description|
| -------- | -------- | -------- |
| username     | String     | special id for user     |
| password    | String     | special password for user     |

- Profile Screen

| Property | Type | Description|
| -------- | -------- | -------- |
| profilePic     | File     | image of author  |
| postPic     | File     | author's posts  |
| profilePic     | File     | image of author  |

- Search Screen

| Property | Type | Description|
| -------- | -------- | -------- |
| userID     | String     | Unique ID   |
| Data     | List | List of current existing matches
| filteredData | String | Represent rows of data that match the search text
| Image     | File     | image that users post    |
| Description     | String     | image description by author     |


### Networking 

- Login Screen
    - (Create) New Account
    - (Get) Username 
    - (Get) Password

- Profile Screen
    - (Read/GET) Query logged in user object
    - (Update/PUT) Update user profile image
    - (Update/PUT) Update user's post image
    
- Search Screen
    - (Create/POST) Create a new like on the profile
    - (Delete) Delete existing like
    - (Create/POST) Create a new comment on the post
    - (Delete) Delete existing comment on the post

- [Create basic snippets for each Parse network request]
- [OPTIONAL: List endpoints if using existing API such as Yelp]

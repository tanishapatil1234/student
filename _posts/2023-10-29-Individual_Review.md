---
toc: true
comments: true
layout: post
title: Individual Review Ticket
description: Recap of key events this trimester and all that I have learned. 
type: plans
courses: { compsci: {week: 2} }
---
# CB MCQ Reflection (in progress) 
- [Link](https://tanishapatil1234.github.io/student/2023/10/29/CB_Final.html)

# End of Tri Reflection
- [Link](https://tanishapatil1234.github.io/student/2023/10/29/EndofTriReflection.html)

# Student Grading

<img width="142" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/efd7e426-8572-45fc-8fc8-5da1c24aefa5">



# Issue Recap and Highlight Meaningful Commits 

## Backend - Developed Functional Spring backend 
> Quote.java [Commits](https://github.com/vivianknee/PT_Backend/commit/ffb6ade720f9d9cb405993ae5bc936f5f3b22aa3), 
> QuoteApiController.java [Commits](https://github.com/vivianknee/PT_Backend/commit/ee09baefb4d1b0e707e73d54f7dd65648d155f39), 
> QuoteJpaRepository.java [Commits](https://github.com/vivianknee/PT_Backend/commit/2f351dfdd6c8b562750101f3074d5eb5dd25ee5d), V
> QuoteService.java [Commits](https://github.com/vivianknee/PT_Backend/commit/ee8faa3620f8e3963119052d2b61d34c08073407)

- Read about Spring and creating stand-alone applications. [Reading](https://spring.io/projects/spring-boot) 
- Used jokes and person files as reference. Went line-by-line to understand all functionality
- Created Spring backend system to support the application's functionality. I made: 
    

<img width="525" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/920f0993-ec3e-4040-bd17-00f4baacd61a">

### Quote.java: 

- Defines the "Quote" class.
- Each instance has attributes like "quote" and "emotion."


<img width="525" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/5852d638-0f95-4812-b8ad-a2831388236e">

### QuoteApiController.java: 
 -  Created endpoints for: 
    - GET random quotes by emotion
    - POST new quotes
    - PUT existing quotes
    - DELETE quotes.

### QuoteJpaRepository.java:
- extends Spring Data JpaRepository
- defines methods for accessing and manipulating the "Quote" entity
- includes methods for saving and querying quotes.

<img width="525" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/83c63546-c4f5-4cdb-9ab3-a9e9184ed00d">

### QuoteService.java: 
- service provides methods for saving quotes
- uses "QuoteJpaRepository" for operations on the data
- used to manage quotes within the application.



## Backend - [CRUD Functions](https://github.com/vivianknee/PT_Backend/commit/6c23472a5e43f00f71dec78f0c51ca5e9d9cabde)
- See Issue [Link](https://github.com/vivianknee/PocketTherapist/issues/12) for code and Postman proof
- Created all functioning 4 CRUD operations for data management


## Backend - CORS
- I also dealt with CORS errors which made me look into the SecurityConfig.java and MvcConfig.java files. Below are the changes I made to fix CORS

<img width="1019" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/39e99488-c342-492f-a4ac-9c819a9625cf">
<img width="1019" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/2c1536fc-7582-47be-b74c-8be4a8d536f9">



## Frontend - Created Facial Recognition Model JS
- See Issue [Link](https://github.com/vivianknee/PocketTherapist/issues/1)
- Note that I switched to a pretrained JS model because I wanted to try something new. Because of that I did use a pretrained model. However the implementation of the model (it's weights, dropouts, overfitting parameters etc. ) still took time to implement into our project. 
- The model I referenced for example did not return the emotion. I had to extract that information by comparing each of the emotion values and choosing the highest. 


<img width="546" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/c1b76594-470e-47b0-98dc-d5eb6a4da9f2">
<img width="546" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/3c912126-5478-4481-b525-e4eeac71de6e">

- Live [Demo](http://localhost:5500/c.html) or see GIF below. 
![Untitled_Project_V2](https://github.com/vivianknee/PocketTherapist/assets/111611921/c31f0e1c-eecf-452d-a527-d2d1da9c4eee)


## Frontend - Created A Test Application 
- I created this test application so I could experiment with the GET request and find any problems. It was also a good challenge for me and a way to test out the CRUD. 
- [Link](https://tanishapatil1234.github.io/student/2023/10/08/JournalApp_IPYNB_2_.html)



## Frontend - Implemented Get Request with Model Results
- As you can see in the live demo, a GET request is sent based on the result of the model 
- I created an Endpoint on the backend with a function which randomly generates a quote given an emotion
<img width="590" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/da573124-397a-4e82-b2f5-1965b6391a99">
<img width="590" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/cbfcb124-f9e1-4b57-80f0-683c0ddef86c">
<img width="590" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/9f06f9bd-9477-4ac0-a039-78fc03e224eb">
<img width="590" alt="image" src="https://github.com/vivianknee/PocketTherapist/assets/111611921/1575c72f-e00b-45ca-a64b-d23341309c1d">

![screen-recording webm_V1](https://github.com/vivianknee/PocketTherapist/assets/111611921/334bcdf2-0d88-4cfa-815d-0b2a6c82391d)


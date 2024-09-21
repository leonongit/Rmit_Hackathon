# <p align="center">Rmappy
<p align="center">
CSIT & SWITCH Hackathon - MSEC project <p align="center">
<img src="https://github.com/leonongit/Rmit_Hackathon/blob/main/img/Screenshot%202024-09-20%20225644.png?raw=true" width="400px" height="400px" alt="logo"></img></p>

# Problem Statement
Our group project addresses a common and frustrating challenge faced by students at RMIT University: navigating the campus's numerous and often confusing buildings. This issue is particularly pronounced with buildings like 56 and 57, which are housed within the same larger structure, causing many students, especially newcomers, to mistakenly think they are in the wrong place. This confusion results in wasted time and added stress when trying to find classrooms, impacting punctuality and overall student experience. By identifying this problem, we aim to deliver a solution that simplifies campus navigation, reduces confusion, and improves the overall ease of finding the correct buildings. Our approach focuses on the needs of the target audience,students and is both technically and economically feasible, with a clear value proposition and a scalable plan for implementation.

# Demo Video
Rmappy Website <p>
https://rnithackathon.netlify.app<p>

Youtube address
https://www.youtube.com/watch?v=cDrTSicgxss

<img src="https://github.com/leonongit/Rmit_Hackathon/blob/main/images/Demo_Rmappy.gif?raw=true"></img>
We displyed a demo video showcasing the app's core features, including GPS guidance and visual guides for navigating the campus buildings. The video will demonstrate the ease of use, highlighting how students can confidently find their way around campus using the app.

# Target Audience and Market
Our target audience is primarily RMIT students, particularly those unfamiliar with the campus layout. Additionally, staff and **visitors** may find the app useful in navigating the numerous buildings at RMIT.

# Who Created This
This project was created by 
- NARY BYUN <p>
- LWIN KO MIN <p>
- NYO YAN NAING MIN <p>


# Project Period
From 20th Sep 2024 To 21st Sep 2024 <p>
The development period for this project is **31 hours**, during which we aim to deliver a Minimum Viable Product (MVP) with basic GPS functionality and visual guides. Future versions of the app will expand on this foundation with additional features.

# Value Proposition
Our app saves students time and reduces confusion by offering a streamlined solution for navigating the RMIT campus. By combining **GPS navigation** and **visual guides** the app makes it easy to find the right buildings and classrooms, reducing stress and frustration.

# Product Differentiation

- **User-Friendly Interface**: The app offers a simple, intuitive interface that students can easily navigate, ensuring a seamless experience for all users, even those unfamiliar with technology.
  
- **Personalized Navigation**: The app provides personalized directions based on the user’s current location, taking into account common student routes and allowing users to find classrooms and buildings with ease.

- **Visual and GPS Integration**: Unlike generic map services, **RMIT Navigator** combines both **GPS navigation** and **visual guides**, such as campus-specific photos of building entrances and key landmarks, making it easier for students to recognize and navigate through complex areas like Buildings 56 and 57.

- **Efficient Time-Saving Tool**: The app significantly reduces the time spent searching for classrooms, ensuring that students reach their destinations on time. The real-time GPS updates help avoid any confusion caused by the numerous buildings on campus.

- **Expert Support for Campus Navigation**: The app is tailored for RMIT students, built in collaboration with experts who understand the layout and common navigation challenges faced on campus.

- **Engagement and Customization**: Future versions of the app will offer a **reward system** for user contributions, where students can update building details or upload photos and receive credits or tokens for their efforts. This will ensure that the app remains accurate and up-to-date.

- **Student-Centered Features**: Unlike generic mapping solutions that don't cater to specific campus layouts, **RMIT Navigator** is built with students in mind. It takes into account the unique challenges of navigating a large university in an urban setting and focuses on addressing the pain points of new and existing students.




# Solution Architecture

<img src="https://github.com/leonongit/Rmit_Hackathon/blob/main/images/userPerspective.png?raw=true"></img><p><img src="https://github.com/leonongit/Rmit_Hackathon/blob/main/images/webDevelopment.png?raw=true"></img><p>


The **RMIT Navigator** app utilizes **JavaScript**, **Google Maps API**, and **HTML** to provide real-time navigation assistance for students and staff on the RMIT University campus. The solution is designed to be lightweight, focusing on GPS navigation and visual guides without the need for a database. 

1. **Frontend (HTML, JavaScript)**:
   - The frontend is developed using **HTML** for structure and **JavaScript** to handle user interactions. 
   - Users input their desired classroom or building, and the app retrieves GPS-based navigation data directly from the Google Maps API. The visual interface provides easy-to-understand instructions and photos to assist with navigation.
   - All navigation and visual data are handled dynamically using **AJAX requests** to the Google Maps API.

2. **Google Maps API**:
   - The **Google Maps API** is the core component of the app, providing **real-time GPS navigation** and geolocation services.
   - Key features include:
     - Retrieving GPS coordinates for the requested building.
     - Providing step-by-step navigation from the user's current location to the building.
     - Displaying a map view with markers for both the user's current location and the target destination.
   - The API also supports calculating the best route to the desired building and updating the route in real-time as the user moves.

3. **Backend (JavaScript and Firebase)**:<p>
The lightweight JavaScript backend, powered by Firebase, handles the app’s logic, processes user requests, and manages authentication using Firebase’s login API, which supports methods such as email/password or OAuth providers like Google. Once users are authenticated, Firebase ensures secure session management, enabling only authorized access to navigation features. When a user searches for a building, the backend interfaces with the Google Maps API to retrieve navigation data (e.g., GPS coordinates and directions) and forwards it to the frontend for real-time display. This seamless integration of Firebase ensures efficient data synchronization between the backend and frontend, providing smooth and fast navigation.

4. **Visual Guides**:
   - Visual guides (such as photos of building entrances and key landmarks) are **hardcoded** or linked directly in the frontend, ensuring students can visually recognize their surroundings when navigating the campus.
   - These images are stored locally within the app or fetched from external sources but do not require a database for storage.


By focusing on the **Google Maps API** and a lightweight **JavaScript-based frontend**, this architecture ensures that RMIT students can easily navigate the campus without the complexity of managing a database. The solution is scalable, allowing future enhancements while maintaining simplicity in its current form.



# Web Development
We are using **GitHub** to manage the project’s development. The **main branch** contains the stable version of the app, while the **development branch** is used for active work. New features such as GPS navigation and photo guides are developed in separate branches before being merged into `dev`.

# User Perspective
From the user’s perspective, the app provides:
1. A search feature to find buildings or classrooms by name or number.
2. **GPS-based navigation** to direct the user to the right building.
3. **Visual guides** (photos) to help identify the correct building.
<p>
  
# Future scope 
<p>development activities will include creating a system that allows users to interact by posting or rating each building on the website, as well as implementing additional features such as restricting visibility of updates (e.g., credits or photos) to those who made the updates. These enhancements aim to spark users' interest and attract more people to the platform. Furthermore, we can expect potential additional revenue through credits or subscriptions in the future.

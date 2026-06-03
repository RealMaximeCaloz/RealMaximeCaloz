# Portfolio

---

## AI-Powered Learning Platform

This full-stack project is an AI-powered learning platform where users enter any topic they want to learn, answer prerequisite and clarification questions, and receive a personalized course generated on the fly, with a Duolingo-style UI.

This platform is especially effective in the sense that it remembers what users have already learned, avoiding unintentionally re-teaching the same topics excessively outside of planned spaced repetition.

The platform is split across two repositories: a Go backend that handles authentication, billing, and course generation, and a frontend web client that guides learners through creation, lessons, streaks, and progress.

Down below, you can see screenshots of the AI-Powered Learning Platform:

![AI-Powered Learning Platform](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/ai-powered-learning-platform.png)

On the backend, courses are built asynchronously through a multi-step pipeline. The system researches each topic submitted by the user with web searches, indexing scraped content in a Qdrant vector database for retrieval-augmented generation (RAG), and uses OpenAI API with RAG to produce a full course, complete with units, lessons, and micro-lessons, each with text content, optional Mermaid diagrams, and quizzes. User progress is tracked in SQLite with XP rewards, level progression, daily streaks, and completion state at every level of the course tree. The backend also handles Google OAuth login, JWT sessions, Stripe subscriptions and webhooks, rate limiting, and Swagger documentation.

On the frontend, learners sign in, create courses from their topic of choice, rate their prerequisite skills, and browse generated material through pages for course overview, individual lessons, and account management. The UI uses a gamified layout, and connects to the backend over REST.
The web app is fully-responsive, working on desktop, or on mobile in the browser. Additionally, the web app is available for download on mobile as a PWA (Progressive Wev App), with a service worker and web manifest for offline-friendly access.

The AI-Powered Learning Platform currently includes:

- Google OAuth authentication with JWT-protected API routes
- AI-generated prerequisites and clarification questions before course creation
- Retrieval-augmented course generation grounded in scraped web content, vector search, & OpenAI API knowledge
- Structured courses with units, lessons, micro-lessons, quizzes, and Mermaid diagrams
- Asynchronous course generation with progress persistance with SQLite
- XP, levels, random bonus reward drops, and daily learning streaks
- Stripe subscription management and webhook handling
- Course creation, course overview, lesson view, and account pages all functional in the UI
- Progressive Web App support (manifest and service worker)

This project was made with **Go (Gin, SQLite, OpenAI API, Qdrant, Stripe)** on the backend and **HTML, CSS, and JavaScript** on the frontend.

---

## Car Database Web App

[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/car-database-app)

This project is a database web app which visually shows off the various specs of different cars, with the help of dynamically-resizing progress bars.
The wider the bar, the better that particular spec of the car is.

Down below, you can see screenshots of this car database web app in full glory, thanks to its visual appeal.

You can use the left and right triangular buttons to navigate between the specs of various cars.

![Idle UI](https://github.com/RealMaximeCaloz/car-database-app/blob/1b28bab5db43eb5d66e3555cc5694450c1555b8d/screenshots/car_db_idle_ui.png)

If you would like even more control, you may click the title banner in the middle to make a drop down menu appear. From this menu, you can choose to display whichever car you wish.

![Drop down menu](https://github.com/RealMaximeCaloz/car-database-app/blob/1b28bab5db43eb5d66e3555cc5694450c1555b8d/screenshots/car_db_drop_down_menu.png)

This project was made with **HTML, CSS, JavaScript (node, express)**.

---

## Multithreaded Sudoku Solver

[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/Multithreaded-Sudoku-Solver)

This project was made with **Java (Libraries: Concurrent, Arraylist)**.

This software takes a Sudoku board as an input (array of numbers from 1 to 9, with 0's representing empty cells), solves the board through a recursive algorithm and prints the result.

An example of an initial Sudoku board to solve:

![starting board](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/startingboard.png)

If the board is unsolvable, that information will be printed for the user.

A new ExecutorService job is submitted for each number which would be a valid guess for the Sudoku board's first empty cell, hence harnessing the power of multithreading and parallel processing.

The Sudoku board is solved very quickly, even if it is near-impossible to solve for humans:

![final board](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/finalboard.png)

---

## Commercial Bulk Instagram Post Generator

[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/Commercial-Bulk-Instagram-Post-Generator)

This project was made with **Java (Libraries: AWT, I/O, Graphics)**.

This software takes into input a folder filled with images (backgrounds for posts), and an array of strings with the text to add to each post.

This software will crop all the images in bulk down to square size, dim the images to increase contrast with text, and will add 1 string from the array of strings to each image.

This effectively generates Instagram posts in bulk extremely quickly with little-to-no effort.

You can even brand the posts with your own Instagram handle, to prevent content stealing, and free publicity.

If you want to generate 1000 posts in seconds, so that you do not have to worry about content creation for the next 3 years, you can simply use this software.

Example of a generated Instagram post:

![generated post example](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/GeneratedInstagramPostExample.jpg)

A [REST API version](https://github.com/RealMaximeCaloz/REST_API) of this program has also been created to practice using Spring Boot and Thymeleaf.

The REST API features a front-end which accepts a String and an image as inputs.

![api_inputs](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/pic1_rest_api.png)

The API adds the text to the image provided, and returns the processed image to the user on the front end.

![api_outputs](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/pic2_rest_api.png)

---

## Full-Stack License Manager Web App

This project was made with Javascript (React, Node, Express), SQLite, HTML & CSS.

The License Manager web app is meant to be a platform where clients of a software company can login to view, purchase or extend their access to software licenses.

The License Manager currently has the following features:
-	User login (with verification of inputs and feedback to the user)
-	Sign Up (with verification of inputs)
-	License Manager Dashboard with dynamically rendered content pulled from the database tables, depending on who is logged in
-	Ability to change user profile picture
-	Simulated credit card payment to buy a license (with input verification)
-	Unique License Key Generator in the backend (with keygen rules to make guessing license keys very difficult)
-	Verification of the validity of input license keys

Down below, you can see a screenshot of the login page.

![login](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/license_manager_pic1.png)

Here is a screenshot of the License Manager's Dashboard:

![dashboard](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/license_manager_pic2.png)

The user's first name and profile picture is dynamically generated based on who is logged in, as well as all license data in the dashboard.

Down below, you can find a screenshot of the License Manager's Popup to purchase a new license or redeem an externally-obtained license.

![Purchase Popup](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/license_manager_pic3.png)

More features will later be added such as:
-	Improved security features
-	Stripe integration for payments

---

## Image Cryptography Tool

[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/Image-Cryptography-Tool)

This project was made with **Python (Libraries: PIL, NumPy)**.

This software uses bitwise operations to cloak a given image within the image information of another image, making it nearly invisible to unsuspecting parties.

Example of an image to hide:

![image to hide](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/epiccar.jpg)

Example of the container image in which you want to cloak your hidden image:

![container image](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/basiccar.jpg)

After running this software, you obtain a combined image which contains the hidden image, but it looks very much like the unmodified container image.

Example of the combined image, which contains the hidden image:

![combined image](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/composite-image-with-hidden-image.jpg)

You (or the party you are trying to send a hidden message to) can also run an image extractor in the software, which will extract the hidden image from the combined image.

Example of the hidden image extracted from the combined image:

![extracted image](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/hidden-image-extracted-from-composite.jpg)

As you can see, the extracted hidden image has inherited a few visual artefacts.

However, its depiction is still blatantly obvious, despite having been secretly cloaked in a completely different image.

---

## TurboSpeed - Infinite Scrolling Racing Game

[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/TurboSpeed/tree/master)

This project was made with **Python (Library: Pygame)**.

TurboSpeed is an engaging and addictive arcade-style infinite scrolling racing game developped with Python and the Pygame library.

In TurboSpeed, the player controls a car speeding down a dynamically-scrolling road, with the objective of avoiding boulders for as long as possible. As time goes on, the car moves faster and faster, thus increasing the difficulty.

Down below, you can see a screenshot of the gameplay.

![gameplay](https://github.com/RealMaximeCaloz/TurboSpeed/blob/master/Game%20Screenshots/gameplay.png)

Here is a screenshot of the TurboSpeed title screen.

![title screen](https://github.com/RealMaximeCaloz/TurboSpeed/blob/master/Game%20Screenshots/title_screen.png)

Down below, you can find a screenshot of the TurboSpeed game over screen (and my high score!).

![game over screen](https://github.com/RealMaximeCaloz/TurboSpeed/blob/master/Game%20Screenshots/game_over_screen.png)

---

# Text-Based Adventure Game Engine + Game: The Last Dragon Hunter

[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/The-Last-Dragon-Hunter)

This project was made with C++ and the MSYS2 compiler.

This project is a game engine that allows users to create text-based adventure games.

The game engine allows players to interact with a text-based UI in order to progress through an adventure as the main character.

The player can navigate to different rooms and areas, and their choices dictate how the game plays out.

The game engine also comes coded with a battle engine, allowing for thrilling battle encounters with foes.

As the player accumulates victories, they will level up, resulting in strengthened personal attributes.

A game has also been created with this game engine. 

The game is called The Last Dragon Hunter and follows the story of a 220 year old dragon hunter, left alone to fend off organized attacks by the repopulating dragons.

Down below, you can see a screenshot of the game and game engine in action:

![game](https://github.com/RealMaximeCaloz/Portfolio/blob/main/screenshots/the_last_dragon_hunter_gameplay_screenshot.png)

The infrastructure in this c++ game engine offers text-based adventure game creators a flexible and relatively simple development experience, comprehensible even for non-developers.

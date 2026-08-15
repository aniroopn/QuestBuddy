# QuestBuddy

QuestBuddy is an Android travel planning application that my team and I built as a class project. Our team consisted of four students, and we worked together on both the Android frontend and Spring Boot backend.

The idea behind QuestBuddy was to make planning a trip with other people easier by putting several useful features in one place. Instead of using separate apps for messaging, budgeting, scheduling, and keeping track of tasks, QuestBuddy allows users to manage these parts of a trip from the same application.

## Features

Some of the main features we implemented include:

* User signup and login
* Creating and managing trips
* Inviting other users to trips
* Friends, friend requests, and friend suggestions
* Direct messaging between users
* Group messaging within trips
* Real-time messages and notifications using WebSockets
* Trip calendar and events
* Task manager
* Packing checklist
* Trip budget management and expense splitting
* Currency converter
* User profiles and settings
* Notifications
* Premium/payment functionality using Stripe

## Tech Stack

### Frontend

The mobile application was developed natively for Android using:

* Java
* Android Studio
* XML layouts
* Android Volley for API requests
* Java-WebSocket for real-time communication
* RecyclerView and other Android UI components

### Backend

The backend was developed using:

* Java 17
* Spring Boot
* Spring Data JPA
* REST APIs
* WebSockets
* MySQL / MariaDB
* Maven
* BCrypt password hashing
* Stripe API
* Swagger / OpenAPI

### Testing

During development, we also wrote frontend and backend tests using tools including:

* JUnit
* Mockito
* Espresso
* REST Assured

## Running the Project

### Backend

The backend requires Java 17 and Maven.

Navigate to the backend directory:

```bash
cd Backend
```

Then run:

```bash
mvn spring-boot:run
```

The backend runs on port `8080` by default.

Database information and other configuration can be changed in:

```text
Backend/src/main/resources/application.properties
```

For security, database passwords and API keys should be stored as environment variables instead of being committed directly to the repository.

### Android App

1. Open Android Studio.
2. Select **Open**.
3. Open the Android frontend folder.
4. Allow Gradle to finish syncing.
5. Start an Android emulator or connect an Android device.
6. Run the app.

The Android application communicates with the Spring Boot backend, so the API address may need to be changed depending on where the backend is running.

## What We Learned

This project gave our team experience building a larger application where a mobile frontend had to communicate with a separate backend and database.

We worked with REST APIs, database relationships, authentication, WebSockets, Android development, testing, Git, and team-based software development. One of the more challenging parts was connecting all of the different features together while making sure changes made by different team members continued to work with the rest of the application.

Working in a team of four also gave us experience dividing up features, integrating each other's work, resolving merge conflicts, and coordinating changes between the frontend and backend.

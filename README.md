# Mapty App

<b>Mapty is a cycling and running tracker application that allows users to log their workouts with various details like location, distance, time, speed, elevation gain, and steps per minute. The app utilizes the Geolocation API to display a map at the user's current location, allowing them to click on the map to add a new workout and record their exercise data.</b>

## User Stories

1. As a user, I want to log my running workouts with location, distance, time, pace, and steps per minute.
2. As a user, I want to log my cycling workouts with location, distance, time, speed, and elevation gain.
3. As a user, I want to see all my workouts at a glance.
4. As a user, I want to see my workouts on a map.
5. As a user, I want my workouts to be saved so that I can see them when I leave the app and come back later.

## Features

### Interactive Map:

- Display a map at the user's current location using the Geolocation API.
- Allow the user to click on the map to add a new workout and obtain the location coordinates.

### Workout Forms:

- Provide forms to input workout details for running and cycling workouts.
- Running Workout Form:
- Input fields for distance, time, and steps per minute (cadence).
- Cycling Workout Form:
- Input fields for distance, time, and elevation gain.

### Display Workouts:

- Show all logged workouts in a list, including the workout type and description.
- Display specific workout details depending on the type (running or cycling) in the list.

### Map Markers:

- Render map markers for each logged workout, indicating its location.
- Show workout details as popups when clicking on the markers.

### Local Storage:

- Store workout data locally using the Local Storage API, enabling persistent data even after the user leaves the app.

## Architecture

The application is built using JavaScript, HTML, and CSS. It follows an object-oriented approach, with the main components being:

- `Workout`: The base class representing a workout. It includes common properties and methods for running and cycling workouts.
- `Running`: A subclass of Workout specific to running workouts. It calculates pace based on distance and time.
- `Cycling`: A subclass of Workout specific to cycling workouts. It calculates speed based on distance and time.
- `App`: The main application class responsible for handling user interactions, map rendering, form submissions, and local storage management.

## Development Steps

The development of the Mapty app can be broken down into the following steps:

1. Set up the basic HTML and CSS structure for the application.
2. Implement the JavaScript classes for Workout, Running, and Cycling, including the necessary methods and properties.
3. Utilize the Geolocation API to obtain the user's current location and render a map.
4. Create forms for entering workout details and handle form submissions.
5. Display logged workouts in a list and on the map as markers with popups.
6. Implement local storage to save workout data and retrieve it when the user returns to the app.

By following these steps, the Mapty app will be fully functional, allowing users to log and track their cycling and running workouts with ease.

<i>Please note that the architecture, flowchart, and development steps are still placeholders in this readme. You can add more detailed information, diagrams, and code snippets as needed while actually developing the application. Happy coding! If you have any questions or need further assistance, feel free to ask.</i>

## Note

<b>This project is part of Jonas Schmedtmann's Udemy course - `The Complete JavaScript Course 2023: From Zero to Expert!`</b>

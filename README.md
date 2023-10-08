# kwordle startup


## Elevator pitch

Have you ever wanted to play wordle, but also be able to compete with others? Kwordle gives players this experience with the live leaderboard that shows up during game play. With this webapp, you can challenge your word-solving skills, compete with friends, and track your progress over time. Whether you're a casual player or a serious word whiz, Kwordle offers a fun and interactive platform to play the classic word game and see how you stack up against other word enthusiasts. Join the wordplay revolution with Kwordle and embark on a journey of linguistic mastery!


## Design
<img width="924" alt="login page for kwordle" src="https://github.com/kschoonmaker32/startup/assets/143727292/ae2748db-5757-4495-ab28-b8e2e21e327e">

<img width="905" alt="gameplay screen for kwordle" src="https://github.com/kschoonmaker32/startup/assets/143727292/b7de89d6-a3cf-4114-9ec5-38707bff63db">

<img width="905" alt="leaderboard page for kwordle" src="https://github.com/kschoonmaker32/startup/assets/143727292/a564e8f8-e9bf-4138-9878-53734e70f3d5">

<img width="905" alt="personal stats for kwordle" src="https://github.com/kschoonmaker32/startup/assets/143727292/cd81b71c-6898-467e-943b-deb253366513">


## Key Features
- login page for easy account access
- gameplay page with keyboard on screen to demonstrate letter status
- updated leaderboard on right of gameplay page (not pictured)
- results get posted to leaderboard as well as personal stats


### Technologies

I will use the required technologies in the following ways.

- **HTML** - Uses correct HTML structure for application. Four HTML pages. One for logging in, one for actual gameplay, one for the overall leaderboard, and one for personal stats from the game.
- **CSS** - Distinct application style that is consistent throughout entire startup to show a cohesive and organized webapp.
- **JavaScript** - Provides login, game updates and time, leaderboard and stats, and backend endpoint calls.
- **Service** - Backend service with endpoints for:
  - login
  - retrieving word for game
  - submitting score, date, time
  - retrieving personal stats from previous games
  - retrieving leaderboard stats from all users' stats
- **DB** - Store users, words for game, user stats, overall stats.
- **Login** - Register and login players. Credentials securely stored in database. Can't play unless authenticated.
- **WebSocket** - As each user plays, their date and gameplay time are added to a dynamic leaderboard.
- **React** - Application will use the React web framework.

## HTML deliverable

The structure of my application will use HTML.

- **HTML pages** - Four HTML page that represent the ability to login, play kwordle, then view personal stats as well as the overall leaderboard.
- **Links** - The login page automatically links to the gameplay page. After game is complete or if user clicks on 'quit,' the page will link to the personal stats page and then to the leaderboard page.
- **Text** - There will be a description of how to play the game in text on the login page. There will also be text within the stats and leaderboard pages.
- **Images** - On the leaderboard page, a gold medal image will be next to the top listing on the leaderboard.
- **Login** - Input box and submit button for login.
- **Database** - The words used in the game will be stored in a database. Players' stats will also be in the database.
- **WebSocket** - The leaderboard will show the realtime stats as players complete their game.

## CSS deliverable

For this deliverable I will use css to consistently style the webpages of the kwordle game in a minimal and clean style with bold colors.

- **Header, footer, and main content body**
- **Navigation elements** - I will use a standard hamburger nav element with simple styling.
- **Responsive to window resizing** - The app will function well on all screen sizes.
- **Application elements** - Clean lines, uncluttered text, and simple styling will be used throughout. Bold colors will be used for button elements.
- **Application text content** - A consistent sans serif font will be used throughout.
- **Application images** - Minimal images to keep the clean aesthetic - only one gold medal to be awarded to the player at the top of the leaderboard!

## JavaScript deliverable

Javascript is used in this webapp to make it interactive as the player logs in and plays the game.

- **login** - When you press enter or the login button it takes you to the game page.
- **database** - Will access database to get word being used in that day's game, then will write to the database a player's stats when they finish the game.
- **application logic** - The leaderboard will adjust to show the player's stats who finished games the fastest. During game play, the colors of the letters on the keyboard will change based on whether the user has already tried that letter.

## Service deliverable

For this deliverable I added backend endpoints that receives player stats and returns overall leaderboard info.

- **Node.js/Express HTTP service** - will be used for login
- **Backend service endpoints** - Placeholders for login that stores the current user on the server. Endpoints for storing player stats.

## DB deliverable

For this deliverable I stored the player stats and the words that are used in the game.

- **Player stats** - i will store the stats of each player and send the info to AWS
- **Word info** - store all word info in database

## Login deliverable

For this deliverable I associate the stats of each player with their login.

- **User registration** - Creates a new account in the game.
- **existing user** - Stores the stats under the same user if the user already exists.
- **Use DB to store player stats** - Stores both user and their stats

## WebSocket deliverable

For this deliverable I used webSocket to update the leaderboard in realtime as other players finish the game.

- **WebSocket data displayed** - All user stats will display in realtime as games are finished.

## React deliverable

For this deliverable I will use the React Framework to build the webapp. I am still learning the basic features of React, will update this section as I learn more.

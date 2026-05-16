# Gaming Database Platform
> Academic collaborative project originally developed in a team envrionment and currently maintained as a portfolio project.
A web application that allows users to discover and interact with games, follow content creators, and engage in community content. The app supports various user roles such as Admins, Regular Users, and Content Creators, each with their specific functionalities.

## Overview
Gaming Database Platform is a collaborative full-stack web application designed for game discovery, creator interaction, and community engagement. The platform supports multiple user roles including Admins, Regular Users, and Content Creators through role-based dashboards and authenticated functionality.

## Project Highlights
- Built using React, Spring Boot, Firebase Firestore, and REST APIs
- Supports role-based authentication and dashboards
- Includes game search, bookmarking, creator following, and admin reporting tools
- Structured with organized frontend/backend architecture
- Developed collaboratively using GitHub workflows

## My Contributions
As a contributor to this collaborative project, I supported application development, project organization, feature implementation, and documentation improvements. I contributed to frontend/backend integration efforts and helped support role-based functionality and user interaction features.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies](#technologies)
- [Folder Structure](#folder-structure)
- [Endpoints](#endpoints)
- [License](#license)

## Features

- **User Roles**: Supports Admins, Regular Users, and Content Creators.
- **Game Information**: Users can browse, search, and bookmark games.
- **Follow Content Creators**: Users can follow content creators and stay updated with their content.
- **Admin Features**:
  - Create reports such as user engagement, content interaction, and subscription trends.
  - Search, deactivate, or activate users.
- **Content Creator Features**: Content Creators can view and interact with their followers.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/game-app.git
   ```
2. Navigate to the project directory:
   ```sh
   cd game-app
   ```
3. Install the dependencies:
   ```sh
   npm install
   ```
4. Start the server:
   ```sh
   npm start
   ```

## Usage

### User Login and Registration

- **Login**: Users can log in using their credentials to access the relevant dashboard based on their role (Admin, User, or Content Creator).
- **Register**: New users can register, specifying their role.

### User Dashboard

- **Game Search**: Users can search for games and bookmark them.
- **Follow Content Creators**: Users can follow content creators to stay updated.
- **Bookmarks and Following**: Users can view the games they have bookmarked and the creators they are following.

### Admin Dashboard

- **User Management**: Admins can search, deactivate, or activate users.
- **Reporting**: Admins can create reports to analyze user engagement and content trends.

## Technologies

- **Frontend**: React, React Router, Axios
- **Backend**: Spring Boot, Firebase Firestore
- **Routing and State Management**: React Router, React Context API

## Folder Structure

```
.
├── src
│   ├── components
│   ├── context
│   ├── pages
│   │   ├── Login.js
│   │   ├── Register.js
│   │   ├── UserDashboard.js
│   │   ├── AdminDashboard.js
│   │   └── ContentCreatorDashboard.js
│   ├── services
│   ├── App.js
│   └── index.js
└── README.md
```

## Endpoints

### User Endpoints
- **Login**: `/api/auth/signin`
- **Register**: `/api/auth/signup`
- **Search Games**: `/api/user/games/search?keyword={keyword}`
- **Follow Content Creator**: `/api/user/content-creators/follow/{creatorId}`
- **Bookmark Games**: `/api/user/bookmark/{gameId}`

### Admin Endpoints
- **Search Users**: `/api/admin/users`
- **Activate/Deactivate User**: `/api/admin/users/{userId}/status`
- **Generate Reports**: `/api/admin/reports`

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.


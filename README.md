# Smart Solar Frontend

Frontend web application for the **Smart Solar Microgrid Trading System**

This repository contains only the React-based web frontend used for deployment on **Vercel**.

## Project Overview

Smart Solar is a client-server microgrid trading system that supports:

- Backoffice administration
- Grid Operator access
- User Management
- Prosumer Management
- Station and Microgrid Management
- Reservation Management
- Account and password management
- Operator dashboard functions
- Role-based access control

The frontend communicates with the centralized ASP.NET Core Web API through REST API calls.

## Technology Stack

- React
- Vite
- JavaScript
- Bootstrap 5
- Axios
- React Router
- Vercel

## Main Web Features

### Authentication and Account Management
- Backoffice and Grid Operator login
- Role-based protected routes
- Profile management
- Password change
- Forgot password
- Password reset

### User Management
- Create Backoffice and Grid Operator users
- Edit user details
- Activate and deactivate user accounts
- Filter and search users

### Prosumer Management
- View registered Prosumers
- View pending activation requests
- Activate Prosumers
- Deactivate Prosumers
- Reactivate deactivated accounts
- Search and filter Prosumer accounts

### Station Management
- Create microgrid stations
- Edit station details
- Address search and location selection
- Manage station capacity and slots
- Configure operating hours
- Activate and deactivate stations
- Search and filter stations

### Reservation Management
- View energy reservations
- Search reservations
- Filter by reservation status
- Approve pending reservations
- View booking information

### Grid Operator Dashboard
- View daily reservation statistics
- View pending, approved, completed and cancelled counts
- View station completion summaries
- View completed reservation history

## Project Structure

```text
src/
├── api/
│   └── apiClient.js
├── components/
│   ├── DashboardLayout.jsx
│   ├── ProtectedRoute.jsx
│   ├── StatCard.jsx
│   ├── StationAddressField.jsx
│   └── StatusBadge.jsx
├── pages/
│   ├── account/
│   ├── auth/
│   ├── backoffice/
│   └── operator/
├── services/
│   ├── accountService.js
│   ├── authService.js
│   ├── errorService.js
│   ├── operatorService.js
│   ├── prosumerService.js
│   ├── reservationService.js
│   ├── stationService.js
│   └── userService.js
├── App.jsx
├── main.jsx
└── index.css

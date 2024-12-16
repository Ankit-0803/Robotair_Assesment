# Robot Fleet Monitoring Dashboard

The **Robot Fleet Monitoring Dashboard** is a comprehensive tool designed to visualize the telemetry and status data of a fleet of robots. It delivers real-time updates and a responsive interface, enabling efficient monitoring of robot performance and locations.

## Features

### Core Functionalities
1. **Robot Overview**
   - Unique Robot Identifier (UUID)
   - Connection status: Online/Offline
   - Battery level
   - CPU utilization
   - RAM usage
   - Last updated time
   - Location details (latitude and longitude)

2. **Live Updates**
   - Implements WebSockets or periodic polling to refresh data every 5 seconds.

3. **Map Integration**
   - Displays robot locations on a map using tools like **Leaflet.js** or **Mapbox**.

4. **Alert System**
   - Highlights specific conditions:
     - Robots that are offline
     - Low battery levels (<20%)

### Additional Features
- Deployed frontend using **Netlify** and backend via **Heroku/Render**.
- Docker support for simplified deployment.
- Filtering options to view robots by status (active, offline, or low battery).

## Technologies Used

### Frontend
- **React.js**: Powers the responsive and user-friendly interface.
- **Leaflet.js**/ **Mapbox**: Provides real-time map-based visualization.

### Backend
- **FastAPI**: Handles the simulation and delivery of telemetry data.
- **WebSockets**: Ensures real-time communication.
- **Mock Data**: Generated from `fake_robot_data.json`.

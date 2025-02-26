# Horizon: Disaster Response and Emergency Management System

Horizon is a comprehensive mobile application designed to provide critical support during natural disasters and emergencies. By combining real-time disaster tracking, emergency service location, and user profile management, Horizon empowers both individuals seeking assistance and emergency service providers.

## 🌊 Features

### For Individuals
- **Real-time Disaster Tracking**: Monitor nearby natural disasters including wildfires, floods, earthquakes, and more.
- **Emergency Services Locator**: Find nearby hospitals, shelters, and blood donation centers with distance information.
- **SOS Emergency Call**: Quick access button to contact emergency services.
- **Personal Health Profile**: Store critical health information for emergency responders.

### For Emergency Service Providers
- **Client Management Dashboard**: Track and manage emergency response clients.
- **Alert Management System**: Receive and respond to emergency alerts in real-time.
- **Service Coverage Visualization**: View service coverage and gaps on an interactive map.

## 📱 Technologies

### Frontend (Mobile App)
- React Native
- Expo
- TypeScript
- React Native Maps
- Axios

### Backend
- Node.js
- Express
- MongoDB
- JWT Authentication

### Admin Dashboard
- Streamlit (Python)

### External APIs
- NASA EONET (Earth Observatory Natural Event Tracker)
- GDACS (Global Disaster Alert and Coordination System)
- OpenStreetMap (via Overpass API)

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Python 3.7+ (for admin dashboard)
- MongoDB account

### Installation

#### Mobile App (Horizon)
```bash
# Navigate to the mobile app directory
cd Horizon

# Install dependencies
npm install

# Start the development server
npm start
```

#### Backend Server
```bash
# Navigate to the backend directory
cd backend

# Install dependencies
npm install

# Start the server
node server.js
```

#### Admin Dashboard
```bash
# Navigate to the streamlit directory
cd streamlit

# Install dependencies
pip install -r requirements.txt

# Run the dashboard
streamlit run app.py
```

## 🔧 Configuration

1. Create a `.env` file in the backend directory with the following variables:
   ```
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

2. Update the API base URL in the mobile app:
   - Open `Horizon/app/index.tsx`
   - Update the API URLs to point to your backend server

## 💡 How It Works

1. **Disaster Data Collection**: The system aggregates data from multiple sources (EONET, GDACS) to provide comprehensive disaster information.

2. **Location Services**: When a user opens the app, their location is determined (with permission) to find nearby emergency services and disasters.

3. **Emergency Services Mapping**: The app identifies nearby hospitals, shelters, and blood donation centers using the OpenStreetMap API.

4. **Alert System**: Emergency service providers can receive and manage alerts through the admin dashboard.

## 📊 Project Structure

- `/Horizon`: React Native mobile application
  - `/app`: Main application entry points
  - `/components`: Reusable UI components
  - `/assets`: Images and fonts

- `/backend`: Node.js/Express server
  - `/routes`: API endpoint definitions
  - `/models`: MongoDB data models
  - `/middleware`: Authentication and other middleware
  - `/utils`: Utility functions for disaster data processing

- `/streamlit`: Python-based admin dashboard

## 🔗 Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/amazing-feature`).
3. Commit your changes (`git commit -m 'Add some amazing feature'`).
4. Push to the branch (`git push origin feature/amazing-feature`).
5. Open a Pull Request.

## 📝 License

This project was created for HackUTA 6 hackathon. All rights reserved.

## 🙏 Acknowledgements

- NASA EONET API for disaster data
- GDACS for global disaster alerts
- OpenStreetMap for location data
- HackUTA 6 organizers and mentors

## 🏆 Hackathon Participation

Horizon was developed during the HackUTA 6 hackathon, held on October 12-13, 2024, at the University of Texas at Arlington. HackUTA is one of North Texas' largest hackathons, offering a 24-hour marathon for students to collaborate and innovate on software projects. ([hackuta.org](https://www.hackuta.org/))

During the event, our team focused on addressing the challenges of disaster response and emergency management. Leveraging real-time data from NASA's EONET and GDACS, we aimed to create a tool that could assist both individuals in crisis and the emergency services that support them.

Participating in HackUTA 6 provided us with invaluable experience, mentorship, and the opportunity to bring Horizon from concept to reality within a collaborative and competitive environment.

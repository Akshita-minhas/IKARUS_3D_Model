# 3D Model Viewer

## Overview
A full-stack web application to view, interact with, and upload 3D models using **React, Three.js, Node.js, Express, and Firebase**.

## Features
- **Frontend**
  - Displays 3D models using React Three Fiber.
  - Interactive controls (rotate, zoom, pan).
  - Search bar to filter models.
- **Backend**
  - Express.js API with Firebase Firestore.
  - Endpoints for fetching and uploading models.
- **Database**
  - Firebase Firestore stores model metadata.
  - Firebase Storage (optional) for file hosting.

## Tech Stack
- **Frontend:** React, TypeScript, Three.js, React Three Fiber, TailwindCSS
- **Backend:** Node.js, Express, Firebase Firestore
- **Database:** Firebase Firestore

## Setup Instructions
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/3dmodel-viewer.git
cd 3dmodel-viewer
```

### 2. Install Dependencies
#### Frontend
```bash
cd myapp
npm install
npm start
```
#### Backend
```bash
cd backend
npm install
node server.js
```

### 3. Configure Firebase
- Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
- Enable Firestore and Storage.
- Download `serviceAccountKey.json` and place it in the `backend/` folder.

### 4. API Endpoints
#### Fetch Models
```http
GET /models
```
#### Upload Model
```http
POST /upload
Content-Type: application/json
{
  "name": "Model Name",
  "url": "Model URL",
  "description": "Optional description"
}
```

## Contributing
Pull requests are welcome. For major changes, open an issue first to discuss.

## License
[MIT License](LICENSE)

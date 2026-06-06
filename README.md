# EventGo

## 1. Brief About the Platform
**EventGo** is a full-stack event booking web application built using the MERN stack (MongoDB, Express.js, React, Node.js)[cite: 1, 2]. The platform provides a seamless end-to-end user experience for discovering and registering for events, backed by secure OTP (One-Time Password) email verification and JWT authentication[cite: 1]. It features an intuitive client interface alongside a comprehensive Admin Panel equipped with data visualization charts for tracking revenue, managing event lifecycles via complete CRUD operations, and modifying ticket registration statuses in real-time.

---

## 2. Environment & Toolchain Configuration
1. Install Node.js Runtime Engine (LTS Release version) from the formal system dashboard locally to inherit native npm script environments[cite: 3].
2. Set up local MongoDB Community Server Edition hosting platform binaries, ensuring default connection strings route through localhost port 27017, or orchestrate an active cloud instance string on MongoDB Atlas[cite: 3].
3. Verify standard local system text editors (Visual Studio Code recommended) and install critical extensions including ESLint and Prettier for strict schema style consistency[cite: 3].
4. Download and install Postman Desktop client tools to manage endpoint verification arrays, authentication headers, and request body parameters tracking[cite: 3].
5. Configure system Git profiles globally, ensuring local development branches cleanly synchronize references with remote repositories[cite: 3].
6. Configure production SMTP Mail Relays by opening target account controls on Google Accounts, validating 2-Step Verification protocols, and establishing a dedicated secure 16-character App Password key[cite: 3].

---

## 3. Core Systems Package Architecture Manifest

### Backend / API Server Architecture Core Package Arrays
```bash
npm install express mongoose dotenv cors bcryptjs jsonwebtoken nodemailer body-parser
npm install --save-dev nodemon
```
# Frontend / Presentation UI Workspace Application Infrastructure
```bash
npm install axios react-router-dom react-hot-toast lucide-react react-chartjs-2 chart.js
```

EventGo-MERN/                        # Root Monorepository Workspace Container
├── server/                            # Core Backend Web Server Module Node Context
│   ├── config/                        # Shared Infrastructure Data Layer Configurations
│   │   └── db.js                      # Main MongoDB Connection Interface Setup
│   ├── controllers/                   # Core Module Routing Implementation Business Logic
│   │   ├── authController.js          # Authentication Strategy Control Logics (Sign-In, Verification)
│   │   ├── eventController.js         # Administration & Creation Matrix Business Endpoints
│   │   └── bookingController.js       # Transactional Validation Routines
│   ├── models/                        # Object Modeling Schemas mapping to Mongoose Schemas
│   │   ├── User.js                    # User Profiles Schema definitions
│   │   ├── Event.js                   # Events Information Matrix fields Mapping
│   │   └── Booking.js                 # Transactional Ticket Registration Records
│   ├── routes/                        # API Pipeline Target URI Routers Definition Layers
│   ├── middleware/                    # HTTP Transaction Guard Interceptor Plugins
│   │   ├── authMiddleware.js          # User Token Validation Strategy
│   │   └── adminMiddleware.js         # Higher-Level Access Control Check
│   ├── utils/                         # Helper Framework Wrappers
│   │   └── mailer.js                  # SMTP Email Service Interface Definition
│   └── index.js                       # Primary Application Startup Hub Context Entry
└── client/                            # Complete Web Client Layer Configuration Directory
    ├── src/                           # Source Application Runtime Presentation Layer Assets
    │   ├── components/                # Modular Reusable Interface Control Components
    │   ├── pages/                     # Full Render Views Template Context Containers
    │   ├── context/                   # Context Global Application State Storage
    │   ├── utils/                     # Pre-Configured Axios Interceptor Core Service Plugins
    │   └── App.jsx                    # Routing Pipeline Assembly Setup
    └── main.jsx                       # Application Bootstrap Initializer Context Script

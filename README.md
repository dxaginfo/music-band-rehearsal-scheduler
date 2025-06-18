# Rehearsal Scheduler

A web application designed to help bands and music groups efficiently organize rehearsals, track attendance, send reminders, and suggest optimal rehearsal times based on member availability.

## Features

- **User Management** - Registration, authentication, and role-based access
- **Band/Group Management** - Create and manage multiple bands and members
- **Rehearsal Scheduling** - Create, edit, and manage rehearsal events
- **Availability Tracking** - Set regular and exception-based availability
- **Optimal Time Suggestion** - Smart algorithm to find the best rehearsal times
- **Attendance Tracking** - RSVP system with history and statistics
- **Notifications & Reminders** - Email notifications for upcoming rehearsals
- **Setlist Management** - Create and track rehearsal setlists
- **Resource Sharing** - Share sheet music, audio files, and notes
- **Calendar Integration** - Sync with external calendar systems

## Technology Stack

### Frontend
- React.js
- Redux for state management
- Material-UI components
- FullCalendar for calendar views
- Responsive design with mobile support

### Backend
- Node.js with Express
- RESTful API architecture
- JWT authentication
- PostgreSQL database with Sequelize ORM
- Redis for caching and real-time features

### DevOps
- Docker containerization
- AWS deployment (EC2, RDS)
- GitHub Actions for CI/CD
- Sentry for error monitoring

## Getting Started

### Prerequisites

- Node.js (v16+)
- npm or yarn
- PostgreSQL (v13+)
- Redis

### Installation

1. Clone the repository:
```bash
git clone https://github.com/dxaginfo/music-band-rehearsal-scheduler.git
cd music-band-rehearsal-scheduler
```

2. Install dependencies:
```bash
# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install
```

3. Configure environment variables:
```bash
# Copy the example environment file
cp .env.example .env

# Edit the .env file with your local configuration
```

4. Set up the database:
```bash
# Run migrations
cd server
npm run db:migrate

# (Optional) Seed the database with sample data
npm run db:seed
```

5. Start the development servers:
```bash
# Start the backend server
cd server
npm run dev

# In a separate terminal, start the frontend development server
cd client
npm start
```

6. Visit `http://localhost:3000` in your browser

## Project Structure

```
music-band-rehearsal-scheduler/
├── client/               # React frontend
│   ├── public/           # Static files
│   └── src/              # React components and logic
│       ├── components/   # Reusable UI components
│       ├── pages/        # Page components
│       ├── redux/        # Redux state management
│       ├── services/     # API services
│       └── utils/        # Utility functions
├── server/               # Node.js backend
│   ├── config/           # Configuration files
│   ├── controllers/      # Request handlers
│   ├── middleware/       # Express middleware
│   ├── models/           # Database models
│   ├── routes/           # API routes
│   ├── services/         # Business logic
│   └── utils/            # Utility functions
└── docker/               # Docker configuration
```

## API Documentation

The API documentation is available at `/api/docs` when running the development server. It includes detailed information about all available endpoints, request/response formats, and authentication requirements.

## Contributing

We welcome contributions to improve the Rehearsal Scheduler! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

Project Link: [https://github.com/dxaginfo/music-band-rehearsal-scheduler](https://github.com/dxaginfo/music-band-rehearsal-scheduler)
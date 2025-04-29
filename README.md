# EduTrack - Student Attendance System

EduTrack is a modern web-based student attendance management system that uses facial recognition technology to automate and streamline the attendance tracking process in educational institutions.

## Features

- **Facial Recognition Attendance**
  - Real-time face detection and recognition
  - Automated attendance marking
  - Support for multiple camera inputs
  - Privacy-focused processing

- **User Management**
  - Role-based access control (Admin/Student)
  - Student profile management
  - Course enrollment tracking
  - Secure authentication

- **Attendance Tracking**
  - Real-time attendance monitoring
  - Historical attendance records
  - Detailed attendance reports
  - Export functionality

- **Course Management**
  - Course creation and management
  - Instructor assignment
  - Schedule management
  - Student enrollment tracking

- **Dashboard & Analytics**
  - Visual attendance statistics
  - Course-wise attendance tracking
  - Attendance trend analysis
  - Performance insights

## Technology Stack

- **Frontend**
  - React 18
  - TypeScript
  - Tailwind CSS
  - Lucide React Icons
  - Face-api.js for facial recognition

- **Backend**
  - Supabase (Database & Authentication)
  - PostgreSQL
  - Row Level Security (RLS)

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v18 or higher)
- npm (v9 or higher)
- A modern web browser with camera access

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/edutrack.git
   cd edutrack
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Copy `.env.example` to `.env`
   - Update the Supabase configuration:
     ```
     VITE_SUPABASE_URL=your-supabase-url
     VITE_SUPABASE_ANON_KEY=your-supabase-anon-key
     ```

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:5173`

## Project Structure

```
edutrack/
├── public/
│   └── models/           # Face recognition models
├── src/
│   ├── components/       # Reusable UI components
│   ├── pages/           # Page components
│   ├── stores/          # State management
│   ├── utils/           # Utility functions
│   └── lib/             # Library configurations
├── supabase/
│   └── migrations/      # Database migrations
└── package.json
```

## Database Setup

1. Connect to Supabase:
   - Click the "Connect to Supabase" button in the top right
   - Follow the setup instructions

2. The database schema includes:
   - `profiles` - User profiles and roles
   - `students` - Student information
   - `courses` - Course details
   - `attendance` - Attendance records
   - `face_data` - Facial recognition data

## Development

- Run development server:
  ```bash
  npm run dev
  ```

- Build for production:
  ```bash
  npm run build
  ```

- Preview production build:
  ```bash
  npm run preview
  ```

## Security

- All database access is controlled through Row Level Security (RLS)
- Facial recognition data is processed locally
- User authentication is handled securely through Supabase
- Role-based access control for admin and student functions

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
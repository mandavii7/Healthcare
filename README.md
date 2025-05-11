# Healthcare Management System

A comprehensive web-based healthcare management solution built with React, TypeScript, and Supabase. This system helps healthcare providers manage patient data, appointments, and analytics efficiently.

## Features

- 📊 **Dashboard**: Real-time overview of key metrics and patient statistics
- 👥 **Patient Management**: Complete patient information management with medical history
- 📅 **Appointment Scheduling**: Track and manage patient appointments
- 📈 **Analytics**: Detailed insights into patient demographics and health trends
- 📋 **Reports**: Generate and export healthcare reports
- ⚙️ **Settings**: Customize system preferences and user settings

## Tech Stack

- **Frontend**: React, TypeScript, Tailwind CSS
- **State Management**: React Context
- **Data Visualization**: D3.js
- **Database**: Supabase
- **Icons**: Lucide React
- **Routing**: React Router
- **Date Handling**: date-fns

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Supabase account

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd healthcare-management-system
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add your Supabase credentials:
   ```
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

The application will be available at `http://localhost:5173`

### Database Setup

1. Connect to Supabase using the "Connect to Supabase" button in the top right corner
2. The database schema will be automatically created with the required tables:
   - patients
   - vital_signs
   - appointments
   - patient_conditions
   - medications

## Project Structure

```
src/
├── components/        # Reusable UI components
│   ├── charts/       # Data visualization components
│   ├── dashboard/    # Dashboard-specific components
│   ├── layout/       # Layout components
│   └── patients/     # Patient-related components
├── context/          # React Context providers
├── data/            # Mock data and data generation
├── lib/             # Utility functions and configurations
├── pages/           # Page components
└── types/           # TypeScript type definitions
```

## Features in Detail

### Patient Management
- Add, edit, and view patient records
- Track medical history and vital signs
- Manage appointments and follow-ups
- Monitor patient risk levels

### Analytics Dashboard
- Patient demographics visualization
- Admission trends analysis
- Vital signs monitoring
- Risk assessment metrics

### Appointment Management
- Schedule and track appointments
- View daily, weekly, and monthly calendars
- Filter appointments by status
- Manage follow-up visits

### Reporting
- Generate patient summary reports
- Track admission and discharge statistics
- Monitor healthcare metrics
- Export data in various formats

## Deployment

The application can be deployed to Netlify:

1. Build the application:
   ```bash
   npm run build
   ```

2. Deploy to Netlify:
   - Connect your GitHub repository to Netlify
   - Configure build settings:
     - Build command: `npm run build`
     - Publish directory: `dist`
   - Add environment variables in Netlify dashboard

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

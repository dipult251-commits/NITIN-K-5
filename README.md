# NITIN K-5 Attendance App

## Overview
A simple Android attendance marking application that allows users to mark their daily attendance with check-in and check-out functionality. The app records location data and stores attendance records in Firebase Realtime Database.

## Features
- ✅ **Easy Check-In/Check-Out**: Simple button-based attendance marking
- ✅ **Location Tracking**: Captures GPS location during attendance marking
- ✅ **Attendance History**: View all attendance records with date and time
- ✅ **Self-Service**: No login system required - designed for NITIN K
- ✅ **Real-time Database**: Uses Firebase Realtime Database for data storage
- ✅ **Settings**: Ability to configure employee name
- ✅ **No Admin Panel**: Simplified for individual user attendance

## Tech Stack
- **Language**: Java
- **Platform**: Android (API Level 21+)
- **Database**: Firebase Realtime Database
- **Location Services**: Google Play Services (FusedLocationProviderClient)
- **UI Framework**: Android Material Design

## App Structure

### Activities
1. **MainActivity** - Main attendance marking screen
2. **HistoryActivity** - View attendance history
3. **SettingsActivity** - Configure employee details

### Models
- **AttendanceRecord** - Data model for attendance records
- **AttendanceAdapter** - ListView adapter for displaying records

## Permissions Required
- `INTERNET` - For Firebase connectivity
- `ACCESS_FINE_LOCATION` - For GPS location access
- `ACCESS_COARSE_LOCATION` - For network-based location access
- `CAMERA` - Optional for future photo verification

## Firebase Setup
1. Create a Firebase project
2. Enable Realtime Database
3. Download `google-services.json`
4. Place it in `app/` directory

## Database Structure
```
attendance/
├── {date}
│   ├── {recordId}
│   │   ├── employee_name: "NITIN K"
│   │   ├── type: "Check-In" or "Check-Out"
│   │   ├── time: "HH:mm:ss"
│   │   ├── latitude: 28.1234
│   │   ├── longitude: 77.5678
│   │   └── timestamp: 1234567890
```

## Installation & Setup
See [INSTALLATION.md](INSTALLATION.md) for detailed setup instructions.

## Usage
1. **Check-In**: Press the green "CHECK IN" button when arriving
2. **Check-Out**: Press the red "CHECK OUT" button when leaving
3. **View History**: Click "View History" to see all attendance records
4. **Settings**: Modify employee name in settings if needed

## Owner
**DIPUL TIWARI**

## License
This project is proprietary and for exclusive use.

## Support
For issues or improvements, please contact the development team.

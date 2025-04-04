# Student Attendance System

A webcam-based facial recognition system for tracking student attendance in multiple classes. This application allows instructors to register students with their facial data and automatically log their attendance when they appear on camera.

## Features

- **Face Recognition**: Automatically identifies students using webcam facial recognition
- **Student Registration**: Easy process to register new students with their facial data
- **Multiple Classes**: Support for multiple class sections with separate attendance logs
- **Visual Identification**: Real-time display of student names on detected faces
- **Attendance Management**: View, filter, and clear attendance records
- **Offline Functionality**: Uses browser storage to work without internet connection
- **Privacy-Focused**: All data stored locally on the user's device

## Technologies Used

- React: Frontend framework
- Vite: Build tool and development server
- IndexedDB: Browser-based database for storing student and attendance data
- face-api.js: Facial detection and recognition library
- GitHub Pages: Hosting platform

## Usage Guide

### Setting Up Classes

1. When you first open the application, click "Add Class" to create your first class
2. Enter a name for the class (e.g., "Math 101", "Biology Section A")
3. Use the dropdown menu to switch between classes

### Registering Students

1. Select the appropriate class from the dropdown
2. Click "Start Camera" to activate your webcam
3. Click "Register New Student"
4. Position the student's face in the camera view
5. When their face is detected, click "Take Photo"
6. Enter the student's name
7. Click "Register Student"

### Taking Attendance

1. Select the class
2. Start the camera
3. As students enter the camera view, the system will:
   - Display their name on their face in the video
   - Automatically log their attendance (once per day per class)
   - Show a notification when attendance is recorded for the first time

### Viewing Attendance Records

1. Click the "Attendance Log" tab
2. View attendance records organized by date
3. Records are filtered by the currently selected class

### Managing Data

1. Click the "Manage Data" tab
2. Use the provided options to:
   - Delete individual students (hover over student cards)
   - Delete all students
   - Clear attendance for a specific class
   - Clear all attendance records

## Data Privacy

- All data is stored locally in your browser's IndexedDB
- No data is transmitted to external servers
- If you clear your browser data, the attendance records will be lost

## Troubleshooting

- **Camera Access Issues**: Make sure you've granted camera permissions to the website
- **Face Detection Problems**: Ensure adequate lighting and clear face visibility
- **Performance Issues**: Try closing other applications that might be using your webcam

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
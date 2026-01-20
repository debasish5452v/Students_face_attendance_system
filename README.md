# Face-Based Student Attendance System

A Django web application for automated employee/student attendance using face recognition. Supports webcam and IP camera sources, live recognition, attendance logging, and admin management.

## Features
- Register employees/students with face image capture
- Live attendance marking via webcam or IP camera
- Face recognition using facenet-pytorch and OpenCV
- Attendance check-in/check-out with duration calculation
- Admin dashboard for managing users, attendance, and camera configs
- Downloadable attendance reports (CSV)
- Camera configuration (name, source, threshold)
- Secure login/logout for admin access

## Technologies Used
- Django 5.x
- facenet-pytorch, OpenCV, dlib, face-recognition
- SQLite (default) or PostgreSQL (production)
- HTML/CSS/JS (custom templates)
- Python 3.10+

## Setup Instructions
1. **Clone the repository**
2. **Install dependencies**:
   ```sh
   pip install -r requirements.txt
   ```
3. **Apply migrations**:
   ```sh
   python manage.py migrate
   ```
4. **Create a superuser**:
   ```sh
   python manage.py createsuperuser
   ```
5. **Run the development server**:
   ```sh
   python manage.py runserver
   ```

##Dashboard
<img width="1349" height="595" alt="Dashboard" src="https://github.com/user-attachments/assets/35927252-4abc-4989-a011-ab9d5e45c7f3" />

##Attandance record
<img width="1362" height="597" alt="attandance record" src="https://github.com/user-attachments/assets/90155955-c96d-4b0e-897c-5a93be40a3f5" />

##Camera configuration
<img width="1365" height="596" alt="camera config" src="https://github.com/user-attachments/assets/4ad91e1f-e414-4c8b-bac1-aed94c48aa94" />

##Employee Lists
<img width="1350" height="601" alt="employee list" src="https://github.com/user-attachments/assets/f0ebbd1d-3b6e-40d4-9f97-e9c54917db22" />




## Camera Configuration
- Go to Camera Config in the dashboard
- For webcam: use `0` (or `1`, `2` for multiple webcams)
- For IP camera: use full URL (e.g. `http://ip:port/video`)
- Set recognition threshold (default: 0.6)

## Attendance Marking
- Go to "Mark Attendance" in the dashboard
- The camera window will open for live recognition
- Recognized faces are logged with check-in/check-out times

## Admin Features
- Authorize/de-authorize users
- Delete users
- View attendance logs
- Download attendance reports
- Manage camera configurations

## License
MIT

---
For troubleshooting camera issues:
- Ensure camera is connected and accessible
- Check IP/port for IP cameras
- Grant necessary permissions
- Consult camera manual if needed

---
**Developed by debasish5452v**

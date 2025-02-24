# DuolCheck - Event Attendance Monitoring System  

## 1. Project Overview  
DuolCheck is a mobile web-based event attendance monitoring system designed to simplify event tracking, feedback collection, and survey participation. The system allows organizers to manage events, track attendance, generate attendance reports based on departments and courses, and collect real-time feedback from participants while ensuring efficient logging and user activity tracking.  

## 2. Technologies Used  

### Backend  
- **Django (Python)** – Web framework for backend logic  
- **PostgreSQL** – Database management system  

### Frontend  
- **HTML, CSS, JavaScript**  
- **Bootstrap** – For basic UI components  
- **Tailwind CSS** – For utility-first styling  
- **DaisyUI** – For pre-designed UI components based on Tailwind CSS  

### Hosting & Cloud Services  
- **Render** – For Django app deployment  
- **PostgreSQL** – Managed database on Render  
- **Cloudinary** – For media and file storage (e.g., profile pictures, QR codes)  
- **Mapbox API** – For event location mapping  

## 3. Features  

### Event Management  
- Create, update, and delete events  
- Set event details (name, date, location, organizer, etc.)  
- Event status tracking  

### Attendance Monitoring  
- QR code-based check-in system  
- User authentication for attendance tracking  
- Logs for registered and anonymous attendees  

### Survey & Feedback System  
- Dynamic survey creation for events  
- User and anonymous feedback collection  
- Ratings and text-based feedback submission  

### User & Admin Management  
- User authentication and role-based access  
- Admin dashboard for monitoring logs and events  
- System settings for theme preference, maintenance mode, and notifications  

### Attendance Reporting & Exports  
- Generate **attendance reports** categorized by **college department and course**  
- **Export reports in CSV or PDF format** for documentation and analysis  
- Filter attendance records based on **event, date, department, and course**  

### Logging & Analytics  
- System logs for admin actions  
- User activity logs with IP tracking  
- Anonymous user logs for tracking general usage  

## 4. Deployment & Production Configuration  

### Hosting & Database  
- Deployed on **Render** with a managed **PostgreSQL** instance  
- Uses **Gunicorn** as the WSGI HTTP server for production  

### Media & File Handling  
- **Cloudinary** is used to store profile pictures and event-related media  
- Uploaded QR codes for verification are also handled via Cloudinary  

### Map & Location Services  
- **Mapbox API** is integrated for event location visualization and navigation assistance  

### Attendance Report Exporting  
- **Django ReportLab or Pandas** is used for generating PDF/CSV reports  
- **Export filters** allow for generating reports per department and course  

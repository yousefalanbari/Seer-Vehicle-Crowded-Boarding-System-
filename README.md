Seer – Intelligent Vehicle Monitoring System

Graduation Project | Computer Engineering | King Saud University

Project Overview

Seer is an AI-powered, real-time vehicle monitoring system designed to improve traffic management in Pick-Up and Drop-Off (PUDO) areas.

The system uses computer vision and object detection to identify vehicles, track their movements, monitor waiting times, and detect traffic violations automatically.

Seer aims to improve traffic flow, reduce congestion, and support efficient management of designated vehicle lanes.

Key Features

* Real-Time Vehicle Detection: Detects vehicles using YOLOv8.
* Vehicle Tracking: Tracks vehicle movements across monitored lanes.
* Excessive Waiting Detection: Identifies vehicles exceeding the permitted waiting time.
* Improper Lane Change Detection: Detects unauthorized movement between designated lanes.
* Illegal Stopping Detection: Identifies vehicles stopping in restricted transit lanes.
* Overtime Parking Detection: Monitors vehicles exceeding parking duration limits.
* Web Dashboard: Displays monitoring information and detected violations.
* Violation Records: Stores violation information and snapshots for review.

Technologies Used

Technology	Purpose
Python	Backend development and processing
YOLOv8	Vehicle detection
OpenCV	Computer vision and vehicle tracking
Flask	Web application and API
SQLite	Violation data storage
HTML, CSS, JavaScript	Web dashboard
Server-Sent Events (SSE)	Real-time dashboard updates

System Architecture

The system follows a computer vision processing pipeline:

1. Video Input: Receives video footage from the monitored area.
2. Vehicle Detection: YOLOv8 identifies vehicles in each frame.
3. Vehicle Tracking: OpenCV-based processing tracks vehicles and their movements.
4. Violation Detection: The system evaluates vehicle behavior against predefined traffic rules.
5. Data Storage: Detected violations and associated information are recorded.
6. Web Dashboard: Flask provides monitoring interfaces and real-time updates.

Traffic Violation Rules

Violation	Detection Rule
Excessive Waiting Time	Leading vehicle in Lane 1 exceeds 20 seconds
Improper Lane Change	Vehicle moves between Lane 1 and Lane 2
Illegal Stopping	Vehicle remains below 3 km/h for more than 2 seconds in transit lanes
Overtime Parking	Vehicle remains in Lane 4 for more than 5 seconds

Project Structure

Seer/
├── main.py
├── vision_tracker.py
├── violation_engine.py
├── storage_manager.py
├── lanes_config.json
├── README.md
└── templates/
    ├── index.html
    ├── database.html
    ├── laner.html
    ├── leader.html
    ├── timer.html
    └── violation.html

Project Components

main.py: Flask application and system integration.

vision_tracker.py: Vehicle detection and tracking functionality.

violation_engine.py: Traffic violation detection logic.

storage_manager.py: Violation records and data management.

lanes_config.json: Lane configuration settings.

templates/: HTML pages for the monitoring dashboard and related interfaces.

Project Team

* Yousef Abdulkarim Alanbari
* Khalid Al Asmari
* Abdulrahman Alshehri
* Rayyan Abuamara

Project Supervisor: Dr. Ayed Alqahtani

Institution: King Saud University – College of Engineering

Project Purpose

Seer demonstrates the integration of artificial intelligence, computer vision, backend development, and real-time monitoring to address traffic management challenges in high-density vehicle areas.

The project was developed as part of the Computer Engineering graduation requirements at King Saud University.


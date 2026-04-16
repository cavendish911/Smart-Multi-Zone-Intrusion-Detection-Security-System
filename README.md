🎯 Objectives
Build a real-time motion detection system
Implement multi-zone security monitoring
Develop time-based threat escalation (normal → danger mode)
Display live system status using LCD interface
Simulate real-world security system behavior
⚙️ Features
🟢 Multi-Zone Detection
Supports 2 independent motion detection zones:
Area 1 (PIR sensor 1)
Area 2 (PIR sensor 2)
Each zone operates independently
⏱ Real-Time Intrusion Timing
Tracks how long motion is detected per zone
Displays live duration on LCD screen
🚨 Danger Mode System
If motion continues for more than 10 seconds, system enters:
High alert state (DANGER MODE)
Escalates alarm intensity automatically
🔊 Adaptive Alarm System
Normal detection → steady tone
Danger mode → fast intermittent alarm
📊 Intrusion Logging
Counts number of detections per zone
Displays statistics when system is idle
🖥 LCD Interface
Real-time status updates:
System Safe
Target Area 1 / Area 2
DANGER alerts
Live timer display per zone
🔐 Software-Based System Control
System can be ARM/DISARM controlled via Serial Monitor:
arm
disarm
🧠 System Logic

The system operates using a state-based architecture:

Idle State → No motion detected
Active State → Motion detected in one or more zones
Escalation State → Motion duration exceeds threshold (10s)
Alert State → Buzzer + LCD warning activated
🛠 Technologies Used
Arduino UNO
Embedded C / Arduino IDE
PIR Motion Sensors
16x2 LCD Display (LiquidCrystal library)
Buzzer + LED indicators
📷 System Preview

(Add your images here)

Circuit setup
LCD output
Live detection demo

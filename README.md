# Real-Time Surveillance and Intrusion Detection 🚨  

This project focuses on developing a computer vision application that detects unauthorized intrusions in restricted zones and monitors truck activities at entry gates. It provides automated alerts and real-time monitoring to improve security and operational efficiency.  

---

## Features  
- Trespasser Detection: Identifies unauthorized individuals entering restricted zones.  
- Truck Surveillance: Monitors truck entries at gates and provides counts/alerts.  
- Real-Time Notifications: Sends immediate email alerts for intrusions or truck activity.  
- Interactive UI: Built with Streamlit for easy video upload, detection visualization, and results.  
- Data Insights: Generates reports on incidents to optimize security strategies.  

---

## Tech Stack  
- Python  
- YOLOv8 (Ultralytics) – real-time object detection  
- OpenCV – video processing  
- Streamlit – interactive user interface  
- SMTP (Email Service) – instant email alerts  
- FFmpeg, tqdm, tempfile, os, subprocess  

---

## Installation & Setup  
1. Clone the repository:  
   ```bash
   git clone https://github.com/username/trespasser-detection.git
   cd trespasser-detection

### How to run it on your own machine

1. Install the requirements

   ```
   $ pip install -r requirements.txt
   ```

2. Run the app

   ```
   $ streamlit run streamlit_app.py
   ```

## How It Works

1. Define regions of interest (ROI) in the video (restricted zones or entry gates).
2. The YOLOv8 model detects persons (ID:0) and trucks (ID:7).
3. On detection inside the ROI:
   -Trespasser → Intrusion alert + email notification
   -Truck → Truck count + alert notification

4.Results are displayed in the Streamlit app with processed video output.

---
## Future Improvements  
- Multi-camera integration for large-scale environments  
- Advanced trackers (BYTETrack, Norfair, Detectron2) 
- Cloud deployment for scalability  
- Integration with IoT devices for real-time alarms  











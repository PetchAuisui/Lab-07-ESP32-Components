# Lab 7-2: Managed Component from GitHub URL Demo

## คำอธิบาย
การทดลองนี้แสดงการใช้งาน managed component จาก GitHub Repository
ใช้ `Sensors` component จาก https://github.com/APPLICATIONS-OF-MICROCONTROLLERS/Lab7_Components

## ผลลัพธ์ที่คาดหวัง
- แสดงข้อความการเริ่มต้น sensor จาก GitHub component
- แสดงข้อมูล temperature และ humidity ทุก 4 วินาที
- แสดงสถานะการทำงานของ sensor
- แสดงแหล่งที่มาของ component (GitHub Repository)

## ความแตกต่างจาก Lab 7-1
- Lab 7-1: ใช้ local component (ในเครื่อง)
- Lab 7-2: ใช้ managed component จาก GitHub URL

## การใช้งาน
1. เข้าไปในโฟลเดอร์ lab7-2_Managed_url_Component
2. รันคำสั่ง `idf.py build` (จะดาวน์โหลด component จาก GitHub อัตโนมัติ)
3. ทดสอบด้วย QEMU
### ผลลัพธ์ที่ได้
```c
I (15910) LAB7-2: 📋 Reading #2 from GitHub Component
I (15910) SENSOR: 📊 Reading sensor data from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 18
I (15910) SENSOR: 🌡️  Temperature: 31.4°C
I (15910) SENSOR: 💧 Humidity: 95.5%
I (15910) SENSOR: ✅ Sensor status check from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 30
I (15910) SENSOR: 📈 All sensors operating normally
I (15910) LAB7-2: � Component Source: GitHub Repository
I (15910) LAB7-2: ==========================================
I (19910) LAB7-2: 📋 Reading #3 from GitHub Component
I (19910) SENSOR: 📊 Reading sensor data from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 18
I (19910) SENSOR: 🌡️  Temperature: 31.1°C
I (19910) SENSOR: 💧 Humidity: 70.1%
I (19910) SENSOR: ✅ Sensor status check from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 30
I (19910) SENSOR: 📈 All sensors operating normally
I (19910) LAB7-2: � Component Source: GitHub Repository
I (19910) LAB7-2: ==========================================
I (23910) LAB7-2: 📋 Reading #4 from GitHub Component
I (23910) SENSOR: 📊 Reading sensor data from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 18
I (23910) SENSOR: 🌡️  Temperature: 31.7°C
I (23910) SENSOR: 💧 Humidity: 89.3%
I (23910) SENSOR: ✅ Sensor status check from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 30
I (23910) SENSOR: 📈 All sensors operating normally
I (23910) LAB7-2: � Component Source: GitHub Repository
I (23910) LAB7-2: ==========================================
I (27910) LAB7-2: 📋 Reading #5 from GitHub Component
I (27910) SENSOR: 📊 Reading sensor data from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 18
I (27910) SENSOR: 🌡️  Temperature: 26.5°C
I (27910) SENSOR: 💧 Humidity: 98.1%
I (27910) SENSOR: ✅ Sensor status check from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 30
I (27910) SENSOR: 📈 All sensors operating normally
I (27910) LAB7-2: � Component Source: GitHub Repository
I (27910) LAB7-2: ==========================================
```
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/ab0dde46-947b-4c9d-b9ad-2a59c8376fe3" />

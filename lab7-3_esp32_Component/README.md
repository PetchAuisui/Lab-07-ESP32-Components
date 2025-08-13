# Lab 7-3: Custom ESP32 Components (Sensor + Display)

## คำอธิบาย
การทดลองนี้แสดงการสร้าง component ใหม่ด้วยคำสั่ง `idf.py create-component`
สร้าง 2 components:
1. **Sensor Component** - อ่านค่า temperature, humidity และคำนวณ heat index
2. **Display Component** - แสดงผลข้อมูลในรูปแบบตาราง

## โครงสร้างโฟลเดอร์หลังใช้ create-component
```
lab7-3_esp32_Component/
├── CMakeLists.txt
├── components/
│   ├── sensor/
│   │   ├── CMakeLists.txt
│   │   ├── include/
│   │   │   └── sensor.h
│   │   └── sensor.c
│   └── display/
│       ├── CMakeLists.txt
│       ├── include/
│       │   └── display.h
│       └── display.c
├── main/
│   ├── CMakeLists.txt
│   └── lab7-3.c
├── build/
└── README.md
```
## ผลลัพธ์ที่ได้
```c
I (14533) LAB7-3: 📋 Reading #2
I (14533) DISPLAY: 🧹 Display cleared
I (14533) DISPLAY: 
I (14533) ENHANCED_SENSOR: 🌡️  Temperature: 30.20°C
I (14533) ENHANCED_SENSOR: 💧 Humidity: 69.80%
I (14533) LAB7-3: 🔥 Heat Index: 65.10
I (14533) DISPLAY: ┌─────────────────────────────────┐
I (14533) DISPLAY: │        SENSOR DATA DISPLAY      │
I (14533) DISPLAY: ├─────────────────────────────────┤
I (14533) DISPLAY: │ 🌡️  Temperature:  30.20°C      │
I (14533) DISPLAY: │ 💧 Humidity:     69.80%       │
I (14533) DISPLAY: │ 🔥 Heat Index:   65.10        │
I (14533) DISPLAY: └─────────────────────────────────┘
I (14533) DISPLAY: ┌─────────────────────────────────┐
I (14533) DISPLAY: │         SYSTEM STATUS           │
I (14533) DISPLAY: ├─────────────────────────────────┤
I (14533) DISPLAY: │ Status: ✅ Comfortable         │
I (14533) DISPLAY: └─────────────────────────────────┘
I (14533) LAB7-3: ==========================================
I (20533) LAB7-3: 📋 Reading #3
I (20533) DISPLAY: 🧹 Display cleared
I (20533) DISPLAY: 
I (20533) ENHANCED_SENSOR: 🌡️  Temperature: 37.90°C
I (20533) ENHANCED_SENSOR: 💧 Humidity: 41.70%
I (20533) LAB7-3: 🔥 Heat Index: 58.75
I (20533) DISPLAY: ┌─────────────────────────────────┐
I (20533) DISPLAY: │        SENSOR DATA DISPLAY      │
I (20533) DISPLAY: ├─────────────────────────────────┤
I (20533) DISPLAY: │ 🌡️  Temperature:  37.90°C      │
I (20533) DISPLAY: │ 💧 Humidity:     41.70%       │
I (20533) DISPLAY: │ 🔥 Heat Index:   58.75        │
I (20533) DISPLAY: └─────────────────────────────────┘
I (20533) DISPLAY: ┌─────────────────────────────────┐
I (20533) DISPLAY: │         SYSTEM STATUS           │
I (20533) DISPLAY: ├─────────────────────────────────┤
I (20533) DISPLAY: │ Status: ✅ Comfortable         │
I (20533) DISPLAY: └─────────────────────────────────┘
I (20533) LAB7-3: ==========================================
```
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/8e4dcee5-60a5-4a66-984e-f8fa0b0b4a91" />

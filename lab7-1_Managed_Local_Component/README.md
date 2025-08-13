# Lab 7-1: Local Component Demo

## คำอธิบาย
การทดลองนี้แสดงการใช้งาน component ที่มีอยู่ในโฟลเดอร์ `components/Sensors/` ของ project

## สรุปคำสั่งที่ใช้ และผลลัพธ์ที่ได้
###  คำสั่งที่ใช้
#### เข้าใช้งาน Docker Container
```
# เริ่มต้น Docker Container
docker-compose up -d

# ตรวจสอบ Docker Container

docker-compose ps -a

# ดูว่ามี NAME เป็น esp32-lab7 หรือไม่

# เข้าใช้งาน Container
docker exec -it esp32-lab7 bash
```

#### เข้าไปใน project directory
```
cd lab7-1_Managed_Local_Component

#export environment เพื่อให้สามารถเรียกใช้ idf tools ได้
. $IDF_PATH/export.sh

# กำหนด target ESP32
idf.py set-target esp32

# Build project
idf.py build
```

### ผลลัพธ์ที่ได้
```c
I (19345) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (19345) SENSOR: 🌡️  Temperature: 27.2°C
I (19345) SENSOR: 💧 Humidity: 61.0%
I (19345) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (19345) SENSOR: 📈 All sensors operating normally
I (19345) LAB7-1: ----------------------------
I (22345) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (22345) SENSOR: 🌡️  Temperature: 35.4°C
I (22345) SENSOR: 💧 Humidity: 68.6%
I (22345) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (22345) SENSOR: 📈 All sensors operating normally
I (22345) LAB7-1: ----------------------------
I (25345) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (25345) SENSOR: 🌡️  Temperature: 30.3°C
I (25345) SENSOR: 💧 Humidity: 90.6%
I (25345) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (25345) SENSOR: 📈 All sensors operating normally
I (25345) LAB7-1: ----------------------------
I (28345) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (28345) SENSOR: 🌡️  Temperature: 25.7°C
I (28345) SENSOR: 💧 Humidity: 69.5%
I (28345) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (28345) SENSOR: 📈 All sensors operating normally
I (28345) LAB7-1: ----------------------------
I (31345) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (31345) SENSOR: 🌡️  Temperature: 33.8°C
I (31345) SENSOR: 💧 Humidity: 87.1%
I (31345) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (31345) SENSOR: 📈 All sensors operating normally
I (31345) LAB7-1: ----------------------------
I (34345) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (34345) SENSOR: 🌡️  Temperature: 29.5°C
I (34345) SENSOR: 💧 Humidity: 89.6%
I (34345) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (34345) SENSOR: 📈 All sensors operating normally
I (34345) LAB7-1: ----------------------------
I (37345) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (37345) SENSOR: 🌡️  Temperature: 29.1°C
I (37345) SENSOR: 💧 Humidity: 67.8%
I (37345) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (37345) SENSOR: 📈 All sensors operating normally
I (37345) LAB7-1: ----------------------------
```
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/e52d0cfb-91c3-40c6-8144-4d515af6ec61" />


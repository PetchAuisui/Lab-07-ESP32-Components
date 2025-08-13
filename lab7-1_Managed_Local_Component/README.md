<<<<<<< HEAD
    
=======
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
I (11417) main_task: Calling app_main()
I (11417) LAB7-1: 🚀 Lab 7-1: Local Component Demo Started
I (11417) SENSOR: 🔧 Sensor initialized from file: /project/components/Sensors/sensor.c, line: 12
I (11417) SENSOR: 📡 Sensor module ready for operation
I (11427) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (11427) SENSOR: 🌡️  Temperature: 34.1°C
I (11437) SENSOR: 💧 Humidity: 82.7%
I (11437) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (11447) SENSOR: 📈 All sensors operating normally
I (11447) LAB7-1: ----------------------------
I (14447) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (14447) SENSOR: 🌡️  Temperature: 30.9°C
I (14447) SENSOR: 💧 Humidity: 71.8%
I (14447) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (14447) SENSOR: 📈 All sensors operating normally
I (14447) LAB7-1: ----------------------------
I (17447) SENSOR: 📊 Reading sensor data from file: /project/components/Sensors/sensor.c, line: 18
I (17447) SENSOR: 🌡️  Temperature: 31.5°C
I (17447) SENSOR: 💧 Humidity: 78.7%
I (17447) SENSOR: ✅ Sensor status check from file: /project/components/Sensors/sensor.c, line: 30
I (17447) SENSOR: 📈 All sensors operating normally
I (17447) LAB7-1: ----------------------------
```
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/6a876deb-c8b3-4b00-8b4b-f4dad6b36e88" />




>>>>>>> 658c858a3a59817117be6b32dae8a635622fd786

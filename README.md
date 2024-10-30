
# แนวทางการทำงาน BLE ANCS Example

ble ancs Example เป็นบริการที่อนุญาตให้แอปพลิเคชันบนอุปกรณ์ที่ใช้ iOS รับการแจ้งเตือนจาก iPhone หรือ iPad โดยสามารถเข้าถึงข้อมูลแจ้งเตือน เช่น ชื่อผู้ส่งและเนื้อหาของข้อความได้

## การเลือก Example IDF

![สกรีนช็อต 2024-10-30 002540](https://github.com/user-attachments/assets/72d9d948-4cd2-4b22-a358-433df0bb9b21)

1. เลือก ESP-IDF

2. เลือก show example

3. พิมพ์คำว่า ble

4. เลือก ble_ancs

![สกรีนช็อต 2024-10-30 002349](https://github.com/user-attachments/assets/38330ce5-983c-422f-955e-616d014a85f8)


5. คลิกเลือก Create project using example ble_ancs


6. เมื่อสร้างแล้วจะได้ไฟล์ทั้งหมด ดังนี้

![สกรีนช็อต 2024-10-30 002403](https://github.com/user-attachments/assets/bfd5d8b8-4931-4b7e-8138-4f48f787b911)

## Build and Flash

7. เลือก com port

8. เลือก Build Flash and Monitor

9. เปิด Bluetooth บนอุปกรณ์ แล้วเชื่อมต่อบลูทูธกับบอร์ด ESP32

![image](https://github.com/user-attachments/assets/d36722e7-a78c-46ba-8054-c07f09c7f1af)


## ผลลัพท์

- Serial Moniter จะดักจับและแสดงการแจ้งเตือนจากโทรศัพท์

![image](https://github.com/user-attachments/assets/244edd27-9710-4772-b8b6-252a148a9a80)

## การแก้ไข

10. เลือกไฟล์ ble_ancs_demo.c

![image](https://github.com/user-attachments/assets/43932b93-d58a-4cc0-94ad-4208f57b4a71)

11. เพิ่มชื่อให้กับอุปกรณ์ที่จะเชื่อมต่อในบรรทัดที่ 13 และ 14  ดังนี้

```

#define BLE_ANCS_TAG  "BLE_ANCS"
#define EXAMPLE_DEVICE_NAME "BLE_ANCS_018"

```

## ผลลัพท์การแก้ไข

![image](https://github.com/user-attachments/assets/d3dc4766-ad0f-4a9d-994c-36b4c9502fe3)


![image](https://github.com/user-attachments/assets/36cf4a58-75da-41da-9dcd-1c047d2b6331)


![image](https://github.com/user-attachments/assets/f2214a21-0d2d-4b1f-bfb3-bdfb0e47f537)


![image](https://github.com/user-attachments/assets/1179cbaf-f6b4-41ba-81b8-e59341c45efb)

## สรุปผลการทดลอง

- การทดลอง BLE ANCS (Apple Notification Center Service) Example บน ESP32 เป็นการทดลองการใช้ Bluetooth Low Energy ในการรับข้อมูลการแจ้งเตือนจากอุปกรณ์ iOS ผ่าน Apple Notification Center Service 


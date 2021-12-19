#  LORA_RFM95_  

![image](https://user-images.githubusercontent.com/56969447/146666488-186c5896-cb30-4045-bb23-0362df57a72e.png)

I. **Tổng quan**
   - RFM915 là module truyền nhận dữ liệu sử dụng sóng LoRa được thiết kế bởi hãng Hope RF.
   - Module này có độ nhạy lên đến -148dBm đi kèm với bộ khuếch đại công suất +20dBm được thiết kế tích hợp.
   - Module này sử dụng nguồn cung cấp từ 1.8VDC – 3.7VDC với dòng tiêu thụ cao nhất lúc truyền là 120mA.
   - Sử dụng giao thức SPI.

II. **Sơ đồ chân**
   - Giao thức SPI. Ta sử dụng 6 chân là MOSI, MISO, SCK, NSS, RESET, DIO0, ngoài ra chọn 1 chân của STM làm chân MODE.
   - MOSI, MISO, SCK là chân của SPI.
   - NSS và RESET là OUTPUT và ban đầu để mức LOW.
   - DIO0 và MODE là INPUT.
   - Chân MODE sẽ cho phép chúng ta chọn chế độ Slave hay là Master. Chân này chúng ta sẽ nối với nút nhấn để chọn chế độ module LoRa.
   
III. **Code**

**Bước 1. Tạo project**

    - Cấu hình chân nạp code
    
![image](https://user-images.githubusercontent.com/56969447/146666540-16b13bb8-18f9-4641-9fad-f93845d234d8.png)

**Bước 2. Cấu hình giao tiếp SPI**

    - Chọn mode Full-Duplex Master, còn lại giữ nguyên.
    
![image](https://user-images.githubusercontent.com/56969447/146666633-6fc5e9d9-7018-4c5e-bd5a-ab62e7248fb4.png)

**Bước 3. Cấu hình các chân MOSI, MISO, SCK, NSS, RESET, DIO0, MODE**

   - MOSI, MISO, SCK là chân của SPI.
   - NSS và RESET là OUTPUT và ban đầu để mức LOW.
   - DIO0 và MODE là INPUT.
   - Chân MODE sẽ cho phép chúng ta chọn chế độ Slave hay là Master. Chân này chúng ta sẽ nối với nút nhấn để chọn chế độ module LoRa.
    
![image](https://user-images.githubusercontent.com/56969447/146666918-2fce6bc4-bd35-4979-b1c6-b6e20fa6c2b1.png)


  
  

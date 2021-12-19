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
  

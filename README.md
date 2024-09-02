วิธีใช้งาน script สำหรับกดบัตรคอนจาก Thaiticketmajor

1.สคริปข้ามยืนยันข้อตกลงการใช้งาน

2.สคริปเลือกรอบวันแสดง(ถ้ามี) //ปรับแต่งบรรทัดที่ 2
เช่น const dayToSelect = 'Mon';
ก็คือ Mon = วันจันทร์ อื่นๆ = Tue,Wed,Thu,Fri,Sat,Sun

3.สคริปเลือกโซนที่นั่งที่ต้องการ //ปรับแต่งบรรทัดที่ 2  
เช่น const zonePrefix = 'A1';
ก็คือที่นั่งโซน A1 *กรณีที่ใส่แค่ชื่อโซนเช่น A ระบบจากที่มีจำนวนที่นั่งเหลือเยอะสุดจากโซน A

4.สคริปหาที่นั่งติดกันอัตโนมัติเริ่มจากหน้าสุดไปหลังสุดตามจำนวนที่นั่งที่ต้องการ //ปรับแต่งบรรทัดที่ 2
เช่น const requiredSeats = 2;
ก็คือ เลือก 2 ที่นั่งติดกันแล้วไปหน้าใส่ชื่อ *กรณีที่ไม่มี 2 ที่ติดกันระบบจะรีเฟรชหน้าเว็บให้ลองใช้คำสั่งอีกครั้งเผื่อมีที่นั่งหลุดจองหรือแนะนำให้เปลี่ยนโซน

5.สคริปกรอกชื่อบนบัตรจากที่เตรียมไว้หลังจากนั้นจะต้องถัดไปเองเพื่อตรวจสอบด้วยตนเองอีกครั้ง
เช่น document.getElementById("txt_firstname_0").value = "Chiraphat chaikhuntod"; 
ก็คือชื่อสำหรับบัตรใบที่ 1 กรณีจองมากกว่า 1 ที่นั่งก็ให้ใส่ชื่อในบรรทัดถัดไปหลัง value="ใส่ชื่อ สกุลตรงนี้"

# Zen-Cart
ขั้นตอนการเพิ่มโมดูล Paysolutions สำหรับ Zen Cart


1.	อัพโหลดไฟล์ post_back_url.php ไว้ที่ rootPath เพื่อรับค่า จาก Paysolutions

2.	อัพโหลด folder includes\modules\payment\pasolutions ไว้ที่ rootPath\includes\modules\payment ที่โปรแกรมของท่าน
•	rootPath หมายถึง path ที่ไว้สำหรับวางโปรแกรม zen cart เช่น zencart\includes\modules\payment

3.	อัพโหลดไฟล์ includes\modules\payment\paysolutions.php ไปไว้ที่โปรแกรมของท่าน

4.	อัพโหลดไฟล์ includes\languages\english\payment\paysolutions.php ไปไว้ที่โปรแกรมของท่าน
•	ขั้นตอนที่ 1 – 3 ท่านต้องวาง path ของโฟล์เดอร์และไฟล์ให้ถูกต้อง

5.	Log in เข้า ระบบ Admin ของ Zencart 

6.	 ทำการเพิ่ม Currencies ให้มี เงิน บาท   เลือก ที่ เมนู  Localization -> Currencies -> new currency

7.	ให้ set ข้อมูลดังนี้

Title   =  Thai

Code  =  TH

Symbol Left   =   ฿

Symbol  Right  = ว่าง  ( หรือจะใส่ ฿ ก็ได้ )

Decimal Point  =   . (จุด)

Thousands Point  =  ,  (จุลภาค)

Decimal Places  = 2

Value  =  1

จากนั้นให้กด update 

8.	ทำการเพิ่ม สถานะของ การจ่ายเงิน  โดยเข้าที่เมนู Localization -> Orders Status -> insert

9.	 ให้ Set ข้อมูล ดังนี้  Orders Status -> insert

10.	เลือกหัวข้อ  Module  ->  Payment  

11.	ที่หัวข้อ  Payment จะมีเมนูของ PAYSOLUTIONS 

12.	 เมื่อเลือกหัวข้อ  PAYSOLUTIONS แล้ว ทางขวามือ จะมีปุ่ม install ให้เลือก  คลิกที่ ปุ่ม install  

13.	หลังจากกด install แล้ว จะปรากฎ ตัวให้กรอกรายละเอียดของ PAYSOLUTIONS module ขึ้นมา

14.	ให้ set ข้อมูลดังนี้

-	Enable Module : True *

-	Sort Order : 0 (ไม่จำเป็น)

-	Email Address : อีเมล์ของร้านค้า PAYSOLUTIOS ที่ท่านสมัครไว้ *

-	AccountID หรือ Merchant ID : 0000000 (จำเป็น) 

-	UserID หรือ Merchant ID : 00000000 (จำเป็น)

-	Payment Zone : None (ไม่จำเป็น)

-	Set Order Status : Default (ไม่จำเป็น)

-	URL : www.thaiepay.com

จากนั้นให้กด update 

 

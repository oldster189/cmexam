# Codemobile Challenge



## สร้างโปรเจค React
<b>1. ติดตั้ง Library</b>
  - axios
  - react-router-dom
  - yup
  - redux toolkit

<b>2. สร้าง Route ขึ้นมา 3 Page</b>
 - Login Page
 - Home Page
 - Detail Page

2.1 ค่าเริ่มต้น Rediect มาหน้า Login Page

<b>3. หน้า Login Page มี UI ตามนี้</b>

3.1 ช่องกรอกข้อมูล (Email, Password)

3.2 ปุ่มเข้าสู่ระบบ

3.3 เงื่อนไขตรวจสอบ
     - เมื่อกดปุ่มเข้าสู่ระบบ ตรวจสอบ Email = aa@bb.cc และ Password = 1234 ถ้าถูกต้อง Redirect ไปหน้า Home Page , ถ้าผิด Alert ข้อความ "Email or password incorrect"

<b>4. หน้า Home Page มีเงื่อนไขตามนี้</b>

4.1 ใช้ useEffect Fetch ข้อมูล JSON, URL GET: https://dummyjson.com/products

4.2 แปลงข้อมูล JSON ข้อ 4.1 เป็น Typescript Interface (ชื่อ interface Product) 

4.3 มีการใช้ useState เก็บข้อมูล products จาก Fetch 

4.4 แสดงข้อมูลที่ Fetch ได้ แสดง Column ตารางดังนี้
  - Thumnal 30*30
  - Title
  - Price
  - Stock
  - ปุ่ม Detail

 4.5 เมือกดปุ่ม Detail ให้ส่ง id product ผ่าน url params ไปหน้า Detail Page

<b>5. หน้า Detail Page</b>

5.1 Get id product จาก params และ  Fetch ข้อมูลสินค้า GET:https://dummyjson.com/products/:id   

5.2 แสดงข้อมูลสินค้า ตามสวยงาม
  - รูปสินค้า 150*150
  - Title
  - Price
  - Stock
  
<b>6. ปริ้น Console.log Life Cycle ของ Reactjs ในหน้า Home Page </b>

<b>7. เพิ่ม ช่องค้นหาข้อมูลสินค้า (ค้นหา ชื่อสินค้า) </b>

7.1 ค้นหาแบบ Debound Time(1 วินาที) และ contain string
 
<b>8. เพิ่มปุ่ม Dropdown 5 เมนู ในหน้า Home Page</b>
  - ทั้งหมด (แสดงสินค้าทั้งหมด)
  - ราคามากว่า 1000 (กรองสินค้าที่มีราคา 1000 ขึ้นไป) [ใช้ function Filter Javascript]
  - แสดงราคารวมต่อชิ้น (คำนวนราคาสินค้า ราคา*จำนวนสินค้า)  ** เพิ่ม Column ขึ้นมาอีก 1 Column สำหรับแสดง ราคารวมต่อชิ้น  [ใช้ function Map Javascript]
  - เรียงเรตติ้ง (เรียง rating สินค้า desc)  [ใช้  function Sort Javascript]
  - แสดงราคารวมทั้งหมด (คำนวนราคาสินค้าทั้งหมด ของ array สินค้า) ** เพิ่ม Label ไว้บนท้ายตารางสำหรับแสดง ราคารวมทั้งหมด  [ใช้ function reduce Javascript]

<b>9. เพิ่ม Validation Yup ในหน้า Login Page</b>
- ตรวจสอบ Format Email 
- ตรวจสอบความรหัสผ่าน ความยาว 4 ตัวขึ้นไป  

<b>10. Interceptor http axios</b>

10.1 console.log ข้อความ ตอน Request http

10.2 console.log ข้อความ ตอน Response http

<b>11. กำหนด Default route path เมื่อพิมพ์ url route path ผิด</b>

11.1 ถ้า ยังไม่ได้ Login ให้ Redirect มาหน้า Login Page

11.2 ถ้า Login แล้วให้ Redirect มาหน้า Home Page

<b>12. ติดตั้ง material ui theme https://mui.com/</b>

12.1 เปลี่ยน UI หน้า Login Page เป็น material ui ตามความสวยงาม

<b>13 ติดตั้ง Redux Toolkit </b>

13.1 สร้าง authStore

13.2 Init default value email = bb@cc.dd & password = 5678

13.3 เปลี่ยนการตรวจความถูกต้องหน้า Login Page ให้ดึงข้อมูลใน authStore มาตรวจสอบ Email & Password กับ Input text

<b>14. Create react hook</b>

14.1 สร้างชื่อ hook useMultiply Logic ภายใน รับค่าใดๆ เข้ามาแล้วคูณด้วย 10 และ Return ออกไป

14.2 Print ผลลัพพ์หน้า Home Page

<b>15. แสดงตัวอย่างการใช้ useMemo และ useCallback ในหน้า Home Page</b>
 
 

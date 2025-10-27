# 🏡 Nivilla - ระบบจัดการหมู่บ้านจัดสรร

แอปพลิเคชันสำหรับอำนวยความสะดวกในการสื่อสารและจัดการบริการต่างๆ ภายในหมู่บ้านจัดสรร พัฒนาด้วย **Flutter** และใช้ **Supabase** เป็น Backend as a Service (BaaS)

---

## ✨ คุณสมบัติหลัก (Key Features)

แอปพลิเคชันแบ่งการทำงานตามบทบาทผู้ใช้งาน 3 ส่วนหลัก โดยมีขอบเขตการทำงาน (Scope) ดังนี้:

<details>
  <summary><strong>👑 1. ผู้ดูแลระบบ (Admin) - (System Administrator)</strong></summary>
  
  <br>
  
  <ul>
    <li><strong>การจัดการระบบ (System & Auth)</strong>
      <ul>
        <li>เข้าสู่ระบบด้วยชื่อผู้ใช้และรหัสผ่าน</li>
        <li>จัดการรหัสผ่าน (เปลี่ยนรหัสผ่าน)</li>
      </ul>
    </li>
    <li><strong>การจัดการผู้ใช้ (User Management)</strong>
      <ul>
        <li>กำหนดสิทธิ์การเข้าใช้งาน (Permissions) ให้แก่ผู้ใช้งาน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลนิติบุคคล</li>
      </ul>
    </li>
    <li><strong>การจัดการข้อมูลหลัก (Master Data)</strong>
      <ul>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลจังหวัดของหมู่บ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลหมู่บ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลบ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลกฎระเบียบของหมู่บ้าน</li>
      </ul>
    </li>
    <li><strong>การจัดการการเงิน (Finance Setup)</strong>
      <ul>
        <li>จัดการ เพิ่ม/ลบ/แก้ไข ข้อมูลประเภทค่าใช้จ่ายส่วนกลาง</li>
      </ul>
    </li>
    <li><strong>การจัดการบุคลากร (Personnel Management)</strong>
      <ul>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลคณะกรรมการหมู่บ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลเจ้าหน้าที่รักษาความปลอดภัย (รปภ.)</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลช่างซ่อม</li>
      </ul>
    </li>
    <li><strong>ระบบรายงาน (Reporting)</strong>
      <ul>
        <li>สามารถจัดทำรายงาน ข้อมูลร้องเรียน</li>
        <li>สามารถจัดทำรายงาน ข้อมูลค่าใช้จ่ายส่วนกลาง</li>
        <li>สามารถจัดทำรายงาน ข้อมูลกองทุนหมู่บ้าน</li>
      </ul>
    </li>
  </ul>
</details>

<details>
  <summary><strong>👨‍💼 2. นิติบุคคล (Juristic Person / Management)</strong></summary>

  <br>

  <ul>
    <li><strong>การจัดการบัญชี</strong>
      <ul>
        <li>เข้าสู่ระบบด้วยชื่อผู้ใช้และรหัสผ่าน</li>
        <li>แก้ไขข้อมูลส่วนตัวของนิติบุคคล</li>
      </ul>
    </li>
    <li><strong>การจัดการข้อมูลหมู่บ้าน</strong>
      <ul>
        <li>ตรวจสอบ และ แก้ไข ข้อมูลหมู่บ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลบ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลกฎระเบียบของหมู่บ้าน</li>
      </ul>
    </li>
    <li><strong>การจัดการลูกบ้าน (Resident Management)</strong>
      <ul>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลร้องเรียน (รับเรื่อง)</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลสัตว์เลี้ยงของลูกบ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลยานพาหนะของลูกบ้าน</li>
      </ul>
    </li>
    <li><strong>การสื่อสาร (Communication)</strong>
      <ul>
        <li>ประกาศข้อมูลข่าวสาร (ผ่าน Supabase Realtime)</li>
        <li>แจ้งเตือนเกี่ยวกับปัญหาต่างๆ ภายในหมู่บ้าน</li>
      </ul>
    </li>
    <li><strong>การจัดการการเงิน (Finance)</strong>
      <ul>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลการเงินหมู่บ้าน</li>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลค่าใช้จ่ายส่วนกลาง (สร้างบิล, จัดการบิล)</li>
      </ul>
    </li>
    <li><strong>การจัดการบุคลากร (Personnel)</strong>
      <ul>
        <li>เพิ่ม/ลบ/แก้ไข ข้อมูลคณะกรรมการ, รปภ., และช่างซ่อม</li>
      </ul>
    </li>
    <li><strong>ระบบรายงาน (Reporting)</strong>
      <ul>
        <li>สามารถจัดทำรายงาน (ข้อมูลร้องเรียน, ค่าใช้จ่ายส่วนกลาง, กองทุนหมู่บ้าน)</li>
      </ul>
    </li>
  </ul>
</details>

<details>
  <summary><strong>👩‍👩‍👧‍👦 3. ลูกบ้าน (Resident)</strong></summary>
  
  <br>
  
  <ul>
    <li><strong>การจัดการบัญชี</strong>
      <ul>
        <li>เข้าสู่ระบบด้วยชื่อผู้ใช้และรหัสผ่าน</li>
      </ul>
    </li>
    <li><strong>ข้อมูลส่วนตัวและที่พักอาศัย</strong>
      <ul>
        <li>ตรวจสอบ ข้อมูลหมู่บ้านของตนเอง</li>
        <li>ตรวจสอบ ข้อมูลบ้านของตนเอง</li>
        <li>ตรวจสอบ ข้อมูลกฎหมายของหมู่บ้าน</li>
        <li>เพิ่ม และ แก้ไข ข้อมูลสัตว์เลี้ยง (ของตนเอง)</li>
        <li>เพิ่ม และ แก้ไข ข้อมูลยานพาหนะ (ของตนเอง)</li>
      </ul>
    </li>
    <li><strong>การแจ้งเรื่อง (Communication)</strong>
      <ul>
        <li>แจ้งปัญหาและร้องเรียน (เช่น แจ้งซ่อม)</li>
        <li>ติดตามสถานะการแก้ไขปัญหา</li>
        <li>ตรวจสอบการแจ้งเตือนข้อมูลข่าวสาร (รับ Notification)</li>
        <li>ตรวจสอบเกี่ยวกับปัญหาต่างๆ ในหมู่บ้าน</li>
      </ul>
    </li>
    <li><strong>การเงิน (Finance)</strong>
      <ul>
        <li>ตรวจสอบข้อมูลการเงินหมู่บ้าน</li>
        <li>ตรวจสอบ และชำระค่าใช้จ่ายส่วนกลาง</li>
      </ul>
    </li>
    <li><strong>ข้อมูลบุคลากร (Directory)</strong>
      <ul>
        <li>ตรวจสอบข้อมูลคณะกรรมการหมู่บ้าน</li>
        <li>ตรวจสอบข้อมูลเจ้าหน้าที่รักษาความปลอดภัย</li>
        <li>ตรวจสอบข้อมูลช่างซ่อม</li>
      </ul>
    </li>
    <li><strong>ระบบรายงาน (Reporting)</strong>
      <ul>
        <li>สามารถจัดทำรายงานสรุปข้อมูลร้องเรียน</li>
        <li>สามารถจัดทำรายงานสรุปข้อมูลค่าใช้จ่ายส่วนกลาง</li>
        <li>สามารถจัดทำรายงานสรุปกองทุนหมู่บ้าน</li>
      </ul>
    </li>
  </ul>
</details>

## 🎬 ตัวอย่างหน้าจอการทำงาน (Screenshots)

<details>
  <summary><strong>คลิกเพื่อดูรูปภาพหน้าจอการทำงาน (Flutter App)</strong></summary>
  
  <br>

| หน้าเข้าสู่ระบบ (Login) | หน้าผู้ดูแลระบบ (Admin) | หน้านิติ (lawer) | หน้าลูกบ้าน (house) |
| :-----------------------: | :--------------------: | :--------------------: | :--------------------: |

 <img src="https://github.com/asmhsever/nivillaWeb/blob/main/docs/login.png" width="220">

  <img src="https://github.com/asmhsever/nivillaWeb/blob/main/docs/admin.png"  width="220">

   <img src="https://github.com/asmhsever/nivillaWeb/blob/main/docs/lawer.png" width="220">

   <img src="https://github.com/asmhsever/nivillaWeb/blob/main/docs/house.png" width="220">

</details>


<img src="https://github.com/asmhsever/nivillaWeb/blob/main/docs/database.webp" width="150">
| ตารางข้อมูล (Database Tables) | การจัดการไฟล์ (Storage) |
| :---------------------------: | :---------------------: |
  <img src="https://github.com/asmhsever/nivillaWeb/blob/main/docs/data_diagram.png" width="1800">


## 🛠️ เทคโนโลยีที่ใช้ (Tech Stack)

- **Frontend (Mobile App):** **Flutter**
- **Programming Language:** **Dart**
- **Backend as a Service (BaaS):** **Supabase**
  - **Database:** PostgreSQL
  - **Authentication:** Supabase Auth
  - **Realtime:** Supabase Realtime Subscriptions
  - **File Storage:** Supabase Storage
  - **Serverless Functions:** Supabase Edge Functions (ถ้ามีการใช้งาน)
- **State Management:** (ระบุ เช่น Provider, Bloc, Riverpod, GetX)

---

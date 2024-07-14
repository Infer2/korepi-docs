---
title: ข้อผิดพลาดทั่วไป
icon: info
category:
  - Troubleshoot
tag:
  - Start
author: Schvis , ShikiYuri 
order: 2
---

## รายการข้อผิดพลาดทั่วไป

### ทำไม Korepi ของฉันถึงหายไป?

ตรวจสอบให้แน่ใจว่าคุณได้ปิดการใช้งานโปรแกรมป้องกันไวรัส, สร้างโฟลเดอร์ใหม่และเพิ่มลงในการยกเว้น(Exclusion list)

![](/assets/images/docs/202312/virus.png)

แตกไฟล์ korepi ภายในโฟลเดอร์ที่เพิ่มลงในการยกเว้น(Exclusion list) แล้วรันอีกครั้ง

---
### สถานะ: No active subscription(s) found, Invalid license key

คุณต้อง[รับคีย์ใหม่](../guide/getkey.md) จาก [`🔑 | micah-bot-verify`](https://discord.com/channels/1069057220802781265/1203687333107335198) หรือ [`verify-bak`](https://discord.com/channels/1069057220802781265/1238877451174678558), ถ้าคุณไม่สามารถรับคีย์ได้หรือคีย์ไม่สามารถใช้งานได้, คุณต้องรอจนกว่าคีย์จะหมดอายุ

`Sponsors สามารถใช้ F:รีเซ็ตคีย์แทนได้`

### [DLL injection]  Process crashed, exit code 0xc000005

เปิด `cmd` ในฐานะผู้ดูแลระบบและเขียนคำสั่งนี้:

`sfc /scannow`

หลังจากนั้นหากพบข้อผิดพลาด ให้รีสตาร์ทคอมพิวเตอร์และตรวจสอบ
หากหลังจากรีสตาร์ทแล้วมันไม่ช่วยหรือไม่พบข้อผิดพลาด ให้เขียนคำสั่งนี้:
`DISM.exe /Online /Cleanup-Image /RestoreHealth`

หลังจากตรวจสอบเสร็จแล้ว ให้รีสตาร์ทคอมพิวเตอร์และตรวจสอบ

หากไม่ได้ผล, ให้ลองสอบถามในเซิร์ฟเวอร์

---
### ImGUI: DirectX11 backend initialized successfully.

เกิดข้อผิดพลาดเนื่องจากการติดตั้งธีม, ให้ลบไฟล์ในโฟลเดอร์ "themes"

---
### The system did not detect MSVCP140.dll

อัปเดต [Microsoft Visual Studio C++](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022)

อัปเดต [DirectX](https://www.microsoft.com/en-us/download/details.aspx?id=35)

---
### File corrupted! This program has been manipulated and maybe it's infected.

![](/assets/images/docs/202312/virus2.png)

ในกรณีนี้ ให้ลองใช้ `Malware Bytes` หรือ `Dr.Web` เพื่อทำการสแกนแบบเต็ม, หากพบไวรัส, ให้ลบออก รีสตาร์ทแล้วลองอีกครั้ง, หากไม่ได้ผล, ให้ติดตั้ง Windows ใหม่เป็นวิธีที่ง่ายที่สุดในการแก้ปัญหานี้

---
### Timeout was reached

![](/assets/images/docs/202312/error1.png)

รีบูตเราเตอร์อินเทอร์เน็ตของคุณ

โปรแกรมป้องกันไวรัสอาจบล็อกการเชื่อมต่อ, ตรวจสอบให้แน่ใจว่ามันไม่ได้อยู่ในตัวจัดการงาน(Task Manager)

ลองใช้ VPN แล้วลองอีกครั้ง

ปิดแอปพลิเคชันทั้งหมดที่ส่งผลต่อไฟร์วอลล์ หากไม่มีอะไรใช้ได้, แสดงว่าคุณอาจประสบปัญหากับเครือข่าย

---
### DLL Injection failed

ถอนการติดตั้งโฟลเดอร์ colorpicker และดาวน์โหลด colorpicker อีกครั้ง

---
### Windows cannot access the specified device, path, or file

![](/assets/images/docs/202312/error2.png)

อย่างแรก[ไปที่นี้](https://support.microsoft.com/en-us/topic/-windows-cannot-access-the-specified-device-path-or-file-error-when-you-try-to-install-update-or-start-a-program-or-file-46361133-47ed-6967-c13e-e75d3cc29657) และทำตามขั้นตอนในโพสต์นั้น

แล้วก็หลังจากไปที่วิธีแก้ปัญหาในโพสต์แล้ว ให้ดาวน์โหลดโปรแกรมป้องกันไวรัสเช่น `Dr.Web` หรือ `Malware bytes` และทำการทำการสแกนแบบเต็ม!

หากไม่ได้ผล, เปิด `cmd` ในฐานะผู้ดูแลระบบและเขียนคำสั่งนี้:

`sfc /scannow`

หลังจากนั้นหากพบข้อผิดพลาด ให้รีสตาร์ทคอมพิวเตอร์และตรวจสอบ
หากหลังจากรีสตาร์ทแล้วมันไม่ช่วยหรือไม่พบข้อผิดพลาด ให้เขียนคำสั่งนี้:
`DISM.exe /Online /Cleanup-Image /RestoreHealth`

หลังจากตรวจสอบเสร็จแล้ว ให้รีสตาร์ทคอมพิวเตอร์และตรวจสอบ

หากไม่ได้ผล, ให้ลองสอบถามในเซิร์ฟเวอร์

---
### Signature checksum failed

![](/assets/images/docs/202312/checksum.png)

เซิร์ฟเวอร์ล่มหรือปิดตัวลง, รอให้เซิร์ฟเวอร์กลับมาออนไลน์อีกครั้ง

---
### Failed to create game process with Error 5

![](/assets/images/docs/202312/error3.png)

ลบ `cfg.ini`.

---
### SSL connect error

![](/assets/images/docs/202312/error4.png)

รีสตาร์ทพีซีของคุณ, รีสตาร์ทเราเตอร์ของคุณ

ลองใช้ VPN หากไม่ได้ผล

---
### Failed to detect game version

อัพเดตโปรแกรมของคุณ ทำตามขั้นตอน[ที่นี้](../start/download.md)

---
### File ok

1. บางครั้งคุณต้องเปิด Launcher สักสองสามครั้งก่อนจึงจะใช้งานได้

2. ลบ cfg.json ของคุณ, อาจมีข้อผิดพลาดเกิดขึ้นกับไฟล์

3. หากยังไม่สามารถแก้ปัญหาได้โปรดอ้างอิงถึง[ที่นี้](https://discord.com/channels/1069057220802781265/1213319789964038184/1242491428441952256).

---
### UserAssembly.dll isn't initialized, waiting for 2 sec.

หากโปรแกรมของคุณ crashes หลังจากบรรทัดนี้ ให้ลองทำตามขั้นตอนต่อไปนี้:

ปิดโปรแกรมป้องกันไวรัสทั้งหมดในพีซี

หากไม่ได้ผล, เปิด `cmd` ในฐานะผู้ดูแลระบบและเขียนคำสั่งนี้:

`sfc /scannow`

หลังจากนั้นหากพบข้อผิดพลาด ให้รีสตาร์ทคอมพิวเตอร์และตรวจสอบ
หากหลังจากรีสตาร์ทแล้วมันไม่ช่วยหรือไม่พบข้อผิดพลาด ให้เขียนคำสั่งนี้:
`DISM.exe /Online /Cleanup-Image /RestoreHealth`

หลังจากตรวจสอบแล้วให้รีสตาร์ทคอมพิวเตอร์แล้วลองเรียกใช้ colorpicker อีกครั้ง

หากเกิดข้อผิดพลาดซ้ำ, คุณต้องรีเซ็ต Windows เป็นค่าเริ่มต้นจากโรงงาน

### Current data does not exist or server error.

![](/assets/images/docs/202312/error.png)

หยุดการพักชั่วคราวและลองอีกครั้ง

### Cannot verify current timestamp.

![](/assets/images/docs/202402/timestamp.png)

กรณีที่ 1:
- คุณอาจได้รับข้อผิดพลาดนี้ขณะใช้ VPN โปรดปิดการใช้งานแล้วลองอีกครั้ง
- หากคุณไม่ได้ใช้ VPN และได้รับข้อผิดพลาดนี้ ให้ลองใช้ VPN

กรณีที่ 2:
- ตรวจสอบว่าเวลาพีซีของคุณถูกตั้งเวลาให้ซิงค์อัตโนมัติ

::: info หากคุณมาจากอิหร่าน คุณอาจจำเป็นต้องใช้ VPN แทน
:::
---
title: วิธีการยืนยันตัวตน
icon: key
category:
  - Guide
tag:
  - Start
  - License
author: Schvis , ShikiYuri , Micah
order: 1
---
## วิธีการยืนยันตัวตน

<div class="iframe-container"><iframe width="1280" height="720" src="https://www.youtube.com/embed/ST9akMsGJog" title="How to activate your key - Korepi" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>

::: danger หากคุณมีการสมัครสมาชิกที่ใช้งานอยู่, อย่า Bind การ์ดอื่นๆ มิฉะนั้นคุณจะสูญเสียการสมัครสมาชิกปัจจุบันของคุณ หากคุณ bind การ์ดอื่นๆแล้ว คุณจะไม่สามารถรับการ์ด sponsor ได้อีก
:::

### ขั้นตอนที่ 1:
- หาช่อง [`🔑 | micah-bot-verify`](https://discord.com/channels/1069057220802781265/1203687333107335198) หรือหากใช้ไม่ได้ ให้ใช้ [`verify-bak`](https://discord.com/channels/1069057220802781265/1238877451174678558)

  ![img.png](/assets/images/docs/202402/verify-1.png)
- หาข้อความที่ส่งโดย Micah-bot หรือ Micah-verify-bot-bak
### Step 2:
สำหรับเวอร์ชันฟรีทำตาม[ลิงค์นี้](free.md)

::: tip หากคุณมีการสมัครสมาชิกที่ใช้งานอยู่, กรุณากดที่ stack card แทน, เพื่อรวมเข้ากับการสมัครปัจจุบันของคุณ
:::

หากคุณซื้อคีย์จากตัวแทนจำหน่าย, คลิกที่ `bind card str` และวางคีย์ของคุณ

### ขั้นตอนที่ 3:
::: info หากคุณมี enc.json อยู่แล้วให้ลบออกก่อนที่จะเปิดโปรแกรม
:::
เปิดโปรแกรมเพื่อรับ`HWID`ของคุณ, หลังจากนั้นไปที่ [`🔑 | micah-bot-verify`](https://discord.com/channels/1069057220802781265/1203687333107335198) หรือ [`verify-bak`](https://discord.com/channels/1069057220802781265/1238877451174678558) อีกครั้ง และกดที่ `Get verification file` และวาง`HWID`ของคุณ
หลังจากคลิกส่ง คุณจะได้รับไฟล์จากบอท ให้ดาวน์โหลดและวางลงในโฟลเดอร์ Korepi ของคุณ ตรวจสอบให้แน่ใจว่าชื่อเป็น `enc.json`

คุณยังสามารถกด `View Subscription Information` เพื่อดูข้อมูลการสมัครสมาชิกของคุณ

## วิธีพักคีย์ชั่วคราว

กดที่ `Pause Card` และพิมพ์ `YES` เพื่อพักคีย์ชั่วคราว. คุณสามารถยกเลิกพักชั่วคราวได้ตลอดเวลาและการสมัครของคุณจะดำเนินต่อไป

::: info คุณสามารถหยุดคีย์ชั่วคราวได้ทุกๆ 30 วันเท่านั้น
:::

## วิธีการเปลี่ยน HWID (Device ID)

กดที่ `ID(Change HWID)`, และวาง `HWID` อันใหม่ที่คุณได้จากการเปิดโปรแกรม, หลังจากนั้นดาวน์โหลดไฟล์ใหม่และวางลงในโฟลเดอร์ Korepi ของคุณ

::: info คุณสามารถรีเซ็ต HWID ได้ทุกๆ 7 วันเท่านั้น
:::

## ปัญหาการยืนยัน MD5
ทุกครั้งที่คุณได้รับ `enc.json` อีกครั้ง, ไฟล์ `enc.json` อันเก่าจะเสียในทันที

หากอันใหม่ยังใช้ไม่ได้, กรุณารับไฟล์อีกครั้ง. หากยังไม่ได้อีกให้รอสักครู่แล้วลองอีกครั้ง

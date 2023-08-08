[<img src="https://raw.githubusercontent.com/jaideejung007/discuzth/v3.5/upload/static/image/common/logo.svg" width="250"/>](logo.svg)

# Discuz! Thai - ระบบเว็บบอร์ดดิสคัส! ภาษาไทย สำหรับสร้างเว็บไซต์ระดับมืออาชีพ

[![GitHub version](https://img.shields.io/github/v/release/jaideejung007/discuzth.svg)](https://github.com/jaideejung007/discuzth)
[![download latest release](https://img.shields.io/badge/Discuz!%20X3.5-Download-success.svg)](https://github.com/jaideejung007/discuzth/releases/latest)
![GitHub all releases](https://img.shields.io/github/downloads/jaideejung007/discuzth/total?label=Total%20Downloads)
[![SE](https://img.shields.io/discord/1065259119239495772?color=purple&label=Discord%20Discuz%21%20Thai%20Community&logoColor=purple)](https://discord.gg/faSzs3geux "Discord ของ Discuz! Thai Community อย่างเป็นทางการ")
[![Discuz! Thai Support](https://img.shields.io/youtube/channel/subscribers/UC3bP2rWm_4rqKBj88smHDgg?label=Discuz%21%20Thai%20Support&style=social)](https://www.youtube.com/@discuzthaisupport)


# คำแนะนำ #
Discuz! เป็นแพลตฟอร์มสร้างเว็บไซต์ที่มุ่งเน้นไปที่การสร้างชุมชนออนไลน์ ช่วยให้เว็บไซต์สามารถให้บริการแบบครบ จบ ในที่เดียว

# ไฮไลท์สำคัญ X3.5 #
* สนับสนุน PHP8
* สนับสนุน MYSQL8
* สนับสนุน IPV6, สนับสนุนไลบรารี IP หลายตัว, สนับสนุนการเข้าถึง IP ในโหมด CDN ต่าง ๆ และสนับสนุนโหมดการเข้าถึงข้อมูลที่เพิ่มขึ้นจากโหมดปกติ
* สนับสนุน UTF8MB4 (จงใช้อิโมจิกันโดยพลัน และสนับสนุนชุดอักขระเพิ่มเติม)
* สนับสนุน InnoDB (ฐานข้อมูลคลาวด์มีการแนะนำให้ใช้งานอย่างแพร่หลาย)
* สนับสนุน การสลับใช้งานฟังก์ชันโมดูลเต็มรูปแบบ (รวมไปถึงเว็บบอร์ด ต่อจากนี้ไป Discuz! X จะไม่ใช่แค่เว็บบอร์ดอย่างเดียว แต่เป็นระบบสร้างเว็บไซต์เต็มรูปแบบ)
* สนับสนุน HTTPS ให้มีประสิทธิภาพกว่าเดิม
* เพิ่ม ระบบชำระเงินใหม่ (ใช้ได้แค่ประเทศจีน ไม่มีไทย) มีชำระเงินด้วย WeChat, Alipay และ QQ Wallet ในตัว สนับสนุนการเชื่อมต่อการชำระเงินแพลตฟอร์มอื่น ๆ
* ปรับปรุง ฐานข้อมูลจังหวัด อำเภอ ตำบล (จาก ThepExcel ปรับปรุงปี 2565) พร้อมทั้งรายชื่อ 199 ประเทศและอีก 52 ดินแดน (จากสำนักงานราชบัณฑิตยสภา 29 มิถุนายน 2565)
* ปรับปรุง ตัวแปลงไอพีเป็นชื่อประเทศ (GeoIP2) โดยใช้ไลบรารีจาก MaxMind's GeoLite2 City ซึ่งสามารถระบุความละเอียดตำแหน่งที่ตั้งของไอพีในระดับ เขต/อำเภอ จังหวัด และประเทศ
* ปรับปรุง BBcode Spoiler โฉมใหม่
* ปรับปรุง ระบบปกป้องขั้นพื้นฐานในตัว และสนับสนุนการเชื่อมต่อ SMS ของบุคคลที่สามโดยผ่านอินเทอร์เฟซ
* ปรับปรุง โหมดรุ่นมือถือแบบใหม่ ไฉไลกว่าเดิม
* ปรับปรุง ระบบหลังบ้าน (AdminCP) โฉมใหม่
* ปรับปรุง UX/UI ต่าง ๆ ในเว็บเพื่อให้เข้ากับสภาพแวดล้อมของประเทศไทยทั้งหมด (เช่น การสลับตำแหน่งคำภาษาจีน ให้เป็นของภาษาไทยในส่วนต่าง ๆ ของเว็บ เป็นต้น)
* ยกเลิก การใช้ Flash ถาวร และขอต้อนรับ HTML5 เต็มรูปแบบ

## การติดตั้งใหม่
* ดาวน์โหลดไฟล์ล่าสุดที่นี่: https://github.com/jaideejung007/discuzth/releases/latest
* อัปโหลดไฟล์และโฟลเดอร์ทั้งหมดใน upload ไปยังเซิร์ฟเวอร์ของคุณ โดยใช้โปรแกรม FTP ตามสะดวกของคุณ เช่น โปรแกรม FileZilla เป็นต้น (ไม่จำเป็นต้องอัปโหลดโฟลเดอร์ readme และไฟล์ utility.html)
* เปิดเบราว์เซอร์เพื่อทำการติดตั้ง Discuz! X3.5 โดยไปที่ yourdomain.com/install เพื่อเริ่มต้นขั้นตอนการติดตั้ง แล้วทำตามหน้าจอที่ปรากฏ

## การอัปเกรดจาก X3.4
* ตรวจสอบการเชื่อมต่อ UCenter กับ Discuz! ของคุณว่าอยู่ในสถานะ “เชื่อมต่อได้” หรือไม่ โดยตรวจสอบที่เว็บ yourdomain.com/uc_server แล้วเข้าสู่ระบบให้เรียบร้อย ไปที่เมนู “การเชื่อมต่อ” --> แล้วดูหัวข้อ “การเชื่อมต่อ” ถ้าขึ้นสถานะสีเขียวว่า “เชื่อมต่อได้” ไม่ต้องทำอะไร ดำเนินการอัปเกรดข้อต่อไปได้เลย แต่ถ้าขึ้นสถานะสีแดงว่า “เชื่อมต่อไม่ได้” ให้คลิก “แก้ไข” แล้วตั้งค่าดังนี้ 1) “URL ของโปรแกรม:” ให้เป็น URLเว็บบอร์ด ของคุณ เช่น https://yourdomain.com โดยไม่ต้องมี / ปิดท้าย, 2) “คีย์สำหรับเชื่อมต่อ:” ค่าดังกล่าวจะต้องตรงกับตัวแปร “UC_KEY” ในไฟล์ “โฟลเดอร์รากเว็บบอร์ด/config/config_ucenter.php”
* ดาวน์โหลดไฟล์อัปเกรดได้ที่: https://discuzthai.com/thread-41059-1-1.html หรือที่โฟลเดอร์ [utility](https://github.com/jaideejung007/discuzth/tree/v3.5/utility) ของ GitHub Discuz! Thai
* สำรองฐานข้อมูลและไฟล์โปรแกรม Discuz! และ UCenter เก่าของคุณ รวมไปถึงไฟล์ที่เกี่ยวข้องทั้งหมดในเซิร์ฟเวอร์ให้เรียบร้อยก่อนดำเนินการ
* ไปที่ “โฟลเดอร์รากเว็บบอร์ด/uc_server” แล้วสร้างโฟลเดอร์ “old” ขึ้นมาใหม่ (ตัวอย่างเส้นทางโฟลเดอร์: “โฟลเดอร์รากเว็บบอร์ด/uc_server/old”) แล้วทำการย้ายโฟลเดอร์ทั้งหมดที่อยู่ใน “โฟลเดอร์รากเว็บบอร์ด/uc_server/*.*” (ยกเว้นโฟลเดอร์ต่อไปนี้ห้ามย้าย: “data”) ไปที่ “โฟลเดอร์รากเว็บบอร์ด/uc_server/old” (หากมีไฟล์การกำหนดค่าเว็บไซต์ต่าง ๆ นอกเหนือจากไฟล์ของ UCenter รวมไปถึงไฟล์ .htaccess หรือ .user.ini ไม่ต้องย้ายไฟล์ดังกล่าว)
* อัปโหลดโปรแกรม UCenter 1.7.0 (อยู่ในไฟล์ ZIP ของ Discuz! X3.5 ตำแหน่งโฟลเดอร์ คือ upload/uc_server หากคุณใช้โปรแกรม FTP ในการอัปโหลด ใช้โหมดการอัปโหลดเป็นไบนารี) ไปที่ “โฟลเดอร์รากเว็บบอร์ด/uc_server” หากคุณได้รับแจ้งให้เขียนทับโฟลเดอร์ขณะอัปโหลด กรุณาเลือก "ใช่"
* อัปโหลดไฟล์ update_ucenter_adult.php ไปที่ “โฟลเดอร์รากเว็บบอร์ด/uc_server/install” และลบไฟล์ “โฟลเดอร์รากเว็บบอร์ด/uc_server/data/upgrade.lock” ออก
* เปิดเบราว์เซอร์ แล้วไปลิงก์นี้: “URLเว็บบอร์ด/uc_server/install/update_ucenter_adult.php” และปฏิบัติตามคำแนะนำตามหน้าจอที่ปรากฎเพื่อดำเนินการอัปเกรด เวลาในการอัปเกรดจะแตกต่างกันไปตามขนาดของข้อมูลและประสิทธิภาพของเซิร์ฟเวอร์
* กลับมาที่ โฟลเดอร์รากเว็บบอร์ด ของคุณ จากนั้น ให้สร้างโฟลเดอร์ old ขึ้นมาใหม่ (ตัวอย่างเส้นทางโฟลเดอร์: “โฟลเดอร์รากเว็บบอร์ด/old”) แล้วทำการย้ายโฟลเดอร์ทั้งหมด (ยกเว้นโฟลเดอร์ดังต่อไปนี้ห้ามย้าย: config, data และ uc_server) ไปที่ “โฟลเดอร์รากเว็บบอร์ด/old” หากมีไฟล์การกำหนดค่าเว็บไซต์ต่าง ๆ รวมถึงไฟล์ .htaccess หรือ .user.ini ไม่ต้องย้ายไฟล์ดังกล่าว
* อัปโหลดโปรแกรม Discuz! X3.5 (ไฟล์โปรแกรมทั้งหมดจะอยู่ในโฟลเดอร์ upload ของไฟล์ ZIP Discuz! X3.5 กรุณาใช้โหมดไบนารีหากคุณใช้โปรแกรม FTP ในการอัปโหลด) ไปที่ “โฟลเดอร์รากเว็บบอร์ด” บนเซิร์ฟเวอร์ของคุณ (ยกเว้นโฟลเดอร์ดังต่อไปนี้ห้ามอัปโหลด: uc_server) และโปรแกรม FTP จะแจ้งให้เขียนทับโฟลเดอร์ กรุณาเลือก "ใช่"
* ย้ายโฟลเดอร์ปลั๊กอินทั้งหมดที่อยู่ใน “โฟลเดอร์รากเว็บบอร์ด/old/source/plugin/*.*” (ยกเว้นโฟลเดอร์ต่อไปนี้ห้ามย้าย: cloudcaptcha, cloudsearch, cloudstat, cloudunion, manyou, mobile, mobileoem, myapp, myrepeats, pcmgr_url_safeguard, qqconnect, qqgroup, security, soso_smilies, wechat, xf_storage) กลับไปที่ “โฟลเดอร์รากเว็บบอร์ด/source/plugin” และย้ายโฟลเดอร์เทมเพลททั้งหมดที่อยู่ใน “โฟลเดอร์รากเว็บบอร์ด/old/template/*.*” (ยกเว้นโฟลเดอร์ต่อไปนี้ห้ามย้าย: “default”) กลับไปที่ “โฟลเดอร์รากเว็บบอร์ด/template”
* อัปโหลดไฟล์ update_adult.php ไปที่ “โฟลเดอร์รากเว็บบอร์ด/install” และลบไฟล์ “โฟลเดอร์รากเว็บบอร์ด/data/update.lock” ออก
* เปิดเบราว์เซอร์ แล้วไปลิงก์นี้: “URLเว็บบอร์ด/install/update_adult.php” และปฏิบัติตามคำแนะนำตามหน้าจอที่ปรากฎเพื่อดำเนินการอัปเกรด เวลาในการอัปเกรดจะแตกต่างกันไปตามขนาดของข้อมูลและประสิทธิภาพของเซิร์ฟเวอร์
> หากต้องการอัปเกรดจากเวอร์ชันอื่น กรุณาอัปเกรดเป็น X3.4 ก่อน: https://discuzthai.com/thread-40670-1-1.html

## การอัปเกรดจาก X3.4 (วิดีโอช่วยสอน)
* https://www.youtube.com/watch?v=QmIj_Ot3f_k

## ทีมพัฒนา (ต้นฉบับภาษาจีน) 
* forked from [Discuz](https://gitee.com/Discuz) / [DiscuzX](https://gitee.com/Discuz/DiscuzX) 

## ทีมพัฒนา (ภาษาไทย) 
* [jaideejung007](https://github.com/jaideejung007/)

## เว็บไซต์ที่เกี่ยวข้อง 
* เว็บไซต์ดิสคัส! ภาษาไทยอย่างเป็นทางการ: https://discuzthai.com
* เว็บไซต์ดิสคัส! ภาษาไทยสำหรับทดสอบ: https://beta.discuzthai.com
* เว็บไซต์ดิสคัส! ภาษาจีน : https://www.discuz.vip/
* เว็บไซต์ดิสคัส! ภาษาจีน (2): https://www.dismall.com/

---
version: prototype1
revision_id: 1173829
locale: th
slug: MDN/Contribute/Howto/Do_a_technical_review
tags: 
title: How to do a technical review
summary: 
keywords: 
needs_technical_review: True
needs_editorial_review: True
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<h2 id="IncludeSubnav_(_en-US_เอกสาร_MDN)"><font><font><font><font>{{IncludeSubnav ( "/ en-US / เอกสาร / MDN")}}</font></font></font></font></h2>

<p class="summary"><strong><font><font><font><font>การตรวจสอบทางเทคนิค</font></font></font></font></strong><font><font><font><font>ประกอบด้วยการตรวจสอบความถูกต้องทางด้านเทคนิคและความสมบูรณ์ของบทความและแก้ไขได้ถ้าจำเป็น</font></font></font><font><font><font>ถ้าเป็นนักเขียนของบทความต้องการให้คนอื่นตรวจสอบเนื้อหาทางเทคนิคของบทความนักเขียนเห็บ "การตรวจสอบทางเทคนิคช่อง" ขณะที่การแก้ไข</font></font></font><font><font><font>การติดต่อมักจะเขียนเป็นวิศวกรที่เฉพาะเจาะจงในการดำเนินการตรวจสอบทางเทคนิค แต่ทุกคนที่มีความเชี่ยวชาญทางเทคนิคในหัวข้อสามารถทำอย่างใดอย่างหนึ่ง</font></font></font></font></p>

<p><span class="seoSummary"><font><font><font><font>บทความนี้อธิบายถึงวิธีการที่จะดำเนินการตรวจสอบทางเทคนิคจึงช่วยให้เพื่อให้มั่นใจว่าเนื้อหา MDN อย่างถูกต้อง</font></font></font></font></span></p>

<dl>
 <dt><font><font><font><font>งานของคุณคืออะไร?</font></font></font></font></dt>
 <dd><font><font><font><font>การตรวจสอบและแก้ไขบทความเพื่อความถูกต้องและครบถ้วนทางเทคนิค</font></font></font></font></dd>
 <dt><font><font><font><font>ที่ไม่ได้จะต้องมีการทำ?</font></font></font></font></dt>
 <dd><font><font><font><font>ในบทความที่เฉพาะเจาะจงที่ถูกทำเครื่องหมายเป็นต้องมี</font></font></font><font><font><font>การตรวจสอบทางเทคนิค</font></font></font></font></dd>
 <dt><font><font><font><font>สิ่งใดที่คุณจำเป็นต้องรู้ที่จะทำงานได้หรือไม่</font></font></font></font></dt>
 <dd>
 <ul>
  <li><font><font><font><font>ความรู้จากผู้เชี่ยวชาญในหัวข้อของบทความที่คุณกำลังตรวจสอบ</font></font></font><font><font><font>หากอ่านบทความไม่ได้สอนอะไรใหม่อย่างมีนัยสำคัญจะพิจารณาตัวเองผู้เชี่ยวชาญ</font></font></font></font></li>
  <li><font><font><font><font>วิธีการแก้ไขบทความวิกิพีเดียใน MDN</font></font></font></font></li>
 </ul>
 </dd>
 <dt><font><font><font><font>มีขั้นตอนอะไรจะทำหรือไม่</font></font></font></font></dt>
 <dd>
 <ol>
  <li><font><font><font><font>เลือกบทความเพื่อทบทวน:</font></font></font></font>
   <ol>
    <li><font><font><font><font>ไปที่รายการของหน้าเว็บที่ต้องการ</font></font></font><font><font><font>แสดงความคิดเห็นทางเทคนิค</font></font></font><font><font><font>นี้แสดงหน้าเว็บทั้งหมดที่มีการตรวจสอบทางเทคนิคได้รับการร้องขอ</font></font></font></font></li>
    <li><font><font><font><font>เลือกหน้ามีหัวข้อที่คุณมีความคุ้นเคยกับ</font></font></font></font></li>
    <li><font><font><font><font>คลิกที่ลิงค์บทความเพื่อโหลดหน้าเว็บ</font></font></font></font></li>
   </ol>
  </li>
  <li><a id="core-steps" name="core-steps"></a><font><font><font><font>อ่านบทความที่ให้ความสนใจใกล้เคียงกับรายละเอียดทางเทคนิค: บทความถูกต้องหรือไม่</font></font></font><font><font><font>มีอะไรหายไป? </font></font></font><font><font><font>อย่าลังเลที่จะเปลี่ยนไปยังเพจที่แตกต่างกันถ้าคนแรกที่คุณเลือกไม่เหมาะกับคุณ</font></font></font></font></li>
  <li><font><font><font><font>"ตรวจสอบอย่างรวดเร็ว" </font></font></font><font><font><font>ๆ</font></font></font></font><br />
   <img alt="ภาพหน้าจอของกล่องแถบด้านข้างของรายการความคิดเห็นที่ได้รับการร้องขอและช่วยให้ธงจะมีการเปลี่ยนแปลง" src="https://mdn.mozillademos.org/files/13016/SidebarTechReviewRequested.png" /></li>
  <li><font><font><font><font>ยกเลิกการเลือก</font></font></font></font><strong><font><font><font><font>เทคนิค</font></font></font></font></strong><font><font><font><font>ช่องทำเครื่องหมายและคลิก</font></font></font><font><font><font>บันทึก</font></font></font></font></li>
  <li><font><font><font><font>หากคุณพบข้อผิดพลาดที่ต้องได้รับการแก้ไขแล้วคุณจะดีใจที่รู้ว่าคุณยังสามารถเปลี่ยนสถานะคำขอตรวจสอบจากภายในบรรณาธิการ</font></font></font><font><font><font>นี่คือขั้นตอนการทำงาน:</font></font></font></font>
   <ol>
    <li><font><font><font><font>แก้ไขหน้าให้คลิก</font></font></font></font><strong><font><font><font><font>แก้ไข</font></font></font></font></strong><font><font><font><font>ปุ่มที่อยู่ด้านบนของหน้า; </font></font></font><font><font><font>นี้ทำให้คุณเข้าสู่</font></font></font><font><font><font>การแก้ไข MDN</font></font></font></font></li>
    <li><font><font><font><font>แก้ไขข้อมูลทางด้านเทคนิคใด ๆ ที่ไม่ถูกต้องและ / หรือเพิ่มข้อมูลใด ๆ ที่สำคัญที่ขาดหายไป</font></font></font></font></li>
    <li><font><font><font><font>ป้อน</font></font></font></font><strong><font><font><font><font>Revision </font></font></font></font></strong><font><font><font><font>ๆ ที่อธิบายถึงสิ่งที่คุณทำ เช่น </font></font></font></font><font><font><font><font>ๆ </font></font></font><font><font><font>qualfied ในการตรวจสอบ</font></font></font></font></li>
    <li><font><font><font><font>ยกเลิกการเลือก</font></font></font><strong><font><font><font>เทคนิค</font></font></font></strong><font><font><font>กล่องใต้</font></font></font><strong><font><font><font>ทบทวนจำเป็น?</font></font></font></strong><font><font><font>เพียงด้านล่างพื้นที่แสดงความคิดเห็นการทบทวนของหน้า</font></font></font></font><em> </em></li>
    <li><font><font><font><font>ที่คลิก</font></font></font></font><strong><font><font><font><font>เผยแพร่</font></font></font></font></strong><font><font><font><font>ปุ่ม</font></font></font></font></li>
   </ol>
  </li>
 </ol>

 <p><font><font><font><font>ขอแสดงความยินดี! </font></font></font><font><font><font>คุณเสร็จสิ้นการตรวจสอบทางเทคนิคครั้งแรกของคุณ! </font></font></font><font><font><font>ขอขอบคุณสำหรับความช่วยเหลือของคุณ!</font></font></font></font></p>
 </dd>
</dl>


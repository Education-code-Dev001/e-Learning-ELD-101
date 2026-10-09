# ELD-101: การออกแบบและพัฒนา e-Learning (Courseware)

บทเรียนคอมพิวเตอร์ผ่านเว็บ (e-Learning Courseware) แบบ Single Page Application (SPA) สำหรับนักศึกษาครูคอมพิวเตอร์ ชั้นปีที่ 3 เพื่อเสริมสร้างสมรรถนะการออกแบบสื่อดิจิทัลเพื่อการเรียนรู้ตามหลักวิชาการ ใช้เวลาในการศึกษาประมาณ 90 นาที

---

## 🎯 วัตถุประสงค์การเรียนรู้ (Course Objectives)
1. **กระบวนการพัฒนาระบบการสอน:** อธิบายขั้นตอนของ ADDIE Model และระบุผลงานหลัก (Deliverables) ในแต่ละขั้นตอนได้อย่างถูกต้อง
2. **การออกแบบการสอน:** เขียนวัตถุประสงค์เชิงพฤติกรรมที่วัดได้ตาม Bloom's Taxonomy และจัดลำดับกิจกรรมการเรียนรู้ตาม 9 เหตุการณ์การสอนของ Gagné ได้
3. **การออกแบบสื่อและการเข้าถึง:** วินิจฉัยปัญหาการออกแบบสื่อบทเรียนตามหลัก Mayer's Multimedia Principles และเกณฑ์การเข้าถึงเว็บ (Web Accessibility: WCAG 2.1 AA)
4. **การวัดและประเมินผล:** เลือกใช้เครื่องมือและหลักฐานในการวัดประเมินผลสัมฤทธิ์ทางการเรียนรู้ได้อย่างสอดคล้องตามเกณฑ์ Kirkpatrick และการวิเคราะห์พัฒนาการด้วย Normalized Gain

---

## 📚 โครงสร้างเนื้อหาบทเรียน (4 บทเรียน)

### บทที่ 1: ภาพรวม e-Learning และ ADDIE Model
* ความหมายของ e-Learning และความแตกต่างระหว่าง Synchronous และ Asynchronous
* รายละเอียดกระบวนการ ADDIE 5 ขั้นตอน (Analysis, Design, Development, Implementation, Evaluation) คำถามชี้นำ และผลงานที่ได้รับ (Deliverables)
* ธรรมชาติการพัฒนาระบบการสอนแบบวนซ้ำ (Iterative Process)
* **กิจกรรม:** ปฏิสัมพันธ์คลิกเรียงลำดับขั้นตอน ADDIE

### บทที่ 2: การออกแบบการสอน (Instructional Design)
* การกำหนดวัตถุประสงค์เชิงพฤติกรรมที่วัดได้ (Measurable Objectives)
* ระดับกระบวนการทางปัญญาตาม Bloom's Taxonomy ฉบับปรับปรุง (Anderson & Krathwohl, 2001) พร้อมคลังคำกริยาที่วัดผลได้
* 9 เหตุการณ์การสอนของ Gagné (Gagné's Nine Events of Instruction)
* **กิจกรรม:** จับคู่สถานการณ์จำลองในห้องเรียนกับเหตุการณ์การสอนของ Gagné

### บทที่ 3: การออกแบบสื่อและกิจกรรม (Media Design & Interaction)
* ทฤษฎีการเรียนรู้มัลติมีเดียของ Mayer เพื่อลดภาระทางปัญญา (Coherence, Signaling, Segmenting, Spatial Contiguity, Redundancy)
* มิติปฏิสัมพันธ์ 3 ประเภทของ Moore (Learner-Content, Learner-Instructor, Learner-Learner)
* เกณฑ์การเข้าถึงเนื้อหาเว็บ (WCAG 2.1 AA): อัตราส่วนความต่างสี (Contrast Ratio $\ge 4.5:1$), ข้อความกำกับภาพ (alt text) และคำบรรยายคลิป (Captions)
* **กิจกรรม:** วินิจฉัยข้อผิดพลาดในการออกแบบสไลด์และสื่อ 4 สถานการณ์

### บทที่ 4: การวัดผลและข้อมูลการเรียนรู้ (Assessment & Analytics)
* การประเมินระหว่างเรียน (Formative) และการประเมินสรุปผล (Summative)
* การวัดประสิทธิผลการเรียนรู้ด้วยอัตราการเพิ่มของพัฒนาการสัมพัทธ์ (Normalized Gain) ตามแนวคิดของ Hake (1998):
  $$g = \frac{\text{Post} - \text{Pre}}{\text{Total} - \text{Pre}}$$
* โมเดลการประเมินโครงการฝึกอบรม 4 ระดับของ Kirkpatrick (Reaction, Learning, Behavior, Results)
* มาตรฐานข้อมูลการเรียนรู้ดิจิทัล (SCORM และ xAPI เบื้องต้น: Actor-Verb-Object) และจริยธรรมข้อมูล
* **กิจกรรม:** จับคู่หลักฐานการประเมินผลกับระดับ Kirkpatrick Model

---

## 🛠️ ข้อกำหนดและคุณสมบัติทางเทคนิค
* **Single File Architecture:** โค้ดทั้งหมด (HTML, CSS, JavaScript) รวมอยู่ภายในไฟล์ `index.html` เพียงไฟล์เดียว ไม่พึ่งพา Framework หรือไลบรารีภายนอก
* **Responsive Design:** รองรับการใช้งานสมบูรณ์แบบบนสมาร์ตโฟน (ความกว้างหน้าจอ 390 px ขึ้นไป) เมนูสารบัญซ้ายจะปรับเป็นเมนูพับได้อัตโนมัติบนอุปกรณ์พกพา
* **Theme Support:** รองรับ Light Mode และ Dark Mode ผ่าน CSS Custom Properties โดยตรวจสอบการตั้งค่าจากระบบ (`prefers-color-scheme`) และมีปุ่มสลับธีมบนหน้าจอ
* **Data Privacy & Storage:** บันทึกความก้าวหน้า คะแนนสอบ และชื่อเล่นลงใน `localStorage` ของเบราว์เซอร์ โดยครอบ `try/catch` ไม่มีการส่งข้อมูลส่วนบุคคลออกนอกอุปกรณ์
* **Accessibility:** รองรับการควบคุมผ่านแป้นพิมพ์อย่างสมบูรณ์ (Tab Index, Visible Focus Rings) และเคารพการตั้งค่าลดการเคลื่อนไหว (`prefers-reduced-motion`)

---

## 🚀 วิธีการเปิดใช้งาน

1. **เปิดใช้งานแบบ Local (ออฟไลน์):**
   * บันทึกไฟล์โค้ดเป็นชื่อ `index.html`
   * ดับเบิลคลิกเปิดไฟล์ด้วยเว็บเบราว์เซอร์มาตรฐาน (เช่น Google Chrome, Microsoft Edge, Firefox, Safari)
2. **เปิดใช้งานผ่าน GitHub Pages (ออนไลน์):**
   * อัปโหลดไฟล์ `index.html` ขึ้นบน Repository
   * ไปที่ **Settings** > **Pages**
   * เลือก Branch เป็น `main` โฟลเดอร์ `/(root)` แล้วกด **Save**
   * เข้าใช้งานผ่าน URL: `https://<username>.github.io/<repository-name>/`

[Read English Version](README.md)

# ชนมภูมิ ธรรมสุวรรณ (CTSuwan)
**นักพัฒนา Operations Research อิสระ และสถาปนิกด้านอัลกอริทึม**

ยินดีต้อนรับสู่ศูนย์กลางของ **GSL Engine** — สถาปัตยกรรมการเพิ่มประสิทธิภาพเชิงกำหนด (Deterministic Optimization Architecture) สำหรับปัญหา Vehicle Routing Problem (VRP) ที่มีความซับซ้อนสูง

จุดมุ่งหมายของโปรเจกต์นี้คือการสำรวจแนวทางการจัดเส้นทางที่เน้น:
- deterministic execution
- low-latency routing
- edge/mobile computation
- และความเสถียรของผลลัพธ์ภายใต้ข้อจำกัดของฮาร์ดแวร์

🔥 **Mobile Execution Proof:**  
สถาปัตยกรรม GSL ทั้งหมดถูกพัฒนา ทดสอบ และประมวลผลบน Mobile Architecture (Snapdragon processor ผ่าน Python/Pydroid 3) โดยใช้แนวทาง Zero-Tuning และ deterministic feasibility-oriented execution เพื่อศึกษาพฤติกรรมของระบบตั้งแต่ benchmark มาตรฐานไปจนถึงโจทย์ระดับ large-scale และ real-world logistics

---

# 🚀 GSL Engine Portfolio (Routing Architecture)

เลือกโมดูลด้านล่างเพื่อดู benchmark, execution logs และเอกสารด้านเทคนิคของแต่ละระบบ

## 📦 1. Capacitated VRP (CVRP) Module

- **ขอบเขต:** ปัญหา VRP ภายใต้ข้อจำกัดด้านความจุรถ
- **รายละเอียด:** ครอบคลุม benchmark หลายตระกูล ตั้งแต่ Set A ถึง XML รวมถึงการทดสอบ Hyper-Scale บน Uchoa Set XL

🔗 ดู Repository CVRP หลัก:  
https://github.com/CT1-deMo-goG/gsl-routing-engine

🔗 ดู Repository Hyper-Scale CVRP (Set XL):  
https://github.com/CT1-deMo-goG/GSL-CVRP-SETXL

---

## ⏱️ 2. VRPTW (Vehicle Routing Problem with Time Windows)

- **ขอบเขต:** ระบบจัดเส้นทางภายใต้ข้อจำกัดด้านเวลา
- **รายละเอียด:** ประเมินบน Solomon และ Homberger benchmark families ภายใต้แนวทาง deterministic execution และ zero-tuning strategy

🔗 ดู VRPTW Repository:  
https://github.com/CT1-deMo-goG/GSL-VRPTW-Portfolio

---

## 🏢 3. Multi-Depot VRP (MDVRP)

- **ขอบเขต:** ระบบจัดเส้นทางแบบหลายศูนย์กระจายสินค้า
- **รายละเอียด:** ทดสอบบนโจทย์ large-scale รวมถึงกรณี 10,000 nodes / 100 depots บน mobile hardware

🔗 ดู MDVRP Repository:  
https://github.com/CT1-deMo-goG/gsl_mdvrp_engine

---

## 🌍 4. Real-World MDVRPTW Module

- **ขอบเขต:** Multi-Depot, Time Windows, Asymmetric Distance และ Dual-Capacity Constraints
- **รายละเอียด:** ประเมินบนชุดข้อมูลโลจิสติกส์จริงภายใต้ deterministic routing execution

🔗 ดู MDVRPTW Repository:  
https://github.com/CT1-deMo-goG/gsl-mdvrptw-engine

---

# 📘 Research & Architecture Notes

## Deterministic Single-Pass Routing Architecture

Repository นี้ยังรวม exploratory whitepaper และ technical notes เกี่ยวกับ:

- deterministic routing execution
- low-latency dispatch systems
- edge-constrained VRP computation
- variance-free execution behavior
- mobile-scale logistics optimization

📄 ดูเอกสาร:  
`Docs/deterministic_single_pass_whitepaper.md`

---

# 💼 Commercial Application & Consulting

GSL Architecture ถูกออกแบบเพื่อสำรวจการประยุกต์ใช้งานในด้าน:

- real-time dispatch systems
- logistics APIs
- edge-compute routing
- industrial optimization environments

---

# GSL-Solver Platform

**Deterministic Routing Platform**

เข้าถึงแพลตฟอร์มได้ที่:  
https://gsl-solver.com

---

# Professional Contact

**Independent Researcher:** ชนมภูมิ ธรรมสุวรรณ (CTSuwan)

📧 ctsuwan@proton.me

---

# Services & Collaboration

เปิดรับความร่วมมือในด้าน:

- Logistics-as-a-Service (LaaS)
- ระบบจัดเส้นทางสำหรับองค์กร
- การออกแบบอัลกอริทึมเฉพาะทาง
- Large-scale optimization testing
- งานวิจัยด้าน deterministic routing และ edge-scale optimization

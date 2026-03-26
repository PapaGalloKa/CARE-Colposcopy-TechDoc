<p align="center">
  <img src="assets_v2/logo.png" alt="C.A.R.E Logo" width="200"/>
</p>

<h1 align="center">C.A.R.E Colposcopy</h1>
<h3 align="center">Computer-Aided Recognition & Evaluation</h3>
<h4 align="center">Technical Document — AI-Powered Medical Imaging Application for Colposcopy</h4>

<p align="center">
  <img src="https://img.shields.io/badge/Framework-Qt%206.10-41CD52?style=for-the-badge&logo=qt" alt="Qt"/>
  <img src="https://img.shields.io/badge/Language-C++17-00599C?style=for-the-badge&logo=cplusplus" alt="C++"/>
  <img src="https://img.shields.io/badge/AI-TensorFlow%20Lite-FF6F00?style=for-the-badge&logo=tensorflow" alt="TFLite"/>
  <img src="https://img.shields.io/badge/Platforms-Android%20%7C%20Windows%20%7C%20iOS-999?style=for-the-badge" alt="Platforms"/>
</p>

---

## 1. Introduction

**Cervical cancer** remains one of the deadliest cancers for women in developing countries, with over 340,000 deaths per year worldwide. Colposcopy is the gold standard examination for early detection of precancerous lesions, but its accessibility remains limited by the lack of suitable digital tools and the high cost of existing solutions.

**C.A.R.E Colposcopy** (Computer-Aided Recognition & Evaluation) is a cross-platform medical application that digitizes and enhances the complete colposcopic workflow: from image capture with a medical green filter, to annotation, AI-powered analysis, and automatic generation of clinical reports.

The application is designed for deployment on clinical smartphones and tablets as well as hospital workstations, and will be integrated into the **future dedicated C.A.R.E hardware prototype** — a standalone digital colposcopy device.

---

## 2. Video Demonstration

The video below presents a complete demonstration of the application, showing the entire user journey:

**[Watch the video demonstration](assets_v2/demo.mp4)**

> *Duration: 4 min 30 | Complete walkthrough: login, patient management, image capture with green filter, medical annotation, PDF report generation, statistics, settings.*

---

## 3. Screen Overview

### 3.1 Login Page
Secure authentication with multi-role management (Super Admin, Admin, Doctor, Assistant). Professional medical interface with C.A.R.E branding.

`[INSERT: assets_v2/screenshots/01_login.png]`

![Login Page](assets_v2/screenshots/01_login.png)

---

### 3.2 Dashboard
Personalized home screen displaying the connected practitioner's name (Dr. Aissatou Diallo — Gynecology), with quick access to main functions: New Exam, Patients, Reports, Statistics. Recent examinations list at the bottom.

`[INSERT: assets_v2/screenshots/02_home.png]`

![Dashboard](assets_v2/screenshots/02_home.png)

---

### 3.3 Patient Selection
Complete patient registry with real-time search by name or medical record number (MRN). Displays avatars, dates of birth, and identifiers. Quick-add button for new patients.

`[INSERT: assets_v2/screenshots/03_patient_list.png]`

![Patient Selection](assets_v2/screenshots/03_patient_list.png)

---

### 3.4 Camera Interface — Normal View
Real-time colposcopic image capture with side controls: LED (lighting), Green Filter, Zoom, Exposure. Status bar at the bottom showing mode, captured image count, and patient MRN.

`[INSERT: assets_v2/screenshots/04_camera.png]`

![Camera Normal View](assets_v2/screenshots/04_camera.png)

---

### 3.5 Camera Interface — Medical Green Filter
The **medical green filter** (OpenGL ES 3.0 GPU shader) amplifies the green channel to better visualize cervical vascular patterns — the digital equivalent of the optical green filter used in traditional colposcopy. Real-time adjustable filter intensity slider (Green Level).

`[INSERT: assets_v2/screenshots/05_camera_green_filter.png]`

![Camera Green Filter](assets_v2/screenshots/05_camera_green_filter.png)

---

### 3.6 Image Capture
After taking a photo, a thumbnail appears at the bottom right confirming the capture. The image counter is updated in real-time in the status bar.

`[INSERT: assets_v2/screenshots/06_camera_capture.png]`

![Image Capture](assets_v2/screenshots/06_camera_capture.png)

---

### 3.7 Exam Gallery
View of images captured during an examination. Multiple selection for group annotation or report generation. Action buttons: Annotate, Report, Delete.

`[INSERT: assets_v2/screenshots/07_exam_gallery.png]`

![Exam Gallery](assets_v2/screenshots/07_exam_gallery.png)

---

### 3.8 Medical Annotation — Measurements
Annotation toolset with millimeter measurements: circles to delineate areas of interest, measurement lines, and markers. Integrated **AI Analysis** button.

`[INSERT: assets_v2/screenshots/08_annotation.png]`

![Annotation Measurements](assets_v2/screenshots/08_annotation.png)

---

### 3.9 Medical Annotation — Complete Tools
Full toolbar: Circle, Line, Freehand Drawing, Rectangle, Measurements, Text. Color palette (red, blue, green, yellow, black) and configurable stroke width. Shown here: text annotation "lesion 1" with bounding rectangle and measurements.

`[INSERT: assets_v2/screenshots/09_annotation_tools.png]`

![Annotation Tools](assets_v2/screenshots/09_annotation_tools.png)

---

### 3.10 Report Generation
Structured colposcopic report form: patient information (name, DOB, MRN, phone, email), clinical indication, cervical appearance, transformation zone (type 1/2/3), acetic acid and iodine findings, vascular patterns.

`[INSERT: assets_v2/screenshots/10_report_generation.png]`

![Report Generation](assets_v2/screenshots/10_report_generation.png)

---

### 3.11 Generated PDF Report
Preview of the automatically generated PDF report in C.A.R.E format. Contains patient information, clinical findings, and annotated images. Opens directly in the browser.

`[INSERT: assets_v2/screenshots/11_report_pdf.png]`

![PDF Report](assets_v2/screenshots/11_report_pdf.png)

---

### 3.12 Patient Detail Record
Complete patient record with Info / Gallery / Reports tabs. Contact information, medical information (allergies, medications, history), gynecological information. "Start Examination" button to directly launch a colposcopy.

`[INSERT: assets_v2/screenshots/12_patient_detail.png]`

![Patient Detail](assets_v2/screenshots/12_patient_detail.png)

---

### 3.13 Patient Gallery
Gallery tab of the patient record showing all images captured during various examinations, with thumbnails and visible annotations.

`[INSERT: assets_v2/screenshots/13_patient_gallery.png]`

![Patient Gallery](assets_v2/screenshots/13_patient_gallery.png)

---

### 3.14 Patient Reports
Access to generated reports for a patient with options: Open, Share, Delete.

`[INSERT: assets_v2/screenshots/14_patient_report.png]`

![Patient Reports](assets_v2/screenshots/14_patient_report.png)

---

### 3.15 Patient Record Editing
Complete editing form for gynecological information: last menstrual period, pregnancy status, contraceptive method, previous Pap smear, previous colposcopy, family history of cancer.

`[INSERT: assets_v2/screenshots/15_edit_patient.png]`

![Edit Patient](assets_v2/screenshots/15_edit_patient.png)

---

### 3.16 Statistics
Analytical dashboards: counters (patients, exams, abnormality rate), examinations by month (bar chart), lesion distribution (donut chart), AI confidence trends, age distribution.

`[INSERT: assets_v2/screenshots/16_statistics.png]`

![Statistics](assets_v2/screenshots/16_statistics.png)

---

### 3.17 Settings
Application configuration: language (French/English), image quality (Low/Medium/High/Maximum), automatic AI analysis, storage location, automatic and manual database backup.

`[INSERT: assets_v2/screenshots/17_settings.png]`

![Settings](assets_v2/screenshots/17_settings.png)

---

### 3.18 User Profile
Practitioner profile management: email, department, specialization, medical license number. Secure password change.

`[INSERT: assets_v2/screenshots/18_profile.png]`

![User Profile](assets_v2/screenshots/18_profile.png)

---

### 3.19 Navigation Menu
Side drawer with connected practitioner identification (Dr. Aissatou Diallo — DOCTOR). Quick access: Home, Patients, Reports, Statistics, Profile, Settings, Logout.

`[INSERT: assets_v2/screenshots/19_navigation_drawer.png]`

![Navigation Menu](assets_v2/screenshots/19_navigation_drawer.png)

---

## 4. Technology Stack

| Component | Technology | Rationale |
|-----------|-----------|-----------|
| **Framework** | Qt 6.10 (C++17 + QML/JavaScript) | Native cross-platform, medical-grade performance, certification-ready |
| **Database** | SQLite with WAL mode | Lightweight, embedded, offline-capable, performant |
| **Artificial Intelligence** | TensorFlow Lite | Cervical lesion detection, on-device embedded inference |
| **Medical Rendering** | OpenGL ES 3.0 (GPU shader) | Real-time medical green filter, GPU image processing |
| **Architecture** | MVC (Model-View-Controller) | Clean separation of services / models / views |
| **Primary Language** | C++17 | Native performance, deterministic memory management |
| **User Interface** | QML + JavaScript | Fluid declarative UI, material animations |
| **Reports** | Native PDF generation | Automatic structured clinical reports |
| **Security** | SHA-256, account locking | Medical data protection |

---

## 5. Why Qt C++ for Healthcare Software

The choice of **Qt C++** as the primary framework is deliberate for a medical application. It addresses specific requirements of the healthcare industry:

- **IEC 62304 Compliance**: The international standard for medical device software lifecycle is facilitated by deterministic C++ — no garbage collector, no unpredictable memory behavior, complete execution traceability.

- **CE / FDA Certification**: Qt is already used in the medical industry (Siemens MRI devices, Philips patient monitors, GE Healthcare imaging systems). The Qt ecosystem provides traceability and testing tools validated for certification.

- **Single Codebase, All Platforms**: The same source code compiles for Android, Windows, iOS, and Linux. This **significantly reduces certification costs** as only one codebase needs to be validated, tested, and documented.

- **Real-Time Performance**: Medical image processing and GPU rendering (green filter, annotations) require native performance that only C++ can guarantee on resource-constrained mobile devices.

- **No Cloud Dependency**: The application works entirely offline, an essential criterion for medical environments where connectivity is not guaranteed and data sovereignty is mandatory.

---

## 6. Target Platforms

| Platform | Status | Intended Use |
|----------|--------|-------------|
| **Android** (ARM64, ARMv7) | In progress | Clinical smartphones and tablets |
| **Windows** (x64) | Functional | Hospital/clinic workstations |
| **iOS** (ARM64) | Planned | iPad for mobile consultations |
| **C.A.R.E Hardware Prototype** | Planned | **The software will be embedded in the future dedicated C.A.R.E medical device** — a standalone digital colposcope integrating high-definition camera, medical lighting, and embedded AI processing |

---

## 7. Key Features

- **Multi-role authentication**: Super Admin, Admin, Doctor, Assistant — each role with specific permissions
- **Complete patient record management**: Creation, modification, search, medical history, gynecological information
- **Colposcopic image capture** with real-time medical green filter (GPU shader)
- **Advanced medical annotation**: Circle, line, freehand drawing, rectangle, measurements in mm, text
- **AI cervical lesion analysis**: Automatic classification, confidence score (TensorFlow Lite)
- **Automatic PDF report generation**: Structured clinical format with annotated images
- **CSV export** of clinical data for external analysis
- **Statistics and dashboards**: Lesion distribution, AI trends, patient demographics
- **Automatic database backup**
- **Bilingual interface**: French / English
- **Complete offline mode**: No internet dependency — guaranteed autonomous operation

---

## 8. Security and Compliance

| Measure | Description |
|---------|-------------|
| **Password hashing** | SHA-256, never stored in plain text |
| **Account locking** | Automatic after failed attempts |
| **Local storage** | Data only on the device — complete sovereignty |
| **GDPR architecture** | Compliant by design — no cloud data transfer |
| **Audit trail** | Action traceability (planned) |
| **Database encryption** | SQLCipher (planned) |
| **Granular permissions** | Role-based access control |

---

## 9. Roadmap

| Period | Milestone |
|--------|-----------|
| **Q2 2026** | Android deployment finalization + clinical testing begins |
| **Q3 2026** | CE marking certification (Class IIa — medical device software) |
| **Q4 2026** | **C.A.R.E Hardware Prototype v1** — standalone digital colposcope |
| **2027** | iOS deployment + HL7/FHIR integration for hospital interoperability |

---

## 10. Contact

For any technical questions or demonstration requests, please contact the C.A.R.E team.

---

*This document is confidential and intended only for authorized parties in the context of the C.A.R.E Colposcopy project technical evaluation.*

# 👋 Hi there! I'm Temmy

![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Courier&size=24&duration=4000&color=2687FF&lines=Backend+Developer;Django+Enthusiast;Open+to+Collaborations)

I'm a Backend Developer with a B.Sc. in Software Engineering, specializing in building efficient, scalable applications. I enjoy working with Django. Currently, I'm expanding my portfolio with advanced API development and integration.

---

## Tech Stack

- **Languages**: Python, SQL
- **Frameworks**: Django
- **Databases**: PostgreSQL, MySQL
- **Tools**: Docker, Celery, GitHub Actions, Git, RESTful APIs
- **Interests**: Machine learning and Model Training

---

## Featured Projects

### A Clinic Management system
![Clinic Management system Demo](path-to-gif-demo.gif) 
An enterprise-grade healthcare administration backend built with Django 5.2 and Django REST Framework. Engineered to handle real-time appointment booking, strict schedule concurrency validation, dynamic administrative reporting, and dual-layered asynchronous notifications via Celery and Redis.

Key Highlights

- **Automated Cron Scheduling:**  
  Leverages `celery-beat` to execute multi-tier, time-sensitive workflows, automatically calculating and dispatching patient reminders exactly **24 hours** and **4 hours** before scheduled appointments.

- **Concurrency & Integrity Controls:**  
  Implements rigorous backend validation mechanisms to prevent double bookings and eliminate scheduling overlaps.

- **Interactive OpenAPI Specifications:**  
  Provides comprehensive API documentation powered by `drf-spectacular`, delivering clean, testable Swagger UI and ReDoc interfaces out of the box.

---

 Core Capabilities

- Schedule Lifecycle Management
Tracks appointment progression securely through a structured multi-state workflow:

`pending → confirmed → cancelled | to-be-rescheduled`

- Omnichannel Notification Matrix
    Integrates:
    - **Gmail SMTP** for patient and administrator email notifications
    - **Twilio API** for direct administrative SMS alerts triggered by critical booking events

- Advanced Admin Workspace
    Extends the Django Admin interface with:
    - Bulk status update operations
    - Custom CSS-based color coding for rapid clinic-side triage and workflow visibility

- Dynamic PDF Reporting
Generates real-time daily operational summaries as downloadable PDF reports directly from the active PostgreSQL database layer.

**[View Project](https://github.com/temmy669/Clinic_backend)**

---

### Wallet Service API
![Wallet Service API Project](path-to-gif-demo.gif)
A robust, production-ready fintech API backend that enables automated digital wallet management, secure peer-to-peer transfers, and third-party service integration. Built with Django REST Framework, integrated with Paystack, and secured via hybrid JWT/API Key authentication.

Key Highlights
- Production-Grade Architecture: Designed with atomic database transactions to eliminate race conditions and financial discrepancies.

- Hybrid Authentication: Supports both user-facing sessions (Google OAuth + JWT) and service-to-service automation (Granular API Keys).

- Bulletproof Webhooks: Idempotent payment processing utilizing HMAC signature verification to prevent double-crediting.

 Core Capabilities
- OAuth & Identity: Google Sign-In integration that seamlessly provisioned user accounts and digital wallets upon first authentication.

- Automated Payments: End-to-end deposit flows via Paystack, managed safely through custom webhook listeners.

- P2P Transfers: Secure wallet-to-wallet fund routing using unique ledger identifiers.

- B2B Developer Features: A custom API Key generation engine allowing up to 5 active keys per user with granular scopes (read, deposit, transfer) and strict expiration/rollover intervals.

**[View Project](https://github.com/temmy669/Wallet-Service)**

---

### Image Processing Upload Service
![Upload-Service](path-to-gif-demo.gif)
A highly scalable, containerized microservice engineered to handle heavy media workloads asynchronously. Built with Django REST Framework, Celery, and Redis, it offloads resource-intensive image manipulation tasks to background workers, serving processed assets via a custom MinIO (S3-compatible) object storage layer.

Key Highlights
- Non-Blocking Architecture:
    Decouples file ingestion from CPU-bound manipulation, ensuring instant API responses (O(1) wait times for users) while workers handle image computation asynchronously in the background.
- Granular Object Pipeline:
    Automatically generates three optimized variations from a single upload:
      i. Resized images (1024×1024)
      ii. Compressed JPEGs (60% quality)
      iii. Thumbnail previews (300×300)
- Cloud-Native Deployment:
    Designed for independent scaling with a decoupled multi-container architecture (Web vs. Worker), optimized for both local Docker environments and cloud platforms such as Railway.
  
 Core Capabilities
- Asynchronous Execution
  Offloads heavy image-processing workloads to isolated Celery workers, using Redis as a high-throughput message broker for efficient task distribution.
  
- Deterministic Object Mapping
  Enforces a structured and predictable cloud bucket directory layout, organizing assets cleanly across:
    /oiginals/
    /resized/
    /compressed/
    /thumbnails/

- State Machine Tracking
  Maintains strict internal lifecycle transitions:

- persistent states:
  pending → processing → completed | failed
  This provides clients with deterministic status tracking through lightweight polling endpoints.
  
- Secure Access Routing
  Abstracts underlying bucket privacy configurations by securely serving assets through time-bound, pre-signed URLs generated via Boto3..

**[View Project](https://github.com/temmy669/Inventory_Management_System)**

---

## 📫 Connect with Me!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adebose-favour)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/tem_mylade)




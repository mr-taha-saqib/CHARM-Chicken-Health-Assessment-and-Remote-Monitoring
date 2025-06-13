# CHARM: Chicken Health Assessment and Remote Monitoring

**CHARM** (Chicken Health Assessment and Remote Monitoring) is an AI-powered web platform for the real-time detection and diagnosis of poultry diseases using deep learning and computer vision. CHARM helps poultry farmers, veterinarians, and researchers upload images or videos of chickens to get instant diagnostic results, health alerts, and actionable treatment suggestions. The system is designed for practical deployment in poultry farms and aims to improve productivity, food safety, and animal health through rapid, automated diagnosis.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [System Architecture](#system-architecture)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)

---

## Project Overview

Poultry farmers often struggle with early detection of infectious diseases, leading to rapid outbreaks and significant economic losses. **CHARM** leverages advanced AI—combining YOLOv8 object detection, BoT-SORT tracking, and ResNet50 classification—to analyze images and video footage, detect symptoms, classify diseases (including infectious coryza, fowl cholera, and fowl pox), and provide immediate results. The platform offers a user-friendly Django web interface, with role-based access for farmers and administrators.

---

## Features

- **Real-Time Disease Detection**: Analyze images and videos instantly for multiple poultry diseases.
- **AI-Powered Diagnosis**: YOLOv8 for detection/tracking, ResNet for disease classification.
- **Supports Multiple Diseases**: Including infectious coryza, fowl cholera, fowl pox, and general poultry diseases.
- **Live Health Monitoring**: Multi-camera and live video stream support.
- **Smart Alerts & Recommendations**: Notifies users if serious disease is detected, offers treatment suggestions.
- **User-Friendly Web Interface**: Secure login, simple upload process, diagnostic history.
- **Admin Dashboard**: User management, system status, and analytics.
- **Modular & Scalable**: Designed for future extension and integration.

---

## Tech Stack

- **Backend**: Python, Django, Django REST Framework
- **Frontend**: HTML, CSS, JavaScript (Django Templates)
- **AI/ML**: YOLOv8 (Detection), BoT-SORT (Tracking), ResNet50 (Classification)
- **Database**: PostgreSQL / SQLite
- **Dev Tools**: OpenCV, NumPy, Pandas

---

## System Architecture

- **Detection Subsystem**: YOLOv8 detects and localizes chickens in frames.
- **Tracking Subsystem**: BoT-SORT tracks individual chickens for continuous health monitoring.
- **Classification Subsystem**: ResNet50 classifies cropped images as healthy or diseased.
- **Web Platform**: Django app for uploads, results, user management.
- **Alerting**: Real-time notification for detected diseases.
- **Data Storage**: Keeps diagnostic records, images, user info, and farm health logs.

---

## Getting Started

### Prerequisites

- Python 3.8+
- Django 4.x
- (Optional for GPU acceleration) CUDA-compatible GPU
- PostgreSQL or SQLite

### Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/your-username/CHARM.git
    cd CHARM
    ```

2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3. **Run migrations**
    ```bash
    python manage.py migrate
    ```

4. **Create a superuser (for admin access)**
    ```bash
    python manage.py createsuperuser
    ```

5. **Start the development server**
    ```bash
    python manage.py runserver
    ```

6. **Configure and run AI models**  
   (See `/ml` or `/models` directory for setup instructions)

---

## Usage

- Access the web app at: `http://localhost:8000`
- Register or login as a user.
- Upload images/videos of poultry for analysis.
- View diagnostic results, health alerts, and treatment recommendations.
- Admins can manage users and monitor system health via the dashboard.

---

## Screenshots

![WhatsApp Image 2025-06-12 at 18 26 38_b12b45b8](https://github.com/user-attachments/assets/ae73ed84-c1eb-4fa8-b424-53cb15a66cf3)
![WhatsApp Image 2025-06-12 at 18 26 40_0a7b7aee](https://github.com/user-attachments/assets/675e4839-9e13-4b95-8886-36cad2a7792b)
![WhatsApp Image 2025-06-12 at 18 26 39_4486d1e0](https://github.com/user-attachments/assets/da25b7f8-5d63-4def-bb21-c1c8a8c1427e)
![WhatsApp Image 2025-06-12 at 18 26 39_97bac32b](https://github.com/user-attachments/assets/d7e43558-7915-4efe-ae0b-05c877e128d5)
![WhatsApp Image 2025-06-12 at 18 26 38_ed9d9ecf](https://github.com/user-attachments/assets/74463555-58a6-4be0-b75b-0f7664103da1)
![chicken-4595843_1920_classified](https://github.com/user-attachments/assets/e3b47656-8521-4a12-9bde-46e4fbcb5dac)
![img5_classified](https://github.com/user-attachments/assets/4bbd1d84-20ec-4780-87cd-dc30f8d565be)
![chicken-4168127_1280_classified](https://github.com/user-attachments/assets/8727395c-b65c-45cf-8b8b-49ade82a236f)


---

## Contributing

We welcome contributions!  
To contribute:

1. Fork this repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request with a clear description.

For major changes, please open an issue first to discuss what you would like to change.

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more details.

---

## Authors

- Muhammad Taha Saqib
- Tayyab Akhtar
- Mateen Abid

**Supervisor:** Ms. Sana Fatima  
*National University of Computer and Emerging Sciences, Lahore*

---

## Acknowledgments

- All open-source contributors and community resources referenced in the making of this project.
- Special thanks to our supervisor for guidance and support.

---

## Contact

For queries or collaboration, please open an issue or contact the authors directly.


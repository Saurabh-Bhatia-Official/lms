<<<<<<< HEAD
<<<<<<< HEAD
# Management-System1
=======
# LMS (26_09_3_LMS) 🎓

A full-stack institutional **Learning Management System (LMS)** configured with a **Spring Boot 3 (Java 21)** backend and a multi-platform **Flutter 3 (Dart)** frontend supporting Web, Windows Desktop, Android, iOS, macOS, and Linux.

---

## 🏗️ Architecture & Technology Stack

| Layer | Technology | Description |
| :--- | :--- | :--- |
| **Frontend** | Flutter 3 + Dart | Multiplatform responsive frontend (Web, Windows, Android, iOS, macOS, Linux) with Provider state management |
| **Backend** | Spring Boot 3.4.3 (Java 21) | REST microservice with JPA / Hibernate, JWT authentication, and PostgreSQL |
| **Config** | Environment Variables | Declarative configuration via `.env` without hardcoded ports or credentials |

---

## 📁 Project Structure

```text
26_09_3_LMS/
├── .env.example                     # Root environment variable template
├── .gitignore                       # Git ignore preventing secrets and build outputs
├── README.md                        # Project documentation
├── run.md                           # Quick execution and build commands reference
├── backend/                         # Spring Boot 3 Backend
│   ├── .env.example                 # Backend environment variable template
│   ├── .gitignore                   # Backend specific git ignore
│   ├── pom.xml                      # Maven configuration with Spring Boot Starter Web & JPA
│   └── src/
│       ├── main/
│       │   ├── java/com/management/ # Spring Boot controllers, entities, repositories & services
│       │   └── resources/
│       │       └── application.properties # Application property bindings
│       └── test/                    # Backend unit & integration tests
└── frontend/                        # Flutter Multiplatform Frontend
    ├── pubspec.yaml                 # Flutter packages & assets
    ├── lib/
    │   ├── constants/               # API endpoints & design system tokens
    │   ├── models/                  # User, Student, Faculty, Exam, Course models
    │   ├── providers/               # Provider state management & navigation router
    │   ├── services/                # HTTP client & persistent StorageService
    │   ├── widgets/                 # ResponsiveBuilder, AppNavbar, StatCard, etc.
    │   ├── screens/                 # Public, Auth, Student Portal, Teacher Portal & Admin Portal
    │   └── main.dart                # App entrypoint & dynamic router
    ├── test/
    │   └── widget_test.dart         # Widget smoke & navigation test
    ├── web/                         # Web platform host & manifest
    ├── android/                     # Android native project
    ├── ios/                         # iOS native project
    ├── windows/                     # Windows native desktop runner
    ├── macos/                       # macOS desktop runner
    └── linux/                       # Linux desktop runner
```

---

## 🚀 Execution Commands

See [`run.md`](file:///c:/Users/ssbha/Desktop/Github/26_09_3_LMS/run.md) for quick copy-paste commands.

### Backend (`/backend`)
```bash
# Run application
mvn clean spring-boot:run

# Build JAR
mvn clean package -DskipTests
```

### Frontend (`/frontend`)
```bash
# Fetch dependencies
flutter pub get

# Run on Chrome
flutter run -d chrome

# Run on Windows Desktop
flutter run -d windows

# Run tests
flutter test

# Run analyzer
flutter analyze

# Build Web release bundle
flutter build web --release
```
>>>>>>> e748a45af7cbc731caed8f47f3a3834494c42e76
=======
# 26_09_3_LMS-sub_master
>>>>>>> efa9eea7512aeffa30b5db3f09872df50c851289

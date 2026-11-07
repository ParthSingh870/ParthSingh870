# Hi, I'm Parth Madhav Singh 👋
I am a 3rd year Computer Science and Engineering undergraduate at IIIT Bhagalpur, actively seeking a Backend Development Internship.
I enjoy designing scalable RESTful APIs, implementing robust authentication & authorization workflows, and writing clean, maintainable backend code.

## 🛠️ Tech Stack
- **Languages & Runtimes:** Node.js, TypeScript, JavaScript (ES6+), C++
- **Frameworks & Real-time:** Express.js, Socket.io
- **Databases & ORM/ODM:** PostgreSQL, Prisma ORM, MongoDB, Mongoose
- **Caching & Queues:** Redis, BullMQ
- **Authentication & Security:** JWT (Access & Refresh Rotation, SHA-256 Hashes), bcrypt, RBAC
- **Testing & Tools:** Vitest, Docker, Docker Compose, Postman, Git, GitHub Actions CI

## 📂 Featured Backend Projects

### 🍽️ [Hostel Mess Management & Real-Time Ordering System](https://github.com/ParthSingh870/Hostel-mess)
Containerized Node.js/TypeScript backend for hostel mess pre-orders:
- **Atomic Stock Control:** Enforced inventory concurrency using Prisma transactions and a PostgreSQL `CHECK` constraint (race condition caught by concurrency test and fixed, preventing overselling).
- **Redis Cache-Aside:** High-speed menu caching with automated cache invalidation upon staff updates and fail-open fallback during outages.
- **BullMQ Kitchen Queue:** Asynchronous kitchen job processing with a dedicated worker (concurrency 3, retries with backoff); in an isolated local test, an ungracefully killed worker's job was auto-resumed by a replacement worker (~73 s).
- **Socket.io Real-Time Rooms:** Authenticated private user rooms for live order status updates (tokens accepted strictly via `handshake.auth`).
- **Hardened Authentication:** Role-based access control (Student/Staff) with refresh tokens stored securely as SHA-256 hex hashes in PostgreSQL.
- **Production Testing & CI:** 28 Vitest automated integration tests across 6 suites, 24-step manual integration test suite, and GitHub Actions CI.

---

### 📝 [Todo List REST API](https://github.com/ParthSingh870/Todo-list-api)
A secure task management REST API featuring dual-token JWT authentication (access & refresh rotation), role-based authorization (USER / ADMIN), Zod schema validation, and soft-delete capabilities.

---

### 🔗 [URL Shortener API](https://github.com/ParthSingh870/ParthSingh870/blob/main/link)
A URL shortening backend service that generates unique short IDs, handles fast HTTP redirections, and tracks click analytics per shortened link.

---

## 📬 Connect With Me
- **LinkedIn:** [linkedin.com/in/parth-singh-008288330](https://www.linkedin.com/in/parth-singh-008288330)
- **GitHub:** [@ParthSingh870](https://github.com/ParthSingh870)
- **Email:** [parthsingh870jlp@gmail.com](mailto:parthsingh870jlp@gmail.com)

Feel free to explore my repositories or reach out for collaboration and internship opportunities!

# Streamora
Streamora is a modern real-time communication platform that enables screen sharing, live streaming, and interactive collaboration across Web, Android, and iOS devices.


# 🚀 Streamora Backend

Backend service for **Streamora**, a real-time screen sharing and live streaming platform supporting Web, Android, and iOS.

## ✨ Features

- 🔐 JWT Authentication
- 👤 User Management
- 🗄 PostgreSQL Database
- ⚡ Prisma ORM
- 🌐 WebSocket Signaling
- 🎥 WebRTC Support
- 📺 Live Streaming
- 🖥 Screen Sharing
- 📱 Cross-platform Support (Web, Android, iOS)
- 🔄 Refresh Tokens
- 🏠 Room Management
- 🎙 Audio & Video Streaming

---

# 🏗 Tech Stack

| Technology | Version |
|------------|---------|
| NestJS | 11.x |
| TypeScript | 5.x |
| PostgreSQL | 18.x |
| Prisma | 6.x |
| JWT | Latest |
| WebSocket | Latest |
| WebRTC | Latest |
| LiveKit | Latest |

---

# 📂 Project Structure

```text
src/
├── auth/
├── users/
├── prisma/
├── rooms/
├── signaling/
├── streaming/
├── common/
└── main.ts

prisma/
├── migrations/
└── schema.prisma
```

---

# ⚙️ Environment Variables

Create a `.env` file in the project root.

```env
DATABASE_URL="postgresql://postgres:YOUR_PASSWORD@localhost:5432/streamora"

JWT_SECRET="your_super_secret_key"

JWT_EXPIRES_IN="7d"
```

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/streamora-backend.git

cd streamora-backend
```

Install dependencies

```bash
npm install
```

---

# 🗄 Database Setup

Generate Prisma Client

```bash
npx prisma generate
```

Run migrations

```bash
npx prisma migrate dev --name init
```

Open Prisma Studio

```bash
npx prisma studio
```

---

# ▶ Running the Application

Development

```bash
npm run start:dev
```

Production

```bash
npm run build

npm run start:prod
```

---

# 🔐 Authentication Endpoints

### Register

```http
POST /auth/register
```

Request

```json
{
  "email": "admin@streamora.com",
  "password": "123456"
}
```

---

### Login

```http
POST /auth/login
```

Request

```json
{
  "email": "admin@streamora.com",
  "password": "123456"
}
```

Response

```json
{
  "accessToken": "jwt_token"
}
```

---

# 🛣 Development Roadmap

### Day 1
- [x] PostgreSQL
- [x] Prisma
- [x] User Model

### Day 2
- [ ] JWT Authentication
- [ ] Register API
- [ ] Login API

### Day 3
- [ ] WebSocket Gateway
- [ ] Room Management

### Day 4
- [ ] WebRTC Signaling
- [ ] Screen Sharing

### Day 5
- [ ] LiveKit Integration

### Day 6
- [ ] Web Dashboard

### Day 7
- [ ] React Native Mobile App

---

# 📄 License

MIT License

---

## Streamora

**Stream smarter. Share instantly.**
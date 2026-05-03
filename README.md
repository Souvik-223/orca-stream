# 🎥 Orca Stream

> A fullstack open source streaming web app like Twitch — with all user controls and chat features, end to end.

`Next.js` &nbsp;|&nbsp; `React` &nbsp;|&nbsp; `TypeScript` &nbsp;|&nbsp; `LiveKit` &nbsp;|&nbsp; `Socket.io` &nbsp;|&nbsp; `MySQL`

---

## 🧠 About

**Orca Stream** is a production-grade, fullstack streaming platform inspired by Twitch. It supports real-time video streaming via RTMP/WHIP protocols, live chat with sockets, a follower/block system, a streamer dashboard, and much more — all built end-to-end with Next.js, React, TypeScript, LiveKit, and Socket.io.

---

## ⚙️ Tech Stack

| Layer | Technology |
| --- | --- |
| Framework | Next.js 14 (App Router, SSR) |
| Language | TypeScript |
| Streaming | LiveKit, RTMP / WHIP |
| Real-time Chat | Socket.io |
| Database | MySQL |
| Auth | Clerk / NextAuth |
| Styling | Tailwind CSS |

---

## 🚀 Key Features

- 📡 **Live Streaming** via RTMP / WHIP protocols
- 🌐 **Ingress generation** for OBS and other streaming software
- 🔐 **Authentication** — secure user accounts
- 📸 **Thumbnail upload** for streams
- 👀 **Live viewer count** in real-time
- 🚦 **Live status indicators**
- 💬 **Real-time chat** powered by WebSockets
- 🎨 **Unique viewer colors** in chat
- 👥 **Following system**
- 🚫 **Blocking system**
- 👢 **Kick participants** from a stream in real-time
- 🎛️ **Streamer / Creator Dashboard**
- 🐢 **Slow chat mode**
- 🔒 **Followers-only chat mode**
- 📴 **Enable / Disable chat**
- 🔽 **Collapsible layout** — hide sidebars, chat, theatre mode
- 📚 **Sidebar** with following & recommendations tab
- 🏠 **Home page** — recommends streams, sorted by live first
- 🔍 **Search results page** with unique layout
- 🔄 **Webhook sync** — user info & live status synced to DB
- 🤝 **Community tab**
- 📄 **SSR** — Server-Side Rendering throughout
- 🗺️ **Grouped routes & layouts**
- ⚡ **Blazing fast performance**
- 🎨 **Beautiful, modern UI**
- 🚀 **Production-ready deployment**

---

## 🤸 Quick Start

### Prerequisites

- Node.js 18+
- MySQL database
- LiveKit account (for streaming)
- Clerk account (for auth)

### 1. Clone the repository

```bash
git clone https://github.com/Souvik-223/orca-stream.git
cd orca-stream
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the project root:

```env
# Database
DATABASE_URL=

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
CLERK_WEBHOOK_SECRET=

# LiveKit
LIVEKIT_API_URL=
LIVEKIT_API_KEY=
LIVEKIT_API_SECRET=
NEXT_PUBLIC_LIVEKIT_WS_URL=

# App
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

### 4. Set up the database

```bash
npx prisma generate
npx prisma db push
```

### 5. Run the development server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 🧪 Demo Account (For Testing)

You can explore the app using the demo credentials below:

```bash
Email: tester@test.com
Password: Tester
```

> Use this account to test live streaming, chat, follow/block, and other features without creating a new account.

---

## 📡 Connecting to OBS

1. Go to your **Streamer Dashboard** → Keys
2. Copy your **Stream Key** and **RTMP URL**
3. Open OBS → Settings → Stream
4. Set **Service** to `Custom`, paste the URL and key
5. Hit **Start Streaming**

---

## 🗃️ Database Schema

Powered by **Prisma ORM** with **MySQL**. Key models:

- `User` — profile, auth, follow/block relations
- `Stream` — ingress keys, live status, chat settings
- `Follow` / `Block` — social graph
- `Message` — real-time chat history

---

## 🤝 Contributing

Contributions are welcome! To get started:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add your feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

Please make sure your code follows the existing conventions and passes linting before submitting.

---

## 📚 Documentation

- [LiveKit Docs](https://docs.livekit.io)
- [Next.js App Router](https://nextjs.org/docs/app)
- [Prisma ORM](https://www.prisma.io/docs)
- [Clerk Auth](https://clerk.com/docs)

---

## 📄 License

MIT © [Souvik Chakraborty](https://github.com/Souvik-223)

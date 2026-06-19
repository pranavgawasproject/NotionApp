# 📤 NotionApp

> A full-stack web app that uploads images and videos directly into a Notion database — using the official Notion API as the storage backend.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Node](https://img.shields.io/badge/Node.js-Express-green)](https://expressjs.com)
[![React](https://img.shields.io/badge/React-Frontend-61DAFB)](https://react.dev)
[![Notion API](https://img.shields.io/badge/Notion-API-000)](https://developers.notion.com)

## ✨ Features

- 🖼️ **Image / Video Upload** — multipart upload up to 20 MB
- 🔐 **Notion Auth** — uses your Notion integration token
- 📚 **Auto-Tagging** — attach captions + categories to each upload
- 🗂️ **Database-Backed** — files are pushed to a Notion DB page block
- 🎨 **Tailwind UI** — clean, modern client
- ⚙️ **Env-Driven Config** — `.env.example` ships with all required keys

## 🛠️ Tech Stack

**Frontend (client/):** React, Tailwind, PostCSS
**Backend:** Node.js, Express, Multer, CORS, dotenv
**Integration:** [`@notionhq/client`](https://github.com/makenotion/notion-sdk-js)

## 📁 Project Structure

```
.
├── client/                 # React app
│   ├── public/
│   └── src/
│       ├── App.js
│       ├── NotionUploader.js
│       └── index.js
├── server.js               # Express API
├── .env.example
└── package.json
```

## 🚀 Getting Started

### 1. Create a Notion Integration
- Go to https://www.notion.so/my-integrations
- Create a new integration, copy the **Internal Integration Token**
- Share your target Notion database with that integration

### 2. Backend

```bash
npm install
cp .env.example .env
# fill in NOTION_API_KEY and NOTION_DATABASE_ID
npm start
```

### 3. Frontend

```bash
cd client
npm install
npm start
```

Open `http://localhost:3000` and start uploading to Notion.

## 📜 License

[MIT](LICENSE) © 2026 Pranav Gawas

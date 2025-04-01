# Byte Rooms

<div align="center">


  <div>
    <img src="https://img.shields.io/badge/-TypeScript-black?style=for-the-badge&logoColor=white&logo=typescript&color=3178C6" alt="typescript" />
    <img src="https://img.shields.io/badge/-Next_JS-black?style=for-the-badge&logoColor=white&logo=nextdotjs&color=000000" alt="nextdotjs" />
    <img src="https://img.shields.io/badge/-Tailwind_CSS-black?style=for-the-badge&logoColor=white&logo=tailwindcss&color=06B6D4" alt="tailwindcss" />
  </div>

  <h3 align="center">A Meeting App</h3>
</div>

## 📋 Table of Contents

1. 🤖 [Introduction](#introduction)
2. ⚙️ [Tech Stack](#tech-stack)
3. 🔋 [Features](#features)
4. 🤸 [Quick Start](#quick-start)
5. 🕸️ [Assets & Code](#snippets)

## 🤖 Introduction

Built with the latest Next.js and TypeScript, Byte Rooms replicates Zoom, a widely used video conferencing tool. It enables users to securely log in, create meetings, and access various meeting functionalities such as recording, screen sharing, and managing participants.

## ⚙️ Tech Stack

- Next.js
- TypeScript
- Clerk
- getstream
- shadcn
- Tailwind CSS

## 🔋 Features

👉 **Authentication**: Secure authentication with Clerk, supporting social sign-on and traditional email/password methods.

👉 **New Meeting**: Start a new meeting with configurable camera and microphone settings.

👉 **Meeting Controls**: Full control over meeting aspects, including recording, emoji reactions, screen sharing, muting/unmuting, and participant management.

👉 **Exit Meeting**: Leave a meeting, or end it for all attendees.

👉 **Schedule Future Meetings**: Input meeting details to schedule future meetings.

👉 **Past Meetings List**: Access a list of previously held meetings.

👉 **View Recorded Meetings**: Review past meetings through saved recordings.

👉 **Personal Room**: Each user has a unique personal meeting link.

👉 **Join Meetings via Link**: Easily join meetings created by others using a link.

👉 **Secure Real-time Functionality**: All interactions occur in real-time while maintaining data security.

👉 **Responsive Design**: Optimized for different screen sizes and resolutions.

## 🤸 Quick Start

Follow these steps to set up the project locally.

### Prerequisites

Ensure you have the following installed:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/)

### Cloning the Repository

```bash
git clone https://github.com/realharshgautam/byterooms.git
cd byterooms
```

### Installation

Install the dependencies:

```bash
npm install
```

### Set Up Environment Variables

Create a `.env` file in the root directory and add:

```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

NEXT_PUBLIC_STREAM_API_KEY=
STREAM_SECRET_KEY=
```

Replace placeholders with your actual Clerk & getstream credentials.

### Running the Project

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🕸️ Snippets

<details>
<summary><code>app/globals.css</code></summary>

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```
</details>

<details>
<summary><code>tailwind.config.ts</code></summary>

```typescript
import type { Config } from 'tailwindcss';

const config: Config = {
  darkMode: ['class'],
  content: [
    './pages/**/*.{ts,tsx}',
    './components/**/*.{ts,tsx}',
    './app/**/*.{ts,tsx}',
    './src/**/*.{ts,tsx}',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
};

export default config;
```
</details>

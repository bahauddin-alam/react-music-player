# 🎵 Music Player

A modern, responsive web-based music player built with **React 19** and **Vite 8**. It provides a clean interface for browsing songs, managing custom playlists, and controlling audio playback.

## ✨ Features

### 🎧 Music Playback

- Play and pause tracks.
- Skip to the next or previous song.
- Seek through tracks using an interactive progress bar.
- Adjust playback volume in real time.
- View the currently playing track with visual indicators.

### 🎼 All Songs Library

- Browse the complete music collection.
- View song titles, artists, and durations.
- Identify the currently active track.

### 📁 Playlist Management

- Create playlists with custom names.
- Search for songs using live autocomplete.
- Automatically exclude songs already added to a playlist.
- Add tracks to specific playlists.
- Play songs directly from a playlist.
- Delete playlists with confirmation prompts.

### 🧭 Navigation & State Management

- Client-side routing with React Router.
- Separate views for the All Songs (`/`) and Playlists (`/playlists`) pages.
- Centralized audio and playlist state using React Context (`MusicContext`).

## 🛠️ Tech Stack

| Technology        | Purpose                           |
| ----------------- | --------------------------------- |
| React 19          | Frontend framework                |
| React Router 8    | Client-side routing               |
| Vite 8            | Development server and build tool |
| ESLint 10         | Code quality and linting          |
| HTML5 Audio API   | Audio playback and controls       |
| React Context API | Global state management           |

## 📂 Project Structure

```text
music-player/
├── index.html
├── package.json
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── index.css
    ├── contexts/
    │   └── MusicContext.jsx
    └── components/
        ├── NavBar.jsx
        ├── MusicPlayer.jsx
        ├── AllSongs.jsx
        └── Playlists.jsx
```

### Component Overview

| File               | Responsibility                                  |
| ------------------ | ----------------------------------------------- |
| `main.jsx`         | Application entry point and React root mounting |
| `App.jsx`          | Main application layout and route configuration |
| `index.css`        | Global application styles                       |
| `MusicContext.jsx` | Shared audio playback and playlist state        |
| `NavBar.jsx`       | Navigation between application pages            |
| `MusicPlayer.jsx`  | Persistent audio player and playback controls   |
| `AllSongs.jsx`     | Displays the complete music library             |
| `Playlists.jsx`    | Playlist creation, search, and management       |

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- npm (included with Node.js)

### Installation

**1. Clone the repository**

```bash
git clone <your-repository-url>
cd music-player
```

**2. Install dependencies**

```bash
npm install
```

**3. Start the development server**

```bash
npm run dev
```

**4. Open the application**

Visit the local URL displayed in your terminal, typically:

```text
http://localhost:5173
```

## 📜 Available Scripts

| Command           | Description                                                      |
| ----------------- | ---------------------------------------------------------------- |
| `npm run dev`     | Starts the development server with Hot Module Replacement (HMR). |
| `npm run build`   | Builds the application for production in the `dist/` directory.  |
| `npm run preview` | Previews the production build locally.                           |
| `npm run lint`    | Runs ESLint to identify code quality issues.                     |

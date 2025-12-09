# Rainflow Dashboard - ROG x Lamborghini Edition

## Design Philosophy
*   **Aesthetic**: Aggressive, High-Performance, Gamer-Luxury.
*   **Colors**:
    *   **ROG Red**: `#ff0033` (Accents, Alerts)
    *   **Lamborghini Yellow**: `#ffcc00` (Primary Actions, Highlights)
    *   **Carbon Black**: `#111111` (Backgrounds)
    *   **Gunmetal Grey**: `#2a2a2a` (Cards, Panels)
    *   **Neon Blue**: `#00f3ff` (Data Visualization, Tech details)
*   **Textures**: Carbon Fiber patterns, Hexagonal grids.
*   **Typography**: `Orbitron` (Headers), `Rajdhani` (Data), `Inter` (Body).

## Core Components

### 1. The Command Center (Dashboard Home)
*   **HUD Display**: Real-time stats (CPU Usage, Active Jobs, Quota Remaining).
*   **Live Feed**: Terminal-like log output of the current worker process.
*   **Quick Actions**: Large, tactile buttons for "Generate Audio", "Render Video", "Emergency Stop".

### 2. Job Queue Visualizer
*   **Kanban/List View**: Pending -> Processing -> Uploading -> Completed.
*   **Status Indicators**: Animated pulsing dots (Green = Good, Red = Error, Yellow = Busy).

### 3. Configuration Deck
*   **Sliders**: Custom styled range inputs for Audio Duration, Bitrate.
*   **Toggles**: Cyberpunk-style toggle switches for "Auto-Upload", "Loop Video".
*   **API Key Manager**: Encrypted vault interface for managing Google Accounts.

## Tech Stack
*   **Framework**: React + Vite + TypeScript
*   **Styling**: Tailwind CSS (v3/v4)
*   **Animations**: Framer Motion (for smooth HUD transitions)
*   **Icons**: Lucide React (with glowing effects)

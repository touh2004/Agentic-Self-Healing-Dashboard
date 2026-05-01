# MicroChat - Real-Time Chat with Self-Healing Platform

A modern real-time chat application built on microservices architecture, integrated with an AI-driven self-healing cloud platform for autonomous system monitoring and recovery.

🌟 **Live Demo Dashboard:** [View Live on Vercel](https://agentic-self-healing-dashboard.vercel.app/dashboard)

## Features

### Real-Time Chat
- Instant messaging with WebSocket support
- Presence indicators (online/offline status)
- Live typing indicators
- Message edit and delete functionality
- Direct messages and group conversations

### Self-Healing Platform
- Real-time system health monitoring
- Autonomous anomaly detection
- Automatic remediation triggers
- Root cause analysis
- Service dependency mapping
- Incident timeline and history

### Microservices Architecture
- **Authentication Service** - User registration and login
- **Messaging Service** - Message handling and storage
- **Presence Service** - User online/offline tracking
- **Conversation Service** - Conversation management
- **Monitoring Service** - System health and metrics

### Chaos Engineering
- CPU spike injection
- Memory leak simulation
- Service crash testing
- Real-time recovery visualization

## Tech Stack

- **Frontend**: Next.js 16 + React 19 + TypeScript
- **UI Framework**: shadcn/ui with Tailwind CSS 4.2
- **Real-time**: Socket.io for WebSocket communication
- **Charts**: Recharts for data visualization
- **Icons**: Lucide React
- **Design**: Glassmorphism dark mode aesthetic

## Project Structure

```text
/app
  ├── (auth)                 # Authentication pages
  ├── (protected)            # Protected routes (requires login)
  │   ├── chat               # Chat interface
  │   ├── dashboard          # Monitoring dashboard
  │   ├── services           # Services status page
  │   └── settings           # User settings
  ├── api                    # API routes
  └── page.tsx               # Homepage

/components
  ├── Chat                   # Chat components
  ├── Dashboard              # Dashboard components
  └── Layout                 # Layout components

/hooks
  ├── useAuth                # Authentication state
  ├── useChat                # Chat state management
  └── useMonitoring          # Monitoring state

/styles
  └── globals.css            # Global styles & theme

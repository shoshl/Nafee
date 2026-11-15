# Nafee AI نفيع

A teaching assistant platform that helps teachers identify and close learning gaps at scale.

## How It Works

1. **Upload** — Teachers submit student assignments (PDF or image)
2. **Analyze** — Gemini AI reviews each submission
3. **Insights** — The platform returns per-student results and class-wide performance gaps
4. **Remediate** — Targeted, AI-generated remediation plans are created for students who need them

## Features

- **Dashboard** — Class overview with key metrics, weakest topics, and mastery distribution
- **Upload** — Submit student assignments for AI analysis
- **Students** — Student roster with performance status and risk flags
- **Class Analytics** — Topic-level performance breakdown across the class
- **Treatment Plans** — AI-generated, per-student remediation plans
- **Reports** — Performance trends and exportable summaries
- **Settings** — Account and notification preferences

## Tech Stack

- **Frontend:** React 19, TypeScript, Vite, Tailwind CSS v4, Recharts
- **Backend:** Node.js, Express
- **AI:** Google Gemini (`@google/generative-ai`)
- **Package manager:** pnpm

## Getting Started

### Prerequisites

- Node.js 22
- pnpm 10+

### Installation

```bash
pnpm install
```

### Development

```bash
pnpm dev
```

The app runs on `http://localhost:8443` by default.

### Backend

The API server lives in `server/`. It requires a Gemini API key:

```bash
# server/.env
GEMINI_API_KEY=your_key_here
```

## Project Status

This is an active MVP under development. The frontend interface is complete; the core AI pipeline (**upload → analysis → structured results → remediation plan**) is in progress and not yet fully connected end-to-end.

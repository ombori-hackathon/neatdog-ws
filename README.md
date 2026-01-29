# Neatdog

A collaborative dog care tracking app for households and families.

## What is it?

Neatdog helps multiple people coordinate care for a shared dog. Create a "pack" (your household), add your dog, and track activities together.

## Features

- **Packs** - Create a group for your household and invite members via shareable codes
- **Dog Profiles** - Add your dog with name, breed, and photo
- **Activity Logging** - Track walks, feeding, grooming, vet visits, and more
- **Stats & Streaks** - See activity counts and maintain care streaks

## Architecture

| Component | Technology | Location |
|-----------|------------|----------|
| API | FastAPI + PostgreSQL | `services/api/` |
| macOS Client | SwiftUI | `apps/macos-client/` |

## Quick Start

```bash
# Start database
docker compose up -d

# Run API
cd services/api && uv run fastapi dev app/main.py

# Run macOS client (separate terminal)
cd apps/macos-client && swift run NeatdogClient
```

## API Docs

Once running: http://localhost:8000/docs

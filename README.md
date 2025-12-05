# Project for Fur-Ever Wild Rehabilitation

## Tech Stack
### Frontend
- **React 19**
- **TypeScript**

### Backend
- **Node.js 20**



## Getting Started Start
### Prerequisites
- **Git**
- **Docker Desktop**
- **NodeJS**

### Setup
```bash
# 1. Clone repo
git clone https://github.com/tmublueprint/bp-furever.git

# 2. Create environment file
cp backend/env.example backend/.env (will change this)

# 3. Start
docker compose up --build

# Install all npm packages ig
npm install
npm run postinstall
```

### Access Points
- **Frontend**: http://localhost:3004
- **Backend**: http://localhost:3003/api/health

## Development Workflow

### Daily Development
```bash
# Pull latest changes
git pull
```

### Configuration Updates
```bash
# When Dockerfile, compose.yaml, or package.json changes
git pull
docker compose down
docker compose up --build
```

### Docker Commands
```bash
docker compose up --build    # Start everything
docker compose down          # Stop everything
docker compose restart       # Restart containers
```

## Project Structure

```
bp-furever/
├── frontend/            # React frontend
│   ├── src/
│   │   ├── components/
│   │   │   └── <component name>/
│   │   ├── pages/
│   │   │   └── <page name>/
│   │   │   │   ├── index.tsx
│   │   │   │   └── style.css
│   ├── public/
│   ├── Dockerfile
│   └── package.json
├── backend/
│   ├── src/
│   ├── Dockerfile
│   ├── env.example
│   └── package.json
├── compose.yaml        # Docker Compose
├── .gitignore          # Git ignore
└── README.md
```

## Contributing

1. Clone repo
2. Create `.env` file (`cp backend/env.example backend/.env`) (we will change this in the future)
3. Start development (`docker compose up --build`)
4. Make changes (hot reload handles updates)
5. Commit and push

## License

MIT
# Environment Variables Management

This folder contains environment-specific configuration files for different applications.

## Structure

```
env/
├── insightforge/
│   └── .env          # InsightForge-specific environment variables
├── brandedge/
│   └── .env          # BrandEdge-specific environment variables
└── README.md         # This file
```

## Purpose

Each application uses its own OpenAI API key and potentially different database configurations:

- **InsightForge**: Uses one OpenAI API key for its marketing modules
- **BrandEdge**: Uses a different OpenAI API key for brand analysis

## Usage

### Running InsightForge

```bash
# Load InsightForge environment
export $(cat env/insightforge/.env | xargs)
Rscript app_insightforge.R
```

Or use the launcher script:
```bash
./run_insightforge.sh
```

### Running BrandEdge

```bash
# Load BrandEdge environment
export $(cat env/brandedge/.env | xargs)
Rscript app_brandedge.R
```

Or use the launcher script:
```bash
./run_brandedge.sh
```

## Environment Variables

### Database (Common)
- `PGHOST`: PostgreSQL host
- `PGPORT`: PostgreSQL port
- `PGUSER`: PostgreSQL username
- `PGPASSWORD`: PostgreSQL password
- `PGDATABASE`: PostgreSQL database name
- `PGSSLMODE`: SSL mode (require/prefer/disable)

### API Keys (App-Specific)
- `OPENAI_API_KEY`: OpenAI API key (different for each app)

### Application Config
- `APP_NAME`: Application name
- `APP_CONFIG_FILE`: Path to YAML configuration file

## Security Notes

⚠️ **IMPORTANT**:
- Never commit `.env` files to version control
- Each `.env` file is git-ignored by default
- Keep API keys secret and rotate them regularly
- Use different API keys for different applications to track usage

## Adding New Applications

1. Create a new subfolder: `mkdir env/newapp`
2. Create `.env` file: `touch env/newapp/.env`
3. Copy template from existing .env and update values
4. Create launcher script (optional)
5. Update this README

## Last Updated

2025-10-06

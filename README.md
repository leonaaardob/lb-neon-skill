# Neon Database Skill

Complete Neon Serverless Postgres documentation as an OpenClaw AgentSkill.

## What's Included

- **546 markdown files** with full Neon documentation
- Introduction, architecture, and core concepts
- Serverless PostgreSQL fundamentals
- Database branching and autoscaling
- Vercel, Drizzle, Prisma, Next.js integrations
- Better Auth, Auth.js, Clerk authentication guides
- Connection pooling and serverless optimization
- PostgreSQL extensions (pgvector, PostGIS, timescaledb)
- API reference and neonctl CLI documentation
- AI/ML features and pgvector guides
- Security best practices and compliance

## Installation

### From Local Directory

```bash
clawhub install /path/to/neon-skill
```

### From Archive

```bash
clawhub install neon.skill
```

## Usage

This skill is automatically loaded by OpenClaw when available in the workspace skills directory.

Agents with this skill can answer questions about:

- Setting up and configuring Neon projects
- Connecting Neon to frameworks (Vercel, Next.js, Drizzle, Prisma)
- Database branching workflows for preview environments
- Serverless optimization and connection pooling
- PostgreSQL extensions and best practices
- API and CLI usage (neonctl)
- AI/ML features (pgvector, embeddings, RAG)

## Documentation Source

Official documentation from:
- Website: https://neon.tech/docs
- Repository: https://github.com/neondatabase/website
- Extracted: 2026-02-07

## File Structure

```
neon/
├── SKILL.md              # Skill metadata and description
├── README.md             # This file
├── .gitignore            # Git ignore rules
└── docs/                 # Full Neon documentation (546 MD files, 6.8MB)
    ├── introduction/
    ├── get-started/
    ├── serverless/
    ├── connect/
    ├── manage/
    ├── extensions/
    ├── guides/
    ├── reference/
    └── ...
```

## Tags

`neon` `postgresql` `serverless` `database` `vercel` `drizzle` `prisma` `nextjs` `branching` `autoscaling` `documentation`

## License

Documentation content © Neon Corporation.
Skill package © OpenClaw Community, MIT License.

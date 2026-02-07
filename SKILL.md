---
id: neon
name: Neon Database
version: 1.0.0
author: OpenClaw Community
description: Complete Neon Serverless Postgres documentation. Covers serverless setup, branching, autoscaling, integrations (Vercel, Drizzle, Prisma), connection pooling, extensions, and best practices.
categories:
  - database
  - documentation
  - postgresql
  - serverless
tags:
  - neon
  - postgresql
  - serverless
  - database
  - vercel
  - drizzle
  - prisma
  - nextjs
  - branching
  - autoscaling
homepage: https://neon.tech
repository: https://github.com/neondatabase/neon
documentation: https://neon.tech/docs
---
## ⚠️ Security Notice

This skill contains Neon Database documentation with command examples. Commands are **for reference only** and should NEVER be auto-executed by agents without explicit user approval.

# Neon Database Documentation

Complete Neon Serverless Postgres documentation extracted from the official Neon website repository.

## Contents

This skill includes **546 markdown files** (6.8MB) covering:

### Core Concepts
- **Introduction** - What is Neon, architecture, and core concepts
- **Get Started** - Quick start guides and initial setup
- **Serverless** - Serverless PostgreSQL fundamentals

### Features
- **Branching** - Database branching workflows (preview, development)
- **Autoscaling** - Compute autoscaling and scale-to-zero
- **Connection Pooling** - Connection pooling and serverless optimization
- **Data API** - HTTP-based data access

### Integrations
- **Vercel** - Vercel integration (env vars, preview branches)
- **Drizzle ORM** - Drizzle setup and migrations
- **Prisma** - Prisma integration
- **Next.js** - Next.js + Neon patterns
- **Auth** - Authentication integrations (Better Auth, Auth.js, Clerk, etc.)

### Database Management
- **Manage** - Projects, branches, databases, roles, compute
- **Import** - Data import strategies (PostgreSQL dump, CSV, etc.)
- **Extensions** - PostgreSQL extensions (pgvector, PostGIS, timescaledb, etc.)
- **Functions** - User-defined functions and stored procedures
- **Data Types** - PostgreSQL data types and Neon-specific types

### Reference
- **API Reference** - Neon API endpoints and CLI (neonctl)
- **Security** - Security best practices, encryption, compliance
- **PostgreSQL** - PostgreSQL-specific documentation
- **AI/ML** - AI embeddings, RAG, pgvector

### Developer Resources
- **Guides** - Step-by-step tutorials for common use cases
- **Community** - Community resources and support channels

## Usage

This skill provides comprehensive documentation for:

1. **Setting up Neon** - Creating projects, connecting to databases
2. **Integrations** - Connecting Neon to frameworks and ORMs (Vercel, Drizzle, Prisma, Next.js, Better Auth)
3. **Advanced Features** - Branching, autoscaling, connection pooling
4. **Best Practices** - Serverless optimization, security, performance
5. **API & CLI** - Programmatic access via API and neonctl CLI

## File Structure

```
docs/
├── introduction/        # Core concepts, architecture
├── get-started/         # Quick start guides
├── serverless/          # Serverless PostgreSQL
├── connect/             # Connection strings, pooling
├── data-api/            # HTTP data access
├── manage/              # Project and database management
├── import/              # Data import guides
├── extensions/          # PostgreSQL extensions
├── functions/           # User-defined functions
├── data-types/          # PostgreSQL data types
├── reference/           # API reference, CLI
├── security/            # Security best practices
├── auth/                # Authentication integrations
├── ai/                  # AI/ML features (pgvector)
├── guides/              # Step-by-step tutorials
├── community/           # Community resources
└── shared-content/      # Reusable documentation snippets
```

## Documentation Source

Official Neon documentation extracted from:
- Repository: https://github.com/neondatabase/website
- Website: https://neon.tech/docs
- Last Updated: 2026-02-07

## License

Documentation content © Neon Corporation. Used for educational purposes under fair use.
Skill package © OpenClaw Community, MIT License.

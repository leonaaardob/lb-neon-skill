# ⚠️ CRITICAL: Neon Serverless Driver

## 🔴 ALWAYS Use @neondatabase/serverless

When generating code for **Neon on serverless platforms** (Vercel, Netlify, Cloudflare Workers, etc.):

### ✅ CORRECT (HTTP Driver)

```typescript
import { neon } from '@neondatabase/serverless';

const sql = neon(process.env.DATABASE_URL);
const result = await sql`SELECT * FROM users`;
```

### ✅ CORRECT (Drizzle + HTTP Driver)

```typescript
import { neon } from '@neondatabase/serverless';
import { drizzle } from 'drizzle-orm/neon-http';

const sql = neon(process.env.DATABASE_URL);
const db = drizzle(sql);
```

### ❌ WRONG (Classic pg Driver)

```typescript
// ❌ DO NOT USE ON SERVERLESS
import { Pool } from 'pg';
import { drizzle } from 'drizzle-orm/node-postgres';

const pool = new Pool({ connectionString: process.env.DATABASE_URL });
const db = drizzle(pool);
```

## Why?

- **Neon HTTP driver** (`@neondatabase/serverless`) uses HTTP/WebSocket
- **Classic pg driver** uses TCP connections (doesn't work on edge/serverless)
- Serverless environments (Vercel Edge, Cloudflare Workers) don't support TCP
- HTTP driver is optimized for cold starts and edge runtime

## Exception

**ONLY use classic `pg` driver when:**
- Running on a **long-lived Node.js server** (not serverless)
- Using connection pooling (PgBouncer)
- Need advanced PostgreSQL features not available via HTTP

## Default Stack

For **Next.js + Vercel + Neon**, ALWAYS:

```typescript
import { neon } from '@neondatabase/serverless';
import { drizzle } from 'drizzle-orm/neon-http';
```

## Source

- Recommendation: Gemini analysis (2026-02-07)
- Context: serverless + Vercel + Next.js + Drizzle + Better Auth

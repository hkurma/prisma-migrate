# Prisma

Example project for database schema migrations using [Prisma (https://www.prisma.io/)](https://www.prisma.io/)

### Prerequisites

- Node
- Docker

### Environment Variables

Create a .env file in the root folder and add DATABASE_URL to the file.

```
DATABASE_URL="postgresql://admin:password@localhost/prisma?schema=public"
```

### Start Postgres SQL Server

Docker is used for running a local Postgres SQL container. 

```
docker-compose up -d
```

### Create and Apply Migrations

In development environments, command to generate and apply migrations. Creates migration script files in migrations folder.

```
npm run dev
```

### Deploy Migration Script

In testing or production environment, command to apply the migrations already created.

```
npm run deploy
```

### Studio

Opens Studio - Explorer for the database

```
npm run studio
```

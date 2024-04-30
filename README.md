# Clean Architecture Template

A Node template that follows the Clean Architecture principles and encourages established practices.

## Features

- TypeScript first
- Dependency injection via Awilix
- CQRS (Command Query Responsibility Segregation)
- Automatic API documentation via Swagger
- Built with scalability and performance in mind by using Fastify (see [benchmarks](https://www.fastify.io/benchmarks))
- Built in logging with Pino
- Comprehensive testing including unit and functional tests
- Prisma ORM integration

## Getting Started

1. Install the latest [Node.js LTS](https://nodejs.org/en/)
2. Install Docker and ensure that it is running
3. Create .env file `cp .env.example .env`
4. Install project dependencies by running `npm install`
5. Start Docker (local Postgres instance) `docker-compose up -d`
6. Create database `npx prisma migrate deploy`
7. Start development server `npm run dev`
8. Navigate to Swagger ([http://localhost:3000/api-docs](http://localhost:3000/api-docs))

## Scripts

**Build production bundle**

```
npm run build
```

**Lint project (eslint)**

```
npm run lint
```

**Start development server**

```
npm run dev
```

**Run all tests**

```
npm test
```

**Run unit tests**

```
npm run test:unit
```

**Run functional tests (API tests)**

```
npm run test:functional
```
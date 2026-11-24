# Cinebh

CinemaApp is an internship project for a cinema ticketing and management application.

## Repositories

- [Frontend](https://github.com/Cinebh/cinebh-frontend) — React, TypeScript, Vite
- [Backend](https://github.com/Cinebh/cinebh-backend) — Java, Spring Boot, PostgreSQL

## Getting Started

1. Install Git and start Docker Desktop (Linux containers, Compose 2.20.3+).
2. Clone both repositories:

   ```powershell
   mkdir Cinebh
   cd Cinebh
   git clone https://github.com/Cinebh/cinebh-backend.git
   git clone https://github.com/Cinebh/cinebh-frontend.git
   ```

3. Create the backend configuration (keep `.env` if it already exists):

   ```powershell
   cd cinebh-backend
   Copy-Item .env.example .env
   ```

4. Set `DB_PASSWORD` in `.env`. For an existing database, use its current password.
5. Start the complete application:

   ```powershell
   cd ../cinebh-frontend
   docker compose up
   ```

6. Wait for seed completion, then open [the application](http://localhost:3000)
   or [Swagger UI](http://localhost:8080/swagger-ui.html).

Stop with `Ctrl+C`. Next time, run `docker compose up` from `cinebh-frontend/`.

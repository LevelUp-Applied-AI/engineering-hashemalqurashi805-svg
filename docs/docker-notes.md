# Docker Task Notes

## Resource Configuration (Step 2)
- Created `.wslconfig` file in the user profile directory.
- Configured memory limit to 4GB using `memory=4GB`.

## Docker Engine Verification (Step 4)
- **Docker Version:** 27.2.1.
- **Memory:** Confirmed Total Memory: **3.825 GiB** as shown in `docker info`.
- **Environment:** Docker Desktop is running on **WSL2 (Ubuntu)**.

## Postgres Container (Step 7 & 8)
- **Command used:** `docker run -d --name pg-prework -e POSTGRES_PASSWORD=prework -p 5432:5432 postgres:15-alpine`.
- **Logs output:** `database system is ready to accept connections`.
- **Confirmation:** The log `database system is ready to accept connections` was verified.

## Stop and Restart (Step 9)
- Successfully tested `docker stop pg-prework`.
- Successfully tested `docker restart pg-prework`.
- Verified container is **Up** and running again using `docker ps`.

## Challenges Faced
- None.
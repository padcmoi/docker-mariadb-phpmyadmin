# MariaDB & phpMyAdmin Docker Setup

## Usage

1. Clone this repository.
2. Copy `.env.sample` to `.env` and fill in your credentials.
3. Run:
   ```bash
   docker compose up -d --build
   ```
4. Access phpMyAdmin at the address and port you set in `.env` (default: [http://127.0.0.1:53081](http://127.0.0.1:53081)).

## Environment Variables

- `MARIADB_ROOT_PASSWORD`: Root password for MariaDB
- `MARIADB_DATABASE`: Database name
- `MARIADB_USER`: Database user
- `MARIADB_PASSWORD`: User password
- `PHPMYADMIN_BIND`: Address and port for phpMyAdmin (e.g. `127.0.0.1:53081`)

## Notes
- The `.env` file is ignored by git.
- Data is persisted in the `data/` folder.

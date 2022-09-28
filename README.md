# docker-postgres-pgadmin4
Docker Compose YAML file for PostgreSQL and pgAdmin4

You can set values for environment variables using a .env file. Compose automatically looks for an .env file in the folder of your Compose file. 
If it's not in the same directory, you can specify the location explicitly, e. g.:
```docker compose --env-file ./config/.env.dev up```

# Adding a Server in pgAdmin4

After both containers have started, pgAdmin4 is running on [http://localhost:5050](http://localhost:5050). You can now add a new server connection.
For hostname/address, use the PostgreSQL container name ("postgres_container").

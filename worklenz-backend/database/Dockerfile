# Use the official PostgreSQL image as the base
FROM postgres:14

# Set environment variables for PostgreSQL
ENV POSTGRES_USER=worklenz_backend
ENV POSTGRES_PASSWORD=securepassword123
ENV POSTGRES_DB=worklenz_db

# Copy all SQL scripts into the container's initialization directory
# COPY ./backend/database/ /docker-entrypoint-initdb.d/
COPY . /docker-entrypoint-initdb.d/


# Ensure the scripts have the appropriate permissions
RUN chmod -R 755 /docker-entrypoint-initdb.d/

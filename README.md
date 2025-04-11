# 🚀 PostgreSQL + pgAdmin Docker Setup

This repository contains a simple Docker Compose setup for running PostgreSQL with pgAdmin. Ideal for local development and testing.

## 📦 Services

- **PostgreSQL**: Relational database server  
- **pgAdmin 4**: Web-based GUI to manage PostgreSQL databases

## 🛠️ Setup

### 1. Clone this repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Start the services

```bash
docker-compose up -d
```

### 3. Access pgAdmin

Open your browser and go to: [http://localhost:8080](http://localhost:8080)

Use the following credentials:

- **Email**: abc@gmail.com  
- **Password**: secret

---

### 4. Register a new server in pgAdmin

Click "Add New Server" and enter:

**General Tab:**
- **Name**: Local PostgreSQL

**Connection Tab:**
- **Host name/address**: postgres  
- **Port**: 5432  
- **Username**: postgres  
- **Password**: mypass123

✅ Make sure the **host** is `postgres` (the service name in `docker-compose.yml`), **not** `localhost`.

---

### 📁 Volumes

PostgreSQL data is persisted in a named Docker volume: `pgdata`

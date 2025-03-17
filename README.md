# Docker Commands for FastAPI 🚀

### 📦 Building & Managing Images
1. **Build Docker Image:**  
```bash
docker build -f Dockerfile.dev -t my-dev-image .
```
2. **List Docker Images:**  
```bash
docker images
```
3. **Inspect Docker Image:**  
```bash
docker inspect my-dev-image
```

### 🐳 Running & Managing Containers
4. **Run Container (Interactive Mode):**  
```bash
docker run --name dev-cont1 -it my-dev-image
```
5. **Run Container (Detached Mode with Port Mapping):**  
```bash
docker run -d --name dev-cont1 -p 8000:8000 my-dev-image
```
6. **Check Running Containers:**  
```bash
docker ps
```
7. **Check All Containers (Including Stopped Ones):**  
```bash
docker ps -a
```
8. **View Container Logs:**  
```bash
docker logs dev-cont1
```
9. **View Container Logs in Real-Time:**  
```bash
docker logs -f dev-cont1
```
10. **Stop a Running Container:**  
```bash
docker stop dev-cont1
```
11. **Remove a Container:**  
```bash
docker rm dev-cont1
```

### 🔨 Rebuilding & Removing Images
12. **Rebuild Docker Image (If Code Changes):**  
```bash
docker build -f Dockerfile.dev -t my-dev-image .
```
13. **Remove Old Image (If Necessary):**  
```bash
docker rmi my-dev-image
```

### 🌐 Testing FastAPI API
14. **Testing API (From Host Machine - Windows):**  
```bash
curl http://localhost:8000
```
Or open your browser and visit:  
```
http://localhost:8000
```

15. **Access FastAPI Docs:**  
- Swagger UI: [http://localhost:8000/docs](http://localhost:8000/docs)  
- ReDoc: [http://localhost:8000/redoc](http://localhost:8000/redoc)


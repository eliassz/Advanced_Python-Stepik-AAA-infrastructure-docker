# Homework
Docker lecture repository at [Avito's Analytics Academy](https://avito-analytics-academy.ru/) Data Science course.

### Step 1:
Run docker-compose file:
```bash
docker-compose up -d
```
Then go to this url:
```bash
http://127.0.0.1:8080/books
http://127.0.0.1:8080/authors
http://127.0.0.1:8080/metrics
```
Here you can see how many times you have opened `/books`, `/authors` or some other path. There is also a lot of additional information - server response time, etc.

### Step 2.
Make requests:
```bash
for i in $(seq 1 15); do \
  curl http://127.0.0.1:8080/books; \
  curl http://127.0.0.1:8080/authors; \
done
```

### Step 3.
Open [grafana](http://localhost:3000/d/_eX4mpl3) in your browser.

### Step 4.
Down all containers.
```bash
docker-compose down
```

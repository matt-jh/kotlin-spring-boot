```bash
curl http://localhost:8080/
```

```
mvn spring-boot:run in the root directory of the application
```

```bash
# adds a new customer
curl -H "Content-Type: application/json" -X POST -d '{
    "firstName": "Bruno",
    "lastName": "Krebs"
}'  http://localhost:8080/customers
```

```bash
# retrieves all customers
curl http://localhost:8080/customers
```

```bash
# updates customer with id 1
curl -H "Content-Type: application/json" -X PUT -d '{
    "id": 1,
    "firstName": "Bruno",
    "lastName": "Simões Krebs"
}'  http://localhost:8080/customers/1
```

```bash
# deletes customer with id 1
curl -X DELETE http://localhost:8080/customers/1
```
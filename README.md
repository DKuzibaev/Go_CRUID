# Simple CRUD API on Golang

This is a simple CRUD API built with Golang using **Gorilla MUX** for handling `CREATE`, `READ`, `UPDATE`, and `DELETE` operations.  

> ⚠️ Note: In this project, all data is stored in slices without using a database. However, a `docker-compose` file is provided so you can easily spin up and integrate a database if needed.  

All endpoints were tested with **Postman**.

---

## API Structure

### Routers
The API has the following routes:

- `GET /movies` — Get all movies  
- `GET /movies/:id` — Get a movie by ID  
- `POST /movies` — Create a new movie  
- `PUT /movies/:id` — Update a movie by ID  
- `DELETE /movies/:id` — Delete a movie by ID  

### Functions
Each route corresponds to a function in the code:

| Function        | Description       |
|-----------------|-----------------|
| `getMovies`     | Get all movies   |
| `getMovie`      | Get movie by ID  |
| `createMovie`   | Create a movie   |
| `updateMovie`   | Update a movie   |
| `deleteMovie`   | Delete a movie   |

### Endpoints & Methods

| Endpoint        | HTTP Method      |
|-----------------|----------------|
| `/movies`       | GET            |
| `/movies/:id`   | GET            |
| `/movies`       | POST           |
| `/movies/:id`   | PUT            |
| `/movies/:id`   | DELETE         |

---

### Testing
Use **Postman** or any API client to test all endpoints.

### Future Improvements
- Integrate a real database (PostgreSQL or MySQL)  
- Add input validation and error handling  
- Implement authentication and authorization

# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
This is a place to store the data and be able to support multiple users
accessing the app.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
Controller```

Why don't we use views in our interpretation of the MVC pattern?

```md
??
```

What does C.R.U.D stand for?

```md
CREATE READ UPDATE DESTROY```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
GET
POST
PATCH
PUT
DELETE```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
API="${API_ORIGIN:-http://localhost:4741}"
URL_PATH="/people/1"
curl "${API}${URL_PATH}" \
  --include \
  --request GET \
  --header "Authorization: Token token=$TOKEN"```

What is the command to generate a new rails-api app?

```bash
rails new
```

What is the command to start an instance of a rails server?

```bash
bins/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
db: drop
db: create
db: migrate
db: seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate scaffold Pet
```

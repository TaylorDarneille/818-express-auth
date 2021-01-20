# Express Auth Boilerplate

---
## How to set up:

1. Fork & Clone

2. Install dependencies
```
npm i
```

3. [OPTIONAL] Change the database names in `config/config.json` to names of your choosing:
```json
{
  "development": {
    "database": "<insert develop db name here>",
    "host": "127.0.0.1",
    "dialect": "postgres"
  },
  "test": {
    "database": "<insert test db name here>",
    "host": "127.0.0.1",
    "dialect": "postgres"
  },
  "production": {
    "database": "<insert poduction db name here>",
    "host": "127.0.0.1",
    "dialect": "postgres"
  }
}
```

**Note:** If your database requires a username and password, you'll need to include these fields as well.

4. Create a database
```
sequelize db:create
```

5. Migrate the `user` model to your database
```
sequelize db:migrate
```

6. Add `SESSION_SECRET` and `PORT`environment variables in a `.env` file

7. Run `nodemon` to start up app
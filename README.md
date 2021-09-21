# sinatra_todos_db

## Purpose of Project 
Take a small web application that was using sessions to persist its data and modify
it to use a PostgreSQL database instead. 

## Particulars of Project:

- Extract the session-specific functionality into the `SessionPersistence` class.
- Replace our use of `SessionPersistence` with `DatabasePersistence` to store data 
  in a different location without making other changes to the application.
- Safely handle inserting parameters into SQL statements with `PG::Connection#exec_params`.
- Use a `configure(:development)` block for environment-specific settings.
- Reload our code in development using `sinatra/reloader`.
- Log database queries made by our application.

## Where to find the application:
https://ls-josh-sinatra-todos-db.herokuapp.com/lists

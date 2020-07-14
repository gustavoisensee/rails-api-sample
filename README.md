# Rails API Sample
The aim of this project is to learn some concept of rails api

## Requirements

* make sure you have ruby 2.6.2 or highier
* aslso rails 6.0.0 or highier

## Running

* `rails server`

##  Learnings

### creating the project

* `rails new folder --api`
* `rails g model User first_name:string last_name:string` this creates the `db/migrate/script` that needs to be run with the next command
* `rails db:migrate` this executes the migration scripts


### extra changes

* **Add new column:** `rails g migration add_email_to_users email:string` this creates a migration script to add email to user table
* **Remame column name:** `rails g migration rename_column` and add the following code inside of `change` function
  * `rename_column :table_name, :old_column, :new_column`
* **Execute migration scripts:** after create migration scripts you must execute: `rails db:migration`
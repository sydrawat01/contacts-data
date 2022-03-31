# Contacts API

## Install MonngoDB on local system

1. `xcode-select --install`

2. `brew tap mongodb/brew`

3. `brew install mongodb-community@5.0`

4. `brew install --cask mongodb-compass`

## Setup & run MongoDB instance

1. `sudo mkdir /System/Volumes/Data/data/db`

2. `sudo chown -R sid /System/Volumes/Data/data/db`

3. `mongod --dbpath /System/Volumes/Data/data/db`

4. `mongosh`

5. `brew services start mongodb-community`

6. Connect the Mongo Compass service after running the above commands.

APIs available in this service

```text
// Retrieve all contacts

GET  /contacts

// Create new contact
POST /contacts

// Retrieve a specific single contact
GET  /contacts/:id

// Update a single contact by id.
PUT  /contacts/:id

//Remove a specific contact by id

DELETE /contacts/id

```

Tools used

1. `expressjs`
2. `mongoosejs`

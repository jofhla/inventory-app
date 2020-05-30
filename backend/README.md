# Inventory App Backend

## Setup

This backend is setup to work with docker, you can find out about docker and how to install it [here](https://www.docker.com/).

1. Install package dependencies 

```sh
npm install
```

2. Copy the .env.sample file to .env

```sh
cp .env.sample .env
```

3. Update .env as needed

| Environment Variable | Description |
| -----------         | ----------- |
| POSTGRES_PASSWORD   | The password used to access the database, including the Adminer UI |
| POSTGRES_USER       | The username used to access the database, including the Adminer UI |
| POSTGRES_DB         | The name of the database |

4. Start up Database

```sh
docker-compose up
```

**Windows Error**

If you are running Docker on a Windows operating system, you will run into issues when you try to run the ```docker-compose up``` command. 

Please check out this [issue](https://github.com/CodingGarden/inventory-app/issues/1) for further details.

## Adminer UI.

By default the Adminer UI is accessible at http://localhost:8090.

## Database Structure
----------------
### Model a SQL Database

Every Record will have:
Created At - datetime
Updated At - datetime
Deleted At - datetime

#### Entities in an Home Inventory System

* [x] User
* [ ] Item
* [x] Item Type
* [ ] Comment
* [x] Manufacturer
* [ ] Warranty
* [x] Item Location
* [ ] Item Purchase Location

#### Seed the Database

* [x] User
* [ ] Countries - Partial, more to do!
* [ ] US States - Partial, more to do!
* [ ] Item Types
* [ ] Location

# Ecoleta_NLW_2

To init this project follow the steps:

in [./server](server) run: 
- `npm install` to install Node dependencies;
- `npm run knex:migrate` to create the database;
- `npm run knex:seed` to insert seed values of items in items table;
- Add images in [uploads](server/uploads), these are images of items we just created;
- `npm run dev` to start run the server application;

Ok, now the server is running in localhost:3333 as defined in [src/server.ts](server/src/server.ts). It's important check the [src/controllers](server/src/controllers) files, because there is setted static external IPs we will use to access files from the mobile (external) application.

Ps: The npm run commands are defined in [package.json](server/package.json)



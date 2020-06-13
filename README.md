# Ecoleta_NLW_2

To init this project follow the steps:

In [./server](server) run: 
- `npm install` to install Node dependencies;
- `npm run knex:migrate` to create the database;
- `npm run knex:seed` to insert seed values of items in items table;
- Add images in [uploads](server/uploads), these are images of items we just created;
- `npm run dev` to start run the server application.

Test the server in your browser using http://localhost:3333/items, a JSON list of items must be loaded.

Ok, now the server is running in localhost:3333 as defined in [src/server.ts](server/src/server.ts). It's important check the [src/controllers](server/src/controllers) files, because there is setted static external IPs we will use to access files from the mobile (external) application.

> The npm run commands are defined in [package.json](server/package.json)

In [./web](web) run: 
- `npm install` to install Node dependencies;
- `npm start` to start the application.

There are no more steps here, a new tab of your browser will open in http://localhost:3000/ and you must see the application home page.
Here you can create some collection points (pontos de coleta) to see them after in mobile app. 

Now it's the gran finale, the mobile app will be born. In this project we are getting help from https://expo.io/ to build the react-native application directly in mobile device (you can use a simulator too), so the first step is download Expo from your device app store.

In [./mobile](mobile) run: 
- `npm install` to install Node dependencies;
- `npm start` to start the application.

A new browser tab will open, there you can see logs, running informations, QR Code of application connection, and set configurations. Connect your mobile device and PC in the same network connection and it's possible to use LAN connection of Expo (another options are able following Expo documentation).

- Open, Expo app on the mobile device;
- Scan QR Code of application connection.

Wait a moment to load the app and then browse it. Write UF and City of the point you created in web application, click enter, and select items the point collect, the point will appear in the map in the same location you choose before

Done! 

Text Editor Application

This text editor requires a number of methods and stores data to an IndexedDB database to be built up.

### Installation

This application will require the installation of Node.js and various npm packages.

- Node Package Manager (npm) is a software manager and installer which puts the modules in place so that the node project can utilize it. It manages dependency conflicts intelligently and is initialized using **npm init**. The package.json will be generated and will contain all the details of the application in which the user has inputted during the npm initialization.

- This application will use the following npm packages:
  - [express](express.js)
  - [webpack](https://www.npmjs.com/package/webpack)
  - [webpack-dev-server](https://www.npmjs.com/package/webpack-dev-server)
  - [webpack-pwa-manifest](https://www.npmjs.com/package/webpack-pwa-manifest)
  - [babel](https://babeljs.io/)
  - [css-loader](https://www.npmjs.com/package/css-loader)
  - [concurrently](https://www.npmjs.com/package/concurrently)
  - [idb](https://www.npmjs.com/package/idb)

The required modules are bundled in the package.json file, and at the CLI or integrated terminal, type in **npm run install**. The modules will be installed.

## Usage

1. **Folder Structure**
   - When you open the application in your editor, you should see a client server folder structure.
   ![Folder Structure](/assets/images/TE07.png)

2. **Running the Application**
   - Run `npm run start` from the root directory.
   - Your application should start up the backend and serve the client.
   - When you run the text editor application from your terminal, your JavaScript files have been bundled using webpack.
   - When you run webpack plugins, you should have a generated HTML file, service worker, and a manifest file.
   ![Running Application](/assets/images/TE02.png)
   ![Generated Files](/assets/images/TE08.png)

3. **Using Next-Gen JavaScript**
   - When you use next-gen JavaScript, the text editor still functions in the browser without errors.
   - When you open the text editor, you should see "Just Another Text Editor (J.A.T.E)."
   ![Text Editor](/assets/images/TE03.png)

4. **IndexedDB Functionality**
   - IndexedDB immediately creates a database storage.
   - When you enter content and click off of the DOM window, the content in the text editor is saved with IndexedDB.
   - When you reopen the text editor after closing it, the content is retrieved from IndexedDB.
   ![IndexedDB Functionality](/assets/images/TE05.png)

5. **Download as Icon**
   - When you click on the Install button, you download your web application as an icon on your desktop.
   ![Desktop Icon](/assets/images/TE04.png)

6. **Service Worker and Caching**
   - When you load your web application, you should have a registered service worker using workbox.
   - When you register a service worker, your static assets are precached upon loading, along with subsequent pages and static assets.
   ![Precached Assets](/assets/images/TE09.png)
   ![Precached Assets](/assets/images/TE10.png)

7. **Deploying to Heroku**
   - When you deploy to Heroku, you should have proper build scripts for a webpack application.
   ![Heroku Deployment](/assets/images/TE11.png)

## References

- The Unit Ahead: Progressive Web Applications (PWA)
- Module 19 Mini-Project: Deploy Contact Directory App on Heroku with Script
- Request-Response: The Full-Stack Blog: Heroku Deployment Guide

## License

This project is licensed under the terms of the MIT license.

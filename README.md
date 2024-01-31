# Photo Management App

This web application provides pages : gallery, upload, and detail  

## Upload Page

In the upload page, users can submit data to the server, including title, description, and an image file. The data is sent to the server using a POST request to the `/upload` route. The server utilizes the npm package multer to handle file uploads, defining local storage, and connecting to MongoDB. The title and description are saved directly, while the image is stored as a buffer in the MongoDB database.

## Gallery Page

The gallery page makes a GET request to the image route, retrieving all stored data and displaying it to the users. Each image is presented as a card. Clicking on any card triggers the creation of a dynamic page using the image's unique ID. This ID is passed to the backend using parameters, and the server returns the corresponding object with the matching ID. The detailed information is then displayed on the page.

## Detail Page

The detail page is dynamically generated based on the image's ID. By passing the ID through the backend, the application fetches the specific object from the database and presents detailed information, including title, description, and the associated image.

 

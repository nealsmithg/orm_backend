# orm_backend

## Description
This is the backend for a store database to store products with there catagories and tags for the product. It is made useing mysql and sequelize to perform the database searches.

## Table of Conternts
<ol>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#preview">preview</a></li>
</ol>
    
## Usage
To use this program you will have to download the program files from github to your local computer. The first thing you can do is input your local mysql information into the `.env` file located in the main folder. You will need to enter the local user and password for the machine you are on. You will also need to delete the `.example` from the end of the file name so the file will be recognized. From there you will need to install the appropriate npm packages as well as create and seed the database. In order to do this, start with opening a termenal in the orm_backend folder. You will need to run the command `npm i` to install all of the npm packages. Then you will need to get into mysql. In the same termenal run the command `mysql -u example -p` replaceing "example" with your local username. The termenal will the prompt you for the password for your local user. Once you enter this you will need to run the command `source db/schema.sql` to create the database this program uses. After that you can enter `quit` to get out of the mysql interface. Now to seed the database you will need to run `node seeds/index.js` or you can use your own data as long as it is formated for this database. I have included base api calls to interact with the database but you can always create or change the calls. Lastly you will need to run `node server.js` for the server to be active on your localhost. I have the port set to 3001 when local but this can be changed in the server.js file as needed. As well this is only for the use of backend information management with this database. You will need to create a frontend aplication to display the data.

## Preview
[Preview of database](https://drive.google.com/file/d/1OSYIlrMCkROfIt3KhShV9A5T5aKQiLSp/view)
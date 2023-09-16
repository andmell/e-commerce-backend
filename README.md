# E-commerce-backend
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
## Description
The purpose of this project was to test functionality of the Object Relational Mapping package "[Sequelize](https://sequelize.org/)", and utilize it while developing a [MySQL](https://www.mysql.com/) database for backend code, as one might find being used for a retail store. 

The code written is not deployed, and cannot be operated by simple means. A walkthrough of the code can be viewed on Youtube [here.](https://youtu.be/VYazgZfIqCE) An instructional guide on how to download and run this code will be featured in the installation section, if running this code on your own personal source-code editor. 

[![A link to a YouTube video showcasing how to use the code in this project.](https://img.youtube.com/vi/VYazgZfIqCE/0.jpg)](https://www.youtube.com/watch?v=VYazgZfIqCE)

For this project, I utilized [Visual Studio Code](https://code.visualstudio.com/) on a computer running Windows 10. 

This project has several dependencies that will render it functionless if not installed correctly. Those are:
- Dotenv at version 8.2.0
- Express at version 4.17.1
- MySQL2 at version 2.1.0
- Sequelize at version 5.21.7

Additionally, Node.js was used to seed the database and connect to the server. Insomnia was used to test pathways and functionality of the code as well. 

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation
Installation is NOT recommended for this code due to the number of dependencies and additional software needed to function correctly. The instructions will be provided regardless.

1. Ensure you have Node.js and MySQL installed on your computer.
2. Copy the code from this GitHub repository and clone it to your preferred destination.
3. Install the required node packages listed in the description.
4. Create a .env file, which will contain the following code:
```
DB_NAME='ecommerce_db'
DB_USER=''
DB_PASSWORD=''
```
Populate those fields with the appropriate credentials. The "user" field may be root or dev. The password field is your password that you use to sign into MySQL. 

5. Run the following MySQL Commands:
```
1. mysql -u [user] -p
2. [password]
3. SOURCE ./db/schema.sql;
```

6. Open an additional terminal instance and run node.js first on your /seeds folder, and then on your server.js file.

7. Using insomnia, test the various paths found in the /routes folder.

## Usage
Once properly installed, navigate through Insomnia to retrieve, post, update, and delete data from the seeded database. All necessary attributes needed to post new data to the database are provided within the code. Be sure to be using the correct path in order to navigate through the Insomnia interface. The example below is using a GET request on the path:
```
http://localhost:3001/api/categories
```
![An image of the Insomnia application. A request has been made to http://localhost:3001/api/categories, and the data received are various retail clothing items, such as hats and shirts, and their database metadata.](/assets/insomnia%20example.PNG)

Be sure to familiarize yourself with the respective paths to better navigate through the application.

## Credits
Jude Clark, a tutor found through Washington University's Web Developer Bootcamp Program, was instrumental in developing this code. 

This code was developed through Washington University's Web Development Bootcamp Program.

## License
This application is utilizing the MIT License. Please refer to the respective [GitHub repository](https://github.com/andmell/Company-Content-Management-System) for further information.




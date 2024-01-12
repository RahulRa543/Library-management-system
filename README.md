# Library Management System
This is a basic library management system. It uses node.js (express.js), ejs, html, css, javascript, cookie session and mongoDB.
## Features
### Users
1. Can create account, login, and see library catalog.
2. Can see their profile, change their name, see books issued to them.
3. They can borrow books by verifying OTP sent to their email registered with library account.

### Admins
1. Logged in administrators can create new accounts for other administrators.
2. Admins can see edit the book catalog i.e. add or remove books.
3. They can accept book return by students.
4. Change the 'about' content of the website.

# How to run this app
1. Clone the repository on your machine.
2. Move to directory named 'backend'.
3. Install dependecies. If you are having npm, run command 'npm install'
4. Run 'nodemon app' to start the server. Server would be started. You may need to change app.js file to remove ipaddress from function app.listen()
5. To be able to use featue of otp verification you would need to give this app access to your email account. Here I have used gmail if you also use gmail then in backend/routes/otp.js file replace 'process.env.gmail_password' with your gmail password generated by going to gmail-account -> Security -> How you sign in to Google -> App password.
Note: MongoDB needs to be installed on your machine.
6. To acces admin feature for the first time you need to create a new admin by removing condition that an existing admin should be logged in to do this.

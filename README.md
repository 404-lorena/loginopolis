# loginopolis
A secure API with login and register endpoints, using express and bcrypt

## Getting Started
### Goal
Create POST /register and POST /login that:
* Create a new user and hashed password in a database
* Compares a usernames plaintext password with the stored hashed version.


### Start app
- [ ] npm install
- [ ] npm run start-dev

### Run tests
- [ ] npm test

## Write the Handlers
### POST /register
- [ ] Create the route handler in express, so app.post(/*etc*/)
- [ ] Pull out the username and password from the req.body object.
- [ ] Hash the password with bcrypt.hash
- [ ] Call User.create (User is already imported above)
- [ ] Send back a success message (a string) per the test specs.


### POST /login
- [ ] Create the route handler in express, so app.post(/*etc*/)
- [ ] Pull out the username and password from the req.body object. (yep! Just like register)
- [ ] Call User.findOne to look up the user by username
- [ ] If a user is found, bcrypt.compare the db password with the password from the req.body. This returns a boolean (true if it’s a match, false if not)
- [ ] If the passwords match, send back a success message (a string) per the test specs.
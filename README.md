# Scheduling web application
#### `Short description:`

This app will allow users to register & login, access protected pages only accessible to logged in users, stay logged in when they close the app or refresh the page. On a scheduling(protected) page will be monthly calendar with functionalities(reminders and editable modals)

----

This project uses the following technologies:

- [React](https://reactjs.org) and [React Router](https://reacttraining.com/react-router/) for frontend
- [Express](http://expressjs.com/) and [Node](https://nodejs.org/en/) for the backend
- [MongoDB](https://www.mongodb.com/) for the database
- [Redux](https://redux.js.org/basics/usagewithreact) for state management between React components
# Procedure for running the project locally

## Configuration

Make sure to add your own `MONGOURI` from your [MongoDB](https://account.mongodb.com/account/login) database in `config/keys.js`.

```javascript
module.exports = {
  mongoURI: "YOUR_MONGO_URI_HERE",
  secretOrKey: "secret"
};
```
## Install & QuickStart
Afrer cloning repository folow this `steps:`
```
> cd Scheduling_Calendar
> npm install
> cd client
> npm install
> cd ..
> npm run dev
```
Running `npm run dev` from root folder will start both servers, http://localhost:5000/ for Express.js & http://localhost:3000/ for create-react-app.

### Tracking information
* Install the [React](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en) and [Redux Chrome Extensions](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en)
* Open inspector `Ctrl + Shift + i` & open `Redux`
* Track information about errors(for passwords,emails, unique usernames....etc) and current logged in user. 

### Script that run project
Using Fakefile, universal **Makefile** for JS proxies to your npm scripts. Install fakefile from `npm install --save --exact fakefile`



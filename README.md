# mern-template
Simple template for a project using the MERN stack.

The projects is comprised of a **backend** part consisting of `node.js`, `express` and `mongoDB` parts, and of a **frontend** part consisting of a `react` project created with the `create-react-app` tool.

It also has already sample models (`backend/models/`), api (`backend/routes/api/`) and components (`frontend/src/components/`) for managing books.

This template was created with the help of the tutorial by *[Nur Islam](https://blog.logrocket.com/mern-stack-tutorial/)*.

## Stack

- **M**ongoDB: A general purpose, document-based, distributed database built for modern application developers and for the cloud era.
- **E**xpress: A minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.
- **R**eact: A JavaScript library for building user interfaces
- **N**ode.js: A JavaScript runtime built on [Chrome's V8 JavaScript engine](https://v8.dev/).

## Dependencies

**Backend:**

- `express`
- `mongoose`
- `body-parser`
- `bcryptjs`
- `validation`
- `config`
- `cors`
- `nodemon` (DEV)

**Frontend**

- `react`
- `react-dom`
- `react-router-dom`
- `react-scripts`

- `axios`
- `web-vitals`

- `jest-dom` (Testing)
- `user-event` (Testing)
- `bootstrap` (CDN)
- `fontawesome` (CDN)

## Quickstart

### Connect MongoDB database

`backend/config/default.json`

```json
{
	"mongoURI":
  	"mongodb+srv://<userName>:<password>@<clusterUrl>/<defaultDatabaseName>?retryWrites=true&w=majority"
}
```

### Edit Project informations

`backend/package.json`

```json
{
  "name": "mern-template",
  "version": "1.0.0",
  "description": "template structure for a MERN stack project",
  "main": "app.js",
  "scripts": {
    "start": "node app.js",
    "app": "nodemon app.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/Beomar97/mern-template.git"
  },
  "author": "Marco Forster",
  "license": "MIT",
  "bugs": {
    "url": "https://github.com/Beomar97/mern-template/issues"
  },
  "homepage": "https://github.com/Beomar97/mern-template#readme",
  "dependencies": {
    "bcryptjs": "^2.4.3",
    "body-parser": "^1.19.0",
    "config": "^3.3.4",
    "cors": "^2.8.5",
    "express": "^4.17.1",
    "mongoose": "^5.11.15",
    "validation": "^0.0.1"
  },
  "devDependencies": {
    "nodemon": "^2.0.7"
  }
}
```

`frontend/package.json`

```json
{
  "name": "mern-template",
  "version": "0.1.0",
  "private": true,
  "dependencies": {
    "@testing-library/jest-dom": "^5.11.9",
    "@testing-library/react": "^11.2.5",
    "@testing-library/user-event": "^12.8.1",
    "axios": "^0.21.1",
    "react": "^17.0.1",
    "react-dom": "^17.0.1",
    "react-router-dom": "^5.2.0",
    "react-scripts": "4.0.3",
    "web-vitals": "^1.1.0"
  },
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
  "eslintConfig": {
    "extends": [
      "react-app",
      "react-app/jest"
    ]
  },
  "browserslist": {
    "production": [
      ">0.2%",
      "not dead",
      "not op_mini all"
    ],
    "development": [
      "last 1 chrome version",
      "last 1 firefox version",
      "last 1 safari version"
    ]
  }
}
```

### Run frontend and backend in separate Terminal windows

- In `backend/` run command `npm start`
- In `frontend/` run command `npm start`


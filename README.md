# heroku-H10_err-fix
snippet to fix deploy react app without server

run:
`npm install serve --s`
---
change scripts in package.json file:<br>
```json
 "scripts": {
 "dev": "react-scripts start",
 "start": "serve -s build",
 "build": "react-scripts build",
 "test": "react-scripts test --env=jsdom",
 "eject": "react-scripts eject",
 "heroku-postbuild": "npm run build"
}
```
---

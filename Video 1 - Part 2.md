## Video 1 - Part 2
[Video 1 - Part 2](http://www.youtube.com/watch?v=Fa4cRMaTDUI&t=17m41s)

## open a second NodeJS command prompt

```
cd C:\Users\Wouter\source\repos\tab-tracker
mkdir server
cd server
npm init -f
npm install --save nodemon eslint
node node_modules\eslint\bin\eslint.js --init
> Use a popular style guide
> Standard
> JavaScript
```

## edit package.json
```
...
"scripts": {
    "start": "node node_modules\\nodemon\\bin\\nodemon.js src\\app.js --exec \"npm run lint && node\"",
    "lint": "node node_modules\\eslint\\bin\\eslint.js **\\*.js"
  },
...
```

## Create src\app.js
```
console.log('hello')

```

## Run application
```
npm start
```

## Add to git
``` 
cd ..
copy client\.gitignore server\
git add -all
git commit -m "Added server (Part 2)"
git push
```
# tvOSAppServer
tvOS App Server test bed

This is a barebones Node.js app to serve up javascript & tvml for my tvOS testing.

Why heroku to test tvOS apps? Because you need an external host for the tvml and javascript pages. Heroku also provides HTTPS which as of iOS9, apps are prevented from linking to non-HTTPS servers to encourage best practices. Sure you can do this locally but this is a fast and free solution to get something up quick!

You can skip the non-HTTPS check by adding "Allow Arbitrary Loads" bool value to YES under App Transport Security Settings in Info.plist. 

## Running Locally

Make sure you have [Node.js](http://nodejs.org/) and the [Heroku Toolbelt](https://toolbelt.heroku.com/) installed.

```sh
git clone git@github.com:heroku/node-js-getting-started.git # or clone your own fork
cd node-js-getting-started
npm install
npm start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```
heroku create
git push heroku master
heroku open
```

## Documentation

For more information about using Node.js on Heroku, see these Dev Center articles:

- [10 Habits of a Happy Node Hacker](https://blog.heroku.com/archives/2014/3/11/node-habits)
- [Getting Started with Node.js on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- [Heroku Node.js Support](https://devcenter.heroku.com/articles/nodejs-support)
- [Node.js on Heroku](https://devcenter.heroku.com/categories/nodejs)
- [Using WebSockets on Heroku with Node.js](https://devcenter.heroku.com/articles/node-websockets)

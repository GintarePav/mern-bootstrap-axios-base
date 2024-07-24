# How I made this base

This base is created with the intention for the project to be deployed on _Render_ and _Vercel_.

## Part I

1. Inside a directory that's not pushed to git, ran _npx create-react-app app-name_; this is going to be the main directory.
1. Created the _client_ folder and moved everything there.
1. Ran the command _cd client npm i axios bootstrap bootstrap-icons react-router-dom_ to add all the needed dependencies.
1. Deleted defaulr React files that are not needed and created the _components_ folder inside _src_.
1. Inside _index.js_ imported Bootstrap styles and scripts.
1. Created _.env_ and included it in _.gitignore_; also craeted _example.env_ for reference.

## Part II

1. Created the _server_ folder inside the main directory.
1. Ran the commands _cd server_ and _npm init -y_.
1. Ran the command _npm i express dotenv mongoose nodemon bcryptjs jsonwebtoken validator cors_.
1. Created _.gitignore_ and included _node_modules_ inside it.
1. Created _config.env_ and included it inside _.gitignore_; also created _example.env_ for reference.
1. Created _index.js_ and _server.js_ files.
1. Inside _package.json_, added _"start": "nodemon server.js"_ under _scripts_.
1. Created the following folders: _models, controllers, routes, utils_.
1. Set up _index.js_ and _server.js_ and _utils_ following the guides below.

## Guides and Tutorials Used

1. _[Express](https://expressjs.com/en/5x/api.html)_ docs for creating an _express_ app.
1. _[.env](https://medium.com/@akhilanand.ak01/simplify-your-node-js-configuration-with-dotenv-env-ee371ad6bf9a)_ file creation guide.
1. _[Mongoose](https://mongoosejs.com/docs/connections.html)_ docs for connecting to the DB.
1. _[JWT](https://www.freecodecamp.org/news/how-to-secure-your-mern-stack-application/)_ (used for authentication and authorisation) creation totorial.
1. _[JWT](https://medium.com/@vkcivil62p/basics-of-jwt-and-how-to-decode-jwt-tokens-in-node-97c2975266e9)_ decoding tutorial.
1. _[JWT + localStorage](https://medium.com/@giwon.yi339/how-to-store-jwt-token-in-local-storage-for-react-b0957686b75c) setup; it's the quickest but not the safest and should not be used in actual production, as explained [here](https://medium.com/kanlanc/heres-why-storing-jwt-in-local-storage-is-a-great-mistake-df01dad90f9e).
1. _[Axios](https://dev.to/techcheck/creating-a-react-node-and-express-app-1ieg)_ setup for connecting BE to FE.
1. _[Deployment](https://medium.com/@yashpatel54257/how-to-deploy-a-mern-app-on-vercel-635683167e30)_ tutorial for deploying BE on Render and FE on Vercel.
1. _[Vercel's CORS](https://vercel.com/guides/how-to-enable-cors#enabling-cors-using-vercel.json) setup details needed for deployment.

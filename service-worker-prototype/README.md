## Service Worker Prototype

### Description
I wanted to learn more about service workers and how they could be implemented within a React app, so I created this project.


### Commands
I used [`create-react-app`](https://github.com/facebookincubator/create-react-app) to get this thing up and going quickly, so if you wanted to run this locally, you'll need to first install it using

`npm install -g create-react-app`

and then run one of the following commands (as output by `create-react-app`):

`npm start` -> Starts the development server.

`npm run build` -> Bundles the app into static files for production.

`npm test` -> Starts the test runner.


### Running the Production Build to test the Service Workers
I'm still in the process of learning how to test service workers within a development build, but
in the meantime, they currently work in the production build.  In order to run the production build
locally, you'll need a static server. `pushstate-server` is the one I'm currently using as it was recommended by `create-react-app`, and can be installed by running:

`npm install -g pushstate-server`

Once it's installed, run the following command to start running the server with the output of `npm run build`:

`pushstate-server build`

*Note*: By default this uses port 9000

You can then view the results at `localhost:9000`


### References
I used the following projects as references in building this:

* https://github.com/jeffposnick/create-react-pwa
* https://github.com/GoogleChrome/sw-precache
# This project is offline and deprecated with no plans for support in the future.

# spotifier.io

spotifier.io is a web application that aims to make tracking new releases on Spotify efficient, reliable, and effortless
for the user. It utilizes node.js and express for routing, mongodb for session storage and database management, redis
for running long processes in a queue, and angular for front-end.

## Getting Started

Getting started developing for spotifier.io is easy. First, `clone` the repository to your development directory of choice. Then run `npm install` to initialize the required node modules. 

You will need to setup a file called `config-private.js` and the directory `./private/` which you create. Use the template `config-private-template.js` in the root folder to easily input your variables.

Follow the directions in the config template to get setup.

You will also need to run your own local mongo and redis servers for the application to run properly. 

#### To setup mongo/redis check out the following links:

[mongodb](https://www.mongodb.com/download-center#community)

*note:* we are running our db on the `spotifier` instance. Run `use spotifier` in your mongo cli to switch and be able
to manage collections.


[redis](https://redis.io/download)


## Running the tests

Unit tests are written with `chai`, `sinon`, and `mocha`. They are found in the `./tests/` directory and can be run
from the command line with `mocha <test-file-name>.js`


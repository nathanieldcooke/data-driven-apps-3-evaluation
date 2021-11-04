    "start": "nodemon ./bin/www",
    "start:development": "nodemon -r dotenv/config ./bin/www",
    "start:production": "node ./bin/www"

    the code above, always runs the first script, but does not load the .env variables
    to some capacity.
    If I make the PORT be 3000 in the .env, it'll load the default 8080, becuase the 
    dotenv command does not load the port variable, unless added to the "start" command.

    
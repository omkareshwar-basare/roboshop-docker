FROM mongo:7.0
COPY *.js /docker-entrypoint-initdb.d/


# When we start the container then the MongoDB will be initialized with the JavaScript files 
# which are copied to the /docker-entrypoint-initdb.d/ directory.
# The JavaScript files will be executed in the order they are copied to the /docker-entrypoint-initdb.d/ directory.
# For example, if we have two JavaScript files named init.js and data.js then the init.js file will be executed first 
# and then the data.js file will be executed.
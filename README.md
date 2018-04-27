# spring-cloud-config-sample
Sample usage of spring cloud config with a server and client setup

# Confirm Changes in Config Files
Visit http://localhost:8888/sample-config-client/default

# To test
Run the config server
Run the config client

Check http://localhost:8888/sample-config-client/default for the property config values
Run a test to http://localhost:8080/message to see the value

Change sample-config-client.properties, change the message key or anything appropriate, commit and push to repository
Check http://localhost:8888/sample-config-client/default again to see that the new value has reflected

Run a post to http://localhost:8080/actuator/refresh of the client to refresh and load the new config
Run a test to http://localhost:8080/message to see the new value
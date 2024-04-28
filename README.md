# Run ELK in docker and test with nginx logs
This environment was created to play and understand elk. To have some logs to play with, I am using the nginx access/error logs.

## Download the repository and setup the docker environment
Clone the repository
```
git clone https://github.com/gnzdotmx/elk-docker-container.git
```

Run docker compose to setup the environment
```
$ docker compose up
```

## Create the data view
If no errors
1) Go to Nginx to generate some access logs `http://localhost:9999/`
2) Go to kibana `http://localhost:5601/`. 
2) Navigate to Home->Analytics->Discover.
3) As your source should already be detected (nginx), create the data view
    - Type a name, for example, filebeat-test-view
    - Type an index pattern, for example, filebeat-test*

Keep adding views, dashboards, etc to keep learning :)
# Grafana
Data visualization &amp; Monitoring tool Grafana in depth

#Push dashboard to grafana#
curl -X POST <ip>:3000/api/dashboards/db -s -d @./grafanadashboard.json --header "Authorization: Bearer eyJrIjoiUXRFZlBPbU53NGw3YVlKQnJrUlp5eG1kYkkyaElBbmUiLCJuIjoidGVzdCIsImlkIjoxfQ=="  --header 'cache-control: no-cache' --header 'content-type: application/json' --write-out %{http_code}


#Delete grafana dashboard #
curl -X DELETE -H "Authorization: Bearer ${grafanaApiKey}" http://<ip>:3000/api/dashboards/db/${pipelinename}-monitor

curl -X POST 9.109.190.137:3000/api/dashboards/db -s -d @./alokTest3.json --header "Authorization: Bearer eyJrIjoiUXRFZlBPbU53NGw3YVlKQnJrUlp5eG1kYkkyaElBbmUiLCJuIjoidGVzdCIsImlkIjoxfQ=="  --header 'cache-control: no-cache' --header 'content-type: application/json' --write-out %{http_code}



# Grafana  API key 
    How to create
    From UI - setting 
    curl -H "Authorization: Bearer eyJrIjoiN...ImlkIjoxfQ==" http://<ip>:3000/api/dashboards/home

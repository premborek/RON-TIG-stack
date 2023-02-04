# TIG (Telegraf / InfluxDB / Grafana) Stack For Monitoring RON Link

Sample TIG stack collecting telemetry data from Cisco routers equipped with ZR/ZRP 400G transceivers. 

![image](https://user-images.githubusercontent.com/118137428/216769416-63d638ca-523e-4b51-a770-ef9dc5fa49b8.png)

Telemetry is based on gNMI protocol and native Yang models.

## Installation:
  1. Clone repo
  2. Update`.env` file:
     * Docker IP address to match your host IP
     * Grafana Admin password (if needed, default is **changemeplease**)
     * Aplication ports if needed
     * Routers IP and credentials
  3. Run `docker-compose up -d`
  4. Updata Grafana dashboard with correct router names (on To Do list to get it done automatically:))
     * Go to dashboard properties
     ![g1](https://user-images.githubusercontent.com/118137428/201667010-78e5c060-0e6c-4dee-8145-283b7558f866.jpg)
     * Update regex expression for `host1` and `host2` variables
     ![g2](https://user-images.githubusercontent.com/118137428/201667321-540e69f9-7825-4dd4-8ea7-98f9daea5eb2.jpg)
     * Other variables depend on them thus no need to update them too.
     
   5. Select interfaces from the dashboard
   
   ![g3](https://user-images.githubusercontent.com/118137428/201668056-6808346b-3122-496e-ac8c-c4250268e249.jpg)





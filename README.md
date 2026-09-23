# assignment2 
## Link to main.cpp and README.md on github below
https://github.com/juanrsanchez2/assignment2/blob/403566e3b00ba9f85e79b3c923c359d4745bb053/main
https://github.com/juanrsanchez2/assignment2/blob/403566e3b00ba9f85e79b3c923c359d4745bb053/README.md

## Mirror Server Simulation
The purpose of this program is to simulate a system with 5 servers. The simulation tracks of when a server is online(UP) and fails(DOWN) and how long it takes to restore it. The simulation will continue to run as long as one server is still online. Simulation will end when all servers are down at the same time. A total of 5 simulations runs will be performed.

### Server Fails and Restore
Each server is given a random failure rate. The failure rates are generated using a <ins>**Poisson Event Model**</ins>. When a server fails, its state will change from <ins>**UP** to **DOWN**</ins>. A server requires 2 hours to be restored. If all servers are DOWN at the same time, the current simulation run ends.

### Simulation Output
The program will display the state of all the servers during each simulation run. Server states are displayed as either <ins>**UP** or **DOWN**</ins>. The time of the state change is on the left and displayed in hours. A display show the average statistics <ins>**Avg Uptime, Avg Downtime, Availability, MTBF**</ins> for each server across the 5 simulation runs.

### How Statistics are obtain
Average Uptime is calculated by getting the total uptime for a server across all the SIM runs and then dividing it by the number of SIM runs.
- **Average Uptime = total uptime / SIM runs**<br>

Average Downtime is calculated by getting the total downtime for a server across all the SIM runs andthen dividing it by the number of SIM runs.
- **Average Downtime = total downtime / SIM runs**<br>

Availability represents the percentage of time that the server was up in regard to its total operating time 
- **Availability = average uptime / (average downtime + average uptime)**<br>

Mean Time Between Failures represents the average total operation time between server failures across all 5 SIM runs
- **Mean Time Between Failures (MTBF) = total uptime / total number of failures**

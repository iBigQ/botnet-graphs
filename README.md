# P2P-based Botnet Graphs
This repository contains P2P overlay snaphots of the botnets Sality and ZeroAccess. The data was collected with our monitoring tool *Strobo-Crawler* and the overlay graphs have been reconstructed with *advanced reconstruction* methods.

If you want to get more details about how these graphs have been created or if you use these graphs, please **refer to our paper [1]**.

```
[1] S. Haas, S. Karuppayah, S. Manickam, M. Mühlhäuser, M. Fischer. On the Resilience of P2P-based Botnet Graphs. IEEE Conference on Communications and Network Security (IEEE CNS), 2016
```

# Repository Structure
We publish snapshots in two different categories. Individual snapshots can be found under **Individual Snapshots** and usually describe a certain situation. In addition we provide series of snapshots in fixed intervals.
Currently we have data for two P2P botnets: Sality and ZeroAccess.
## Graph Structure
Graphs in this repository are provided as compressed GraphML files. IP addresses are anonymized and cannot be grouped into subnets. However, hased IP addresses are consitnet in all graphs.

**File Naming Convention:**  
Core: Only nodes/bots that have unfiltered internet access, i.e., superpeers  
All: Core + nodes/bots with restricted internet access, i.e., non-superpeers (e.g. NATed or behind firewall)

## Individual Snaphots
Snapshot Name | Time | Description
-------------------|--------|-----------------
sality_v3_core_max | 2016-02-25 18:38:29 | Sality_V3 Core: Highest population
sality_v3_core_min | 2016-02-24 03:34:02 | Sality_V3 Core: Lowest population
za_16464_core_max | 2016-02-24 17:17:23 | ZeroAccess_16464 Core: Highest population
za_16464_core_min | 2016-02-23 04:19:30 | ZeroAccess_16464 Core: Lowest population
za_16464_all_max | 2016-02-24 13:52:11 | ZeroAccess_16464 All: Highest population
za_16464_all_min | 2016-02-28 04:25:44 | ZeroAccess_16464 All: Lowest population
 
## Snapshot Series
Series Name | From | To | Interval
------------------|---------|-----|------------
 sality_v3_core_15x12h | 2016-02-13 00:00:00 | 2016-02-20 00:00:00 | 12 hours
 sality_v3_core_25x1h | 2016-02-24 00:00:00 | 2016-02-25 00:00:00 | 1 hour

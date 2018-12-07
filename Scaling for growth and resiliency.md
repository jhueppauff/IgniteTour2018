# Scaling for growth and resiliency

- Resource exhaustion under load 
- application ceases to meet its objective
- aticipated/unanticipated load (spikes are tricky)

## Scaling types

- scaling up (vertical)
  - box is not big enough to serve
  - default way for eg. sql
- scaling out (horizontal)
  - makes more sense for web apps

## Autoscale App Service

- Scale out based on conditions
  - scale based on metric or instance count
    - eg. cpu higher than 80% on one instance

## scaling for resilency

- regions pairs
  - aka.ms/region-pairs
- horizontal architecture
- active/active or active/passive
- data consistency
- race conditions (which user wins when changing a entry)
- data sovereignty

## Azure Front Door

- Global HTTP Load Balancer

- SSL Offload close to the user
- application firewall and DDoS protection
- central control pane for traffic orchestration

## Cosmos DB

- Global Scaling/Replicating

## Others

- CDNs
- Failovers testing
- Traffic Shaping
- Draining load to Datacenters
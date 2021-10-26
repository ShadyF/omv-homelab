<div align="center">
<br/>
<img src="https://user-images.githubusercontent.com/6564442/119241148-b009a080-bb54-11eb-8786-293265711f5c.png" align="center" width="144px" height="144px"/>

### My openmediavault home server :computer:

</div>

## :book:&nbsp; Overview

This repository contains various `docker-compose` files for applications that I ran on a spare computer that I had.

This repo is mainly for archival and historical purposes as I have moved everything into a kubernetes cluster,
maintained in [this repo](https://github.com/ShadyF/k8s-homelab)

## :computer:&nbsp; Infrastructure

[openmediavault](https://www.openmediavault.org/) installed on a spare computer I had

| Component    | Details |
|--------|---------------------------------------------|
| CPU    | Intel Core i5-2500K (Overclocked to **4.5GHz**) |
| Cooler | Cooler Master Hyper 212 EVO                 |
| RAM    | 8GB DDR3                                    |
| GPU    | AMD Radeon HD 6950                          |
| PSU    | Antec 650W                                  |

## :straight_ruler:&nbsp; Random Tips and Tricks

#### Network mode

You can make a docker container use another docker container's network using the `network_mode` keyword

Can be used in one of the following ways:

```yaml
# container keyword can be used to use the network of any container
network_mode: container:container_name

# service keyword can be used to select services in the same docker-compose file
network_mode: service:service_name
```

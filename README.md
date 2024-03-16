# baisc_applicaton_load_balancer
This is a basic application load balancer guide

### Create a VPC

![create vpc.png](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/create%20vpc.png)

### Create Subnets

![create subnet.png](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/create%20subnet.png)

### Make route table

![route table.png](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/route%20table.png)

### VPC table

![resource map.png](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/resource%20map.png)

## Create security groups

One for load balancer

![lb security group.png](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/lb%20security%20group.png)

Other for the instances

![instance security group.png](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/instance%20security%20group.png)

http and https is only enabled from load balancer security group

### Create instances

![instances.png](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/instances.png)

### Create Target groups

- Create two target groups with /search and /mail

### Create load balancer

- Add listener as port 80 (choose either of target groups)
- then add rules and select path, then add /search and /mail in the rules separately

### Then well search for our load balancer

[16.03.2024_15.41.15_REC.mp4](https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/blob/c344842fec941a0162189c7c829e93a474d27fb8/16.03.2024_15.41.15_REC.mp4)


https://github.com/Siddhant00Tiwari/baisc_applicaton_load_balancer/assets/110492372/8c98d1e1-7f4a-49f6-8577-671ccfb7237a


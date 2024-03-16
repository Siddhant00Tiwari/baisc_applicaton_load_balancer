# baisc_applicaton_load_balancer
This is a basic application load balancer guide

### Create a VPC

![create vpc.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/fdb6e856-ec13-4022-a20f-cd333ff5473b/create_vpc.png)

### Create Subnets

![create subnet.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/d43b9f45-6d53-4d45-8cc3-76f036363c4f/create_subnet.png)

### Make route table

![route table.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/bb58d3d8-d183-41b8-a690-5a98d2451d11/route_table.png)

### VPC table

![resource map.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/b1d6a55c-54fc-45ea-a40c-28260a4b891d/resource_map.png)

## Create security groups

One for load balancer

![lb security group.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/a315fc76-35d5-46bd-824f-eddce45421b4/lb_security_group.png)

Other for the instances

![instance security group.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/a5f896a8-1a8e-40d9-a211-01b6b0e0099a/instance_security_group.png)

http and https is only enabled from load balancer security group

### Create instances

![instances.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/ca15fc84-1eba-4184-a4c7-2f0305c0a9f2/instances.png)

### Create Target groups

- Create two target groups with /search and /mail

### Create load balancer

- Add listener as port 80 (choose either of target groups)
- then add rules and select path, then add /search and /mail in the rules separately

### Then well search for our load balancer

[16.03.2024_15.41.15_REC.mp4](https://prod-files-secure.s3.us-west-2.amazonaws.com/77ead240-a866-4aa1-883b-179fa59f3972/f7672619-522e-43f8-a614-240f73d3934b/16.03.2024_15.41.15_REC.mp4)

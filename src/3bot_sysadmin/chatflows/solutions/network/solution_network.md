# Network solution

This package is used to deploy a network on the grid and to connect your solutions together.

## Accessing the solution

Go to your admin dashboard `https://localhost/admin` and click on Network

![solutions menu](adminmenu.png)


## Inputs

The solution takes some configurations from the user, we will list them and explain their meaning
- `Network name` : a name for the network to deploy on and also to reference in the reservation manager.
- `Payment currency`: a currency that will be used for the payment
- `Expiration time`: a network expiration time (minutes=m ,hour=h, day=d, week=w, month=M) is how long you want that solution to live on the grid
- `IP version` : (IPv4 or IPv6) Version of the entrypoint node.
- `IP range` : Configure network manually by choosing an IP range to use or the deployer could choose for you and generate an IP range automatically



## User setup

- register user 3Bot on explorer `kosmos "j.tools.3Bot.init_my_3Bot(name=3Bot_NAME,email=EMAIL)"` **Note**: name of 3Bot is (your 3Bot name).3Bot , email is your 3Bot email
- Install [wireguard](https://www.wireguard.com/install/)


## Chatflow steps:

### Choosing the network name

![Step1](./img/network1.png)
We choose the network name to be referenced again in the dashboard reservation manager

### Payment currency
![Step2](./img/network2.png)
Choosing a currency that will be used for the payment

### Expiration time
![Step3](./img/network3.png)
Choosing the expiration time for the network on the grid

### Choosing how to reach the entry point node
![Step4](./img/network4.png)

To reach your solution on the grid you could use IP v6, problem is some countries don't have that infrastructure so we provide them access with an IP v4 entry point.

### The network IP Range
![Step5](./img/network5.png)

We decide the IP range the network and all of the other solutions connected on it will operate on

### Wireguard install
![Step6](./img/network6.png)
Just ask you to make sure you have Wireguard installed

### Wireguard configurations
![Step7](./img/network7.png)
While the grid is built around IP v6 you need you to connected to the network, and that's done using wireguard.

### Configuring your machine
![Step8](./img/network8.png)
Now you need to configure your machine to access the network by applying the wireguard configurations
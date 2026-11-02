Build a lab with a router

In this lab we are building onto our previous network with an addition to a router as well.

The key aspect is to identify, the use of the router, whether the connection has been established, the reason for a default gate way , loopback integration and any troubleshooting we might run into.

## <u>Diagram Topology</u>

![A screenshot of a Cisco Packet Tracer network topology](Pasted%20image%20261102163814.png)




### <U>Router </u>

The first step was to go within the CLI of the router. Verified the IP interface brief within the router and we could see the physical interfaces of the router.

By default the interfaces of the router is shut down so we enabled it first.
    - **In this case it is Gig0/0/0 (no shut)**

The interface state has now changed to up and the Fa0/1 interface still loading, this is due to spanning Tree protocol determining whether there are no loops.

The next step was to put an **IP address on the interface**, so in this case we used the IP address **192.168.1.254  255.255.255.0**

![[Pasted image 20261102164735.png]]


### <u>Pinging the Switches in our topology</u> 

To verify whether we can ping the switches from the Router, used the command ping and got the following results.

![[Pasted image 20261102165120.png]]


## <u>Configuring a Default Gateway </U>

The next step we want to do is configure a Default gateway.

For all your device essentially what you are instructing them to do is if you don't know where to go send it to the **router.**


### <u>Configuring Default Gateway for PC1</U>

![[Pasted image 20261102190442.png|611]]


## <u>Configuring Default Gateway for PC2</U>

![[Pasted image 20261102191050.png|581]]

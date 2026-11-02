Build a lab with a router

In this lab we are building onto our previous network with an addition to a router as well.

The key aspect is to identify, the use of the router, whether the connection has been established, the reason for a default gate way , loopback integration and any troubleshooting we might run into.

## <u>Diagram Topology</u>


<img width="1018" height="427" alt="image" src="https://github.com/user-attachments/assets/83f798da-1820-4ce3-a64d-9ee1af7fa8e1" />





### <U>Router </u>

The first step was to go within the CLI of the router. Verified the IP interface brief within the router and we could see the physical interfaces of the router.

By default the interfaces of the router is shut down so we enabled it first.
    - **In this case it is Gig0/0/0 (no shut)**

The interface state has now changed to up and the Fa0/1 interface still loading, this is due to spanning Tree protocol determining whether there are no loops.

The next step was to put an **IP address on the interface**, so in this case we used the IP address **192.168.1.254  255.255.255.0**


<img width="750" height="87" alt="image" src="https://github.com/user-attachments/assets/3daa3e3c-440e-4e72-a2d2-8bd86880b391" />




### <u>Pinging the Switches in our topology</u> 

To verify whether we can ping the switches from the Router, used the command ping and got the following results.

<img width="600" height="180" alt="image" src="https://github.com/user-attachments/assets/de2c5b76-b790-468f-bd49-d2d38b19b725" />



## <u>Configuring a Default Gateway </U>

The next step we want to do is configure a Default gateway.

For all your device essentially what you are instructing them to do is if you don't know where to go send it to the **router.**


### <u>Configuring Default Gateway for PC1</U>

<img width="500" height="160" alt="image" src="https://github.com/user-attachments/assets/00b160d0-23c8-48bd-90ca-aecce981b196" />



## <u>Configuring Default Gateway for PC2</U>

<img width="500" height="160" alt="image" src="https://github.com/user-attachments/assets/7e11f013-e9d9-4d0c-ac64-d1210447b4aa" />


# Source Route Bridging

A Bridge is deemed to connect 2 different LAN segment


        
                  LAN   -------MAC     Bridge     MAC --------   LAN
        
        
 
 ![bridge](https://s3.notfalse.net/wp-content/uploads/2018/05/15023113/bridge-demo.png)

Source-Route Bridging is designed for interconnecting token ring segments into a bigger LAN.

Originally, Source-Route Bridging was deemed as a universal method for creating large-scale networks. However in actual world, source-route can not meet client's requirement.

# Premises of Source-Route Bridging to be based upon 

Non-Transparent

* The headers of token ring frames that must travers source-route bridge (the frame contains routing information that is used by the bridges to forward the frame thru source-route bridged LAN from src to des), the routing info describes precisely which bridges and segments the frame must traverse to arrive at the des.

* The Source Node is responsible for inserting the routing information into the headers of the token ring frames that must be delivered thru Source-Rout Bridge.

* Source-Route Bridge requires each node to be able to discover and memorize routing information to DES accessible thru Source-Route Bridge.

# Config of Source-Route

- [x] Each Ring shall be assigned a unique number.

- [x] Each bridge shall be assigned a unique number with each ring to which the bridge is connected.

# Likelyhood between Source-Route & Transparent-Route

Like a transparently bridged LAN, source-route allows redundant paths to exist with a single source-route bridged route LAN. This redundant path helps to be utilized to recover from network component failure.

# Multiple Source-Route Bridge

As designed spec, the source-route bridging got only 2 ports, in order to be bypassed this weired obstacle, can require a significant amount of additional equipment.

A neat solution was devised, it allows multiport source-route bridges to be created, so an abstraction called 'virtual ring'. The operation of such a bridge counts that virtual ring as a regular ring and inserts an extra route designator into all routes and spanning explorers crossing the bridge.

# Alternative to pure source-route Bridging

* DLSw, Data Link SW

![sw](https://www.tp-link.com/resources/images/faq/2008923175652769.jpg)

* RSRB





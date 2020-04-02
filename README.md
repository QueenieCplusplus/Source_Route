# Source Route Bridging

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




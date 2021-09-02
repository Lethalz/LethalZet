# IGP and EGP

## IGP

IGP or *Interior Gateway Protocol*  is one of the two AS or Autonomous Systems that exist within dynamic routing.

IGP is commonly used only in a **Intranet** setting and is not intended for use outside ones on LAN. 

## Common IGP protocols

* Ipv4 Dynamic Routing
    * Ospfv2 (Open Shortest Path First) (link-state)
    * Ripv2 (Routing Information Protocol version 2) (Distance vector)
    * EIGRP ( Cisco Proprietary System) (Distance vector)
 
* IPv6 Dynamic routing 
    * OSPFv3
    * EIGRP for v6
    * RIPng (next gen)
 
 
----

## EGP

EGP or Exterior Gateway protocol is used outside of our local AS to speak between external AS (autonomous systems) while it leverages IGP at its target AS to handle local routing.

**BGP** (Border Gateway Protocol) is the standard for EGP (Hybrid depending on configuration)

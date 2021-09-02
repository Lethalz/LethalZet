# Static and Dynamic Routing

In **Static routing** an admin designates the routes for a router so you are in *full control* of the routing in your network.

Static works well in smaller networks because of.. well the fact that there is one way in and one way out. It also conpletely removes overhead from routing protocols that normally take up CPU , MEM , BANDWITH.

However it does not do very well in larger networks because there are more points of failure which as the network expands becomes increasingly difficult to administrate all of those different nodes.

If there is an unfourtunate outage there is no automatic response unlike **Dynamic routing**.

------
In **Dynamic Routing** and admin only has to configure the settings once and the routers send routes to other routers in almost real-time.

For larger networks this method becomes less of a hassel for any potential netowrk administrators because it makes the routing aspect of the network more Autonomous and prone to scalabilty. 

Default routes are when there are no other routes for the router to route to which is normally the default gateway or as some call it the gateway of last resort.
This can dramtically decrease the routing process.

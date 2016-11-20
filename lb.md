# LB
Load balancing refers to efficiently distributing incoming network traffic across a group of backend servers, also known as a server farm or server pool.

### Listeners:
A listener is a process that checks for connection requests. It is configured with a protocol and a port for front-end (client to load balancer) connections and a protocol and a port for back-end (load balancer to instance) connections.
**Ex.**
http 80 http 8080

### LB method
There are numerous techniques and algorithms that can be used to intelligently load balance client access requests across server pools. We provide two methods

```
Round Robin
Least Connection
```

### persistent
It defines the persistent, persistent means Information about a user’s session is often stored locally in the browser.

### Create cloud vips
It defines whether you want VIP or not. A VIP is the public IP address associated with a VM.

### LB Custom Attrs
Here we can add load balancer attributes.

### Required availability zone
It is used to horizontally scale physical load balancer devices.

### ECV:
This value is used in servicer monitoring

### Servicegroup Custom Attrs:

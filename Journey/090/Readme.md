
# Route 53 routing policy, Health check, 3rd party domain registrar ( An SAA Course by Stephane Maarek on Udemy)

## Cloud Research

### Route 53 routing policy

Simple routing policy – Use for a single resource that performs a given function for your domain, for example, a web server that serves content for the example.com website. You can use simple routing to create records in a private hosted zone.

Failover routing policy – Use when you want to configure active-passive failover. You can use failover routing to create records in a private hosted zone.

Geolocation routing policy – Use when you want to route traffic based on the location of your users. You can use geolocation routing to create records in a private hosted zone.

Geoproximity routing policy – Use when you want to route traffic based on the location of your resources and, optionally, shift traffic from resources in one location to resources in another.

Latency routing policy – Use when you have resources in multiple AWS Regions and you want to route traffic to the region that provides the best latency. You can use latency routing to create records in a private hosted zone.

IP-based routing policy – Use when you want to route traffic based on the location of your users, and have the IP addresses that the traffic originates from.

Multivalue answer routing policy – Use when you want Route 53 to respond to DNS queries with up to eight healthy records selected at random. You can use multivalue answer routing to create records in a private hosted zone.

Weighted routing policy – Use to route traffic to multiple resources in proportions that you specify. You can use weighted routing to create records in a private hosted zone.

### Health Check

Amazon Route 53 health checks monitor the health and performance of your web applications, web servers, and other resources. Each health check that you create can monitor one of the following:

The health of a specified resource, such as a web server.

The status of other health checks.

The status of an Amazon CloudWatch alarm.

Additionally, with Amazon Route 53 Application Recovery Controller, you can set up routing control health checks with DNS failover records to manage traffic failover for your application.

More info : https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover.html

### 3rd Party Domain Registrar



## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1549422634453966848)

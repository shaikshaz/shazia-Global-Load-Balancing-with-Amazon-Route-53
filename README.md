# shazia-Global-Load-Balancing-with-Amazon-Route-53
Task :Global server load balancing is also sometimes called global load balancing (GLB).Route 53 is a Domain Name System (DNS) service that performs global server load balancing by routing each request to the AWS region closest to the requester's location.
1. create an ec-2 instance and create an HTML web server application and run it on the web server and see if it is working or not
2.create a load balancer Ex: ALB to that ec2 server application, select all the subnets give internet facing.
4. create a new security group give inbound rules and outbound rules like HTTP.
5. in listener and routing for the application load balancer create a target group and create Load balancer.
6. In the ALB do a health check test for webserver
7. In route 53 register domain name if the test passes using DNS name, check the web server again if it is properly running
shaziawebserver-test-1363749700.eu-west-2.elb.amazonaws.com
ns-324.awsdns-40.com.
ns-1720.awsdns-23.co.uk.
ns-569.awsdns-07.net.
ns-1382.awsdns-44.org.
8. Create health check for monitoring the health status of the instance 
8. create a latency-based routing in record set for the ec2 Instance depending upon the nearby region of the user for low latency
9. create a geographical latency routing depending upon the location of the user regardless of region.
10. create cloud watch alarm using create metrics and select Ec2 ALB created
11. create metrics by adding conditions like statics, period, threshold type, value and CPU utilization then then select notification options like alarm trigger, SNS.
12.Create topic name n mail ID, confirm subscription, and give a name and now create an alarm.

![Screenshot (43)](https://github.com/shaikshaz/shazia-Global-Load-Balancing-with-Amazon-Route-53/assets/154241222/cb94ee6f-3a02-4ab4-8071-12f1b917e0c5)



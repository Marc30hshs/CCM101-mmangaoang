# Mission Reflection

In this laboratory activity, I learned that server security is an important part of cloud computing. A server may work properly, but without proper security configurations, it can still be vulnerable to unauthorized access and attacks.

A host-based firewall protects a server by controlling incoming and outgoing network traffic directly on the machine. Even if the network perimeter is breached, the firewall can still block connections that are not allowed by its rules. This provides an additional layer of protection and supports the principle of defense in depth.

Managing open network ports is also important because every unnecessary open port can provide another possible entry point for attackers. By allowing only the services required by the application, administrators can reduce the server's attack surface. In this activity, I allowed SSH for administration and TCP port 8080 for the web application.

In a real enterprise environment, leaving a database port such as MySQL port 3306 open to the public internet is dangerous. Attackers could attempt to exploit vulnerabilities, guess passwords, or gain unauthorized access to sensitive information. Database access should normally be restricted to trusted application servers and authorized administrators.

This mission changed my perspective on how easily a server can become vulnerable when security settings are ignored. I realized that deploying an application is not enough; administrators must also configure firewall rules, minimize unnecessary access, and regularly review security settings. I also learned why SSH must be allowed before enabling the firewall on a remotely managed server.

Finally, completing eight cloud computing missions has helped improve my technical knowledge and confidence. My GitHub portfolio now contains more practical documentation covering cloud infrastructure, storage, deployment, monitoring, and security. These activities helped me practice Linux commands, Docker, troubleshooting, and technical documentation. Overall, I understand better how Cloud Security Engineers protect servers and why security must be maintained continuously rather than configured only once.



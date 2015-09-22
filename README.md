# ppe_readiness
partner_readiness_content_FY16
This demonstration explores the benefits for several Microsoft Azure SQL Database features in the context of a software-as-a-service (SaaS) provider, Wingtip Tickets, which provides ticketing software to artists and groups. This demonstration centers on the tenant Julie and the Plantes (a fictitious pop-music tenant).

Other tenants that will be discussed in future labs include the following:
•	The Archie Boyle Band (a fictitious rock-music tenant)
•	Walla Walla Symphony (a fictitious classical-music tenant)

Demo Story Elements
Scenario 0: Purchasing a Ticket
Show the Wingtip Tickets website and discuss the core concept and existing database challenges with the audience to set the scene.
Scenario 1: Vertical Scaling
Discuss how the website is anticipating a big-name artist and how that might require some increased capacity. Simulate some load using the load generator, and then show the spike in resource utilization. From the portal, show how easy it is to scale up by changing the size of an instance (for example, from S3 to P1) and how quickly the change is implemented. Re-run the load generator and show how the increased capacity has significantly improved the site’s ability to handle a spike in ticket sales.
Scenario 2: Azure SQL Database Elastic Database Pools
Discuss how scaling up individual databases might not be the most efficient means of dealing with spikes in usage, particularly where the exact demands of individual databases are not known and hundreds or even thousands of databases might be in play (such as for software-as-a-service [SaaS] providers). From the portal, show how easy it is to set up elastic database pools. Re-run the load generator to produce a spike in demand and show how easily the pool meets the increased demand.
Scenario 3: Auditing
Discuss how auditing can be used to keep track of infrastructure changes made to the environment in addition to database-related issues (such as failed logon attempts). In the portal, show the operation to enable and set up auditing for a specific database. Discuss how we’re going to simulate a scenario to highlight the benefits of auditing by deleting one of the concert events, which will effectively delete all events associated with that concert. Then discuss that by using the auditing dashboard in a Microsoft Excel template, we will show how we can drill down into the auditing events by showing who deleted the event and at what time.
Scenario 4: Point-in-Time Restore
Discuss how point-in-time restore can be used to restore the missing concert event. In the portal, show how easy it is to restore a database to a point in time. From the website, show how the deleted concert event is restored, along with previously purchased tickets.
Scenario 5: Geographic Disaster Recovery
Discuss how point-in-time restore is great for “oops” scenarios, but what about broader server/datacenter failures? Discuss Azure SQL Database active geographic replication. In the portal, show how easy it is to set up a geo-replicated secondary, and view the status via an interactive map. Next discuss how Traffic Manager can be used to detect a failed website and redirect traffic to a hot standby in another datacenter.
Scenario 6: Azure Search
Discuss how Azure Search enables users to search for matching terms across multiple databases or database tables. Discuss how you will walk through the search experience from the user’s point of view.
Conclusion/Summary

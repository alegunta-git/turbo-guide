## OOAD
* Design an ATM 
* Design Blackjack and a Deck of Cards 
* Design a Library Management System 
* Design a Hotel Management System 
* Design a Restaurant Management system 
* Design a Parking Lot 
* Design Chess 
* Design a Movie Ticket Booking System 
* Design an Airline Management System 
* Design an Online Stock Brokerage System 
* Design a Car Rental System 
* Design LinkedIn 
* Design Cricinfo 
* Design Stack Overflow 
* Design Amazon - Online Shopping System 
* Design Facebook - a social network



## Qs System Design
**Steps on Tackling a System Design Interview**
* Ask as many questions as possible to get a clear understanding of the requirements.
* Write them down the main use cases on the whiteboard.
* Ask re-clarifying and scope related questions.
* Once you have reqs written down draw up a flow diagram with various components and how they are connected and talk about the possible use cases.
* Think out loud. Verify your assumptions with the interviewer.
* Be prepared to write up the APIs specs for the flows and split the applications down by features.
* Also, you would need to have a fair understanding of various types of databases. When do you use RDBMS vs NoSQL? 
* When do you use a message queue? Which type of queue would you use?
* Detailing what kind of cache you would use and where.
* Talk about scaling, Redundancy, DR.

**Qs System Design**
* Designing an elevator system
* Design a Parking lot system
* Shopping cart – How do you store this information when you use multiple servers that are load balanced.
* How would you design a Twitter Feed? –Grokking the System Design Interview
* Recommendation system for fashion/clothes and accessories – Fundamentals here.
* How does Uber Store & retrieve lat &long for a cab driver?
* If a user is at x,y give me five of the closest drivers. – Grokking the System Design Interview
* Extend the product page X and add the auction capability.
* How are your ensuring security or localization on a mobile device?
* Design a web-based email system.
* Describes pieces, components, design, large scale, and use case
* Design an application like Siri, Cortana or Alexa
* Design Facebook or the privacy features in Facebook.
* Explain different performance scenarios for Instagram architecture.
* Explain the different places you have caching in OneDrive.
* Designing an activity feed system – Grokking the System Design Interview
* Design WhatsApp / Facebook Messenger: Issues of each, scaling problems, offline/online users and availability, notification etc 
* Grokking the System Design Interview” & Link-1 & Link 2
* An airline carrier is losing a lot of bags – Design a solution.
* Design Dropbox etc. – Grokking the System Design Interview
* Design X’s frequently viewed product page shows the last 5 items you viewed.
* Design the product recommendation feature based on a user’s purchase history.
* Design an online poker game or Tick Tack Toe for multi-players.
* Solve for persistence, concurrency, scale.
* Instagram –Grokking the System Design Interview
* Design a URL compression system – Bitly – Link 1, Link 2
* Search engine: basic crawling, collection, hashing etc. (Depends on your expertise on this topic).
* Autocomplete / Typeahead Search- Link
* Design a coupon system for a website like Peach or Uber.
* Design a picture sharing website. How will you store thumbnails, photos? Usage of CDNS? Caching at various layers etc.
* Design a push and inbox messaging platform.
* Design a product based on maps, eg Hotel / ATM finder given a location.
* Design malloc, free and garbage collection system. What data structures to use? Decorator pattern over malloc etc.
* Design a site like www.Pronto.com (price comparison, availability on eCommerce websites)
* When and will you cache, how often would you query, crawl efficiency, etc?
* Design a system for collaborating over a document simultaneously (e.g.: google docs)?
* Design an electronic election / Ballot machine architecture
* Design a logging system – Splunk or ELK* 
* Design Netflix, Youtube, Spotify –Grokking the System Design Interview
* Build a machine learning system to detect if a fake user.
* How do you design a system with 99.999% availability
* Design an amusement Park Ticketing system for user ride efficiency
* Design Uber –Grokking the System Design Interview
* Design an Inventory Management System
* Design a Video Conferencing application. – InfoQ Solution
* Design any of the above architectures only using AWS, GPC or Azure- For Any cloud team.
* Troubleshoot a slow website or a slow e-reading device.

## SysDesign Topics
**Functional**
* Security (OAuth , Encryption)
* Load Balancing / Proxies / Reverse Proxy
* Databases : SQL(relational),NOSQL , In-memory DB , Sharding , Redundancy , Replication , Indexes
* Data Partitioning ( Consistent hashing)
* Caching (Caching Strategies , Tools like redis/memcached)
* Microservices Vs Monoliths
* Message Queues ( MB Kafka , RabbitMQ for async processing)
* API Design 
* Rate Limiting ( Throttling users and services , preventing DDOS)
* Monitoring and Logging (System Health , Metrics , Alerting)
* Connecting Protocols ( TCP , UDP , HTTPS , Websockets)

**Non-Functional**
* Scalability
* Consistency vs Availability (CAP theorem)
* Concurrency ( Concurrent Processing , Multithreading , Synchronization)
* Reliability ( Data replication , Single Point of Failure , System Failover) 
* Cost Optimization

**User Facing Products**
* Designing Pastebin 
* Designing Typeahead Suggestion 
* URL Shortener ( Bitly , Generating short URLs, Handling redirects ,Analytics)
* Designing Facebook’s Newsfeed 
* Designing Yelp or Nearby Friends 
* Web Crawler ( URL Queue Management , HTML parsing , Data Storage)
* Search Engine( Crawling , Indexing , Query Serving)
* Social Media Platforms ( Twitter , FB , Instagram , Post updates , Follow users , Timeline generation , Twitter search)
* Video Streaming Service ( Netflix/Amazon prime/Hotstar, Video uploads , video Views , Live Streaming , Recommendation Engine)
* E-commerce Website ( Amazon/Flipkart , Product Search , User Authentication , Online Payment processing , Flash Sale)
* Chat Application(WA/FB Messenger , Real time messaging , Online indicators , Group Chats) 
* Ride sharing Service ( Ola/Uber , Ride matching , Tracking , Fare estimation)
* Gaming Platforms ( Handling multiple players , Real time updates , game state management) 
* Email Service ( Sending Emails , Receiving emails , Storage of emails , searching emails )
* Reservation / booking system ( Reliability)

**Technical products**
* Rate Limiter
* Job Scheduler ( Prioritize and distribute jobs to workers)
* Logging Service ( High throughput , Low latency , Easily Searchable)
* Distributed File Storage Service ( S3/Dropbox , Data Sharding , Replication , Fault Tolerance)
* Real-time Analytics Dashboard ( Collection of data , Process data , Data Visualization) 

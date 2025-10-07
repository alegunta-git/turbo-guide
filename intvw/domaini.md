## Database 
db docs
* https://docs.oracle.com/database/121/COMSC/diagrams.htm#COMSC00016
* [DB Design](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=intro.html)
* [DB models](https://web.archive.org/web/20210508051645/http://www.databaseanswers.org/data_models/index_all_models.htm)
* [oracle wiki](https://en.wikiversity.org/wiki/Oracle_SQL_Fundamentals)
* [Oracle 9i docs](https://docs.oracle.com/cd/B10501_01/index.htm)
* [SQL Server](https://www.sqlservertutorial.net/sql-server-basics/sql-server-select-into/)
* [Mysql](https://www.mysqltutorial.org/getting-started-with-mysql/)

yt db
* [yt ora sql](https://www.youtube.com/watch?v=uIsRVBtwXM4)
* [yt sql](https://www.youtube.com/watch?v=p3qvj9hO_Bo&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=6&pp=gAQBiAQB)
* [yt sql2](https://www.youtube.com/watch?v=uIsRVBtwXM4&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=7&pp=gAQBiAQB)
* [yt DB Design PL](https://youtube.com/playlist?list=PLZDOU071E4v6epq3GS0IqZicZc3xwwBN_&si=oRGQtHil9Jhwgkmn)




## API

**yt api**
* [How to Design Good API](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/32713.pdf)
* [REST API tutorial](https://www.restapitutorial.com/)
* [rest api sudoku](https://www.youtube.com/playlist?list=PLTCrU9sGybupzS5-3iYTsYUI1emBDKdHu)
* [yt http course](https://www.youtube.com/watch?v=iYM2zFP3Zn0&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=1&pp=gAQBiAQB)
* [yt json](https://www.youtube.com/watch?v=iiADhChRriM&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=5&pp=gAQBiAQB)
* [yt api design](https://www.youtube.com/watch?v=hEj61QV0wdg&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=1&pp=gAQBiAQB)
* [yt api documentation](https://www.youtube.com/watch?v=NawxzLB4aro&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=2&pp=gAQBiAQB)
* [yt postman beginner](https://www.youtube.com/playlist?list=PLhW3qG5bs-L9P22XSnRe4suiWL4acXG-g)
* [upi](https://www.youtube.com/watch?v=iI2NaN_QVTI&list=PLmMyXRtEtJEb0qXMQIZEvGmTDqDLuxkCA&index=11&pp=gAQBiAQB)
* [api pagination](https://www.youtube.com/watch?v=14K_a2kKTxU&list=PLmMyXRtEtJEb0qXMQIZEvGmTDqDLuxkCA&index=9&pp=gAQBiAQB)


**API Documentation**
* HTTP : https://www.cheat-sheets.org/saved-copy/http-response-codes-1.pdf
* https://owasp.org/www-project-api-security/
* https://developer.mozilla.org/en-US/docs/Web/HTTP
* https://www.javatpoint.com/http-request
* https://rapidapi.com/blog/api-glossary/
* https://stackoverflow.blog/2020/03/02/best-practices-for-rest-api-design/
* [doc learn apis ratthwerwriting](https://idratherbewriting.com/learnapidoc/docapis_introtoapis.html)
* [API Ship docs](https://www.aftership.com/docs/tracking/quickstart/api-quick-start)
* [Parse API](https://docs.parseplatform.org/rest/guide/)
* [Stripe API](https://stripe.com/docs/api/customers)
* [Dropbox API](https://www.dropbox.com/developers/documentation/http/documentation)
* [Twitter API](https://developer.twitter.com/en/docs/twitter-api/api-reference-index)
* https://tech-docs.io/docs/fax-services
* [python docs](https://docs.python.org/3/tutorial/index.html)
* https://www.globalsqa.com/top-20-open-source-python-libraries/
* http://www.catb.org/esr/writings/taoup/html/
  
**API Topics**
1. API Directory , API Catalog , API Collaboration , API Governance ,API Analytics 
1. API Integration , Internal APIs ,External APIs ,API Versioning 
1. API Gateway , Rate Limiter , Request Timeout , CORS (Cross-Origin Resource Sharing)
1. REST Client , RESTful API ,  SOAP API , GraphQ , Webhooks
1. API Authentication , API Security , API Credentials ,  , API Key
1. API Endpoint , HTTP Verbs , CRUD , Payload(JSON) , Idempotency , Stateful vs Stateless
1. API Development ( API Request , API Response , API Error Codes , Parameters ( Path Parameters , Query Parameters )
1. API Documentation , Developer Portal , SDK
1. API Testing
1. Popular API : Facebook , Amazon WebServices
1. Tools ( JSON schema , API Dev : cURL , API Testing : Postman , API Documentation : Swagger )


**API Efax integration**

Integrating an eFax API involves several key steps. Here's a general outline to guide you through the process:

Steps for eFax API Integration

1. **Select an eFax Provider**
   - Research and choose an eFax API provider (e.g., eFax, RingCentral, HelloFax).
   - Evaluate features, pricing, and user reviews.

2. **Create an Account**
   - Sign up for an account with the chosen eFax provider.
   - Obtain API access credentials (API key, secret, etc.).

3. **Review API Documentation**
   - Familiarize yourself with the provider’s API documentation.
   - Understand the endpoints, request formats, response formats, and authentication methods.

4. **Set Up Development Environment**
   - Choose a programming language (e.g., Python, Java, PHP) and set up the environment.
   - Install any required libraries or SDKs provided by the eFax service.

5. **Authenticate API Requests**
   - Implement authentication in your application.
   - Use the provided API key/secret or OAuth tokens as required.

6. **Send a Fax**
   - Prepare the fax content (PDF or image files).
   - Construct the API request for sending a fax, including:
     - Recipient fax number
     - Sender information
     - Document attachment
   - Send the request and handle the response.

7. **Check Fax Status**
   - Implement a method to check the status of sent faxes.
   - Use the status endpoint provided by the API to retrieve delivery status (sent, failed, pending).

8. **Receive Faxes (if applicable)**
   - Set up a webhook or callback URL to receive incoming faxes.
   - Parse the incoming fax data and store or display it as needed.

9. **Error Handling**
   - Implement error handling for API requests.
   - Log errors for troubleshooting and provide user feedback when issues arise.

10. **Testing**
    - Test the integration thoroughly in a development environment.
    - Verify sending, receiving, and status checking functionalities.

11. **Deploy to Production**
    - Once testing is complete, deploy the integration to your production environment.
    - Monitor the performance and address any issues that may arise.

12. **Documentation and Maintenance**
    - Document your integration process and any customizations made.
    - Stay updated with the provider's API changes and maintenance schedules.

Additional Tips
- **Compliance**: Ensure that your integration complies with relevant regulations (e.g., HIPAA for healthcare-related faxes).
- **Security**: Implement secure coding practices, especially when handling sensitive data.

By following these steps, you can successfully integrate an eFax API into your application.

## Mobile
docs
* [IOS Patterns](https://developer.apple.com/design/human-interface-guidelines/)
* [mobile app features](https://attractgroup.com/blog/most-comprehensive-list-of-mobile-app-features-while-developing-a-mobile-application/)


## Scalability
* [yt scaler sysdesign](https://www.youtube.com/watch?v=P_eh1b6vE-4&list=PLmMyXRtEtJEZUAhYNKCpOBP5tlEP7Ky9h&index=12&pp=gAQBiAQB)
* [amazon whitepapers](https://aws.amazon.com/whitepapers/)
* [G Search Arch](https://www.spyfu.com/blog/how-do-search-engines-work/)
* [G Mapreduce](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)
* [G BigTable](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf) 
* [G ProtocolBuffers](https://spline.de/talks/protobuf.pdf) 
* [G sawzall](https://static.googleusercontent.com/media/research.google.com/en//archive/sawzall-sciprog.pdf)
* [FB Thrift](https://www.ijedr.org/papers/IJEDR2102030.pdf)
* [FB Hive](https://web.cse.ohio-state.edu/~zhang.574/Hive-ICDE10.pdf)
* [FB Tao](https://www.usenix.org/system/files/conference/atc13/atc13-bronson.pdf)
* [High Scalability](http://highscalability.com/all-time-favorites/)
* [Twitter engg blog](https://blog.twitter.com/engineering/en_us)
* [webapps](https://www.youtube.com/watch?v=_higfXfhjdo&list=PLmMyXRtEtJEb0qXMQIZEvGmTDqDLuxkCA&index=8&pp=gAQBiAQB)
* [scalability](https://www.youtube.com/watch?v=EWS_CIxttVw&list=PLmMyXRtEtJEb0qXMQIZEvGmTDqDLuxkCA&index=12&pp=gAQBiAQB)
* [so arch](https://www.youtube.com/watch?v=TWaLeC-kmyU&list=PLmMyXRtEtJEb0qXMQIZEvGmTDqDLuxkCA&index=7&pp=gAQBiAQB)
* Scalability : Sys Design , SRE , High Scalability 
* [blog SD prep](https://blog.pragmaticengineer.com/preparing-for-the-systems-design-and-coding-interviews/)
* https://dev.to/somadevtoo/the-software-design-system-design-interview-preparation-roadmap-with-resources-1no0
* [hn t10 sysdia](https://hackernoon.com/10-tips-for-using-diagrams-to-ace-the-system-design-interview-906p3609)
* https://blog.algomaster.io/p/30-system-design-concepts
* https://dev.to/alexr/14-case-studies-master-system-design-in-a-month-2jk2
* https://dev.to/somadevtoo/top-15-system-design-resources-for-programming-interviews-1m15
* [Dist sys patterns](https://www.freecodecamp.org/news/design-patterns-for-distributed-systems/)
* [Latency numbers](https://gist.github.com/jboner/2841832)
* [Back of envelope](https://www.codementor.io/@robinpalotai/back-of-the-envelope-calculation-for-system-design-interviews-z4ljbsp5l)
* [dt Calc Capacity](https://dev.to/ievolved/how-i-calculate-capacity-for-systems-design-3477)
* [Caching](https://dzone.com/articles/introducing-amp-assimilating-caching-quick-read-fo)
* [Scaler Articles](https://www.scaler.com/topics/articles/)


## Dev Blogs
* [philip Software Engineering for Internet Applications](https://philip.greenspun.com/seia/)
* web publishing : https://philip.greenspun.com/panda/
* https://philip.greenspun.com/humor/graduate-student-emotion-check-list.text
* https://philip.greenspun.com/sql/
* https://philip.greenspun.com/materialism/money
* Software Abstractions MIT Press Daniel Jackson , Quora : Webnode , Livenode
yt Mobile
* [yt apps appstore](https://www.youtube.com/watch?v=Ormjb-BX1sw&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=1&pp=gAQBiAQB)
* [release mobile apps](https://www.youtube.com/watch?v=RIX4ufelA58&list=PLmMyXRtEtJEb0qXMQIZEvGmTDqDLuxkCA&index=13&pp=gAQBiAQB)




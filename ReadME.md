<h1 align="center"> SI Project - SOAP/REST Services </h1>




SOAP services often suffer from the lack of flexibility in comparison to RESTful services. This leads to high maintainence and limits the overall possibilities because of its outdated protocol. Addressing these issues, is to give a clear understanding of the challenges with SOAP, and why REST is more common and flexible to use for developers. 


 overly verbose and hard to maintain
 
 <h1>  REST <span class="emoji">🆚</span> SOAP </h1>
 
<h3> Introduction <g-emoji class="g-emoji" alias="page_facing_up" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4c4.png">📄</g-emoji> </h3>

In the old days, SOAP services were the main protocol to web-based services. Today, SOAP is taking a toll on the modern day developer because it is still used in legacy systems, and some developers choose's SOAP since it support  WS-Security which can come in handy. Also, it is overly verbose and hard to maintain. Nowadays developers generally prefer RESTful web services since it is more widely known, new and easy to use.



<h3>What is REST & SOAP <g-emoji class="g-emoji" alias="interrobang" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2049.png">⁉️</g-emoji></h3>

<h4> SOAP(Simple Object Access Protocol) <img width="50" height="33" src="https://jaxenter.com/wp-content/uploads/2015/06/shutterstock_280038503-e1433408034381.jpg" class="attachment-jaxenter_single_post_image size-jaxenter_single_post_image wp-post-image" alt="" srcset="https://jaxenter.com/wp-content/uploads/2015/06/shutterstock_280038503-e1433408034381.jpg 600w, https://jaxenter.com/wp-content/uploads/2015/06/shutterstock_280038503-e1433408034381-120x80.jpg 120w, https://jaxenter.com/wp-content/uploads/2015/06/shutterstock_280038503-e1433408034381-300x200.jpg 300w" sizes="(max-width: 350px) 100vw, 350px"> </h4>


<img src="./SOAP-envelope.png" align="left">

SOAP is a messaging protocol for the exchange of structured information(XML) in regards of web-service development. SOAP uses XML-structure for the format of messages, relies on protocols such as HTTP and SMTP for data transmission and message exchangement. XML communation consists of several elements to achieve messaging and its major characteristics: 

<img src="./SOAP-envelope.png" align="left">




- An envelope, which indicates how the message is structured and how it gets processed. 
- Encoding rules, which specifies the accessible data-types.
- Collection of methods and responses
- SOAP operates over any protocol(Such as HTTP, SMTP, TCP, etc...)
- SOAP is programmable throughout any model, so it does not rely on a specific pattern.
- Extensibility 
  references: (https://en.wikipedia.org/wiki/SOAP)




  Picture links:(https://www.studytonight.com/rest-web-service/types-of-webservices)
  
  
<h4> REST(REpresentational State Transfer) <img class="mi pn dp t u gs al hc" width="51" height="34" role="presentation" src="https://miro.medium.com/max/599/1*uHzooF1EtgcKn9_XiSST4w.png"> </h4>

REST is an architectural style for developing web-services. Some knows this as the successor of SOAP-based services. This is also known as RESTful web-services. This style, allows the requesting system to manipulate textual documents(or representations) by using a set of stateless operations. 
Reference:(https://en.wikipedia.org/wiki/Representational_state_transfer)
RESTful elements consist of:

- **Client-Server:** The separation of client and server, so that the server and client can be run independently of each other. 
- **Stateless:** The server does not need to know in which state the client is, and vice versa.
- **Cache:** To improve network effiency, a cache layer is added. Since REST is stateless, cache gives the client the upportunity to reuse the response/request later on.
- **Uniform Interface**
- **Layered System**
![](/REST.jpg)


NOTE:: Elaborate in the conclusion about how SOAP exposes all of its functionality(creating a state of the current instance), while RESTful webservices are stateless, and therefore more flexible in terms of developing these web-services
-
The problem lies in SOAP being overly verbose and hard to maintain. Other than problems such as these.

How does SOAP lack of flexibility in comparison to REST? 
Why is SOAP causing higher maintainence in comparison to REST? 
Why is REST more preferable than SOAP? 
we had 

#### notes:

Some of the problems we encounted during our experiment had mainly to do with SOAP. We had no freedom of choice when it came to the response (only XML) as we did with REST (JSON,XML etc.). Also we spent more time doing the SOAP part, because the lines of code was more than in REST. 



<h1>Evidence from our project <g-emoji class="g-emoji" alias="mag" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f50d.png">🔍</g-emoji></h1>

<h5>The following screenshots contain relevant evidence and explanations from our mini assignment in system integration</h5>

<p>(for more details on the project, click <a href="https://github.com/Mokayed/Mini-Project-Web-Services"> here</a>)</p>

<figure>
<h4>1. Requests in SOAP vs REST</h4>
  <img src="./RESTrequest.png" alt="{{ include.description }}">
  <figcaption><li>deposit request in REST using postman</li></figcaption>
  <img src="./SOAPrequest.png" width="800" height="200"/>
  <figcaption><li>deposit request in SOAP using SoapUI</li></figcaption>
  <h6>During development we had a much easier time dealing with REST requests, not only because of us having more knowledge on it, but also because we spent more time in average on building the envelope request whereas the REST request could be made in seconds.</h6>
  <h4>2. Response in SOAP vs REST</h4>
  <img src="./RESTresponse.png" width="300" height="100">
<figcaption><li>the response in REST</li></figcaption>
<img src="./SOAPresponse.png" width="700" height="200">
<figcaption><li>the response in SOAP</li></figcaption>
  <h6>As seen, the response from SOAP is in XML format, and this is something that cannot be changed in SOAP. In REST, the data format was our own choice. As seen we went for JSON. As a result of it being JSON the resposne became much smaller than the envelope response</h6>

<h4>3. The SOAP WSDL File</h4>
<h6>in SOAP, there is only one place to go for requesting endpoints, and that is the WSDL url. Our file ended up having 193 lines of xml code and can be seen by clicking <a href="./customerDetailsWsdl.wsdl.xml"> here</a>. Although we liked the idea of having requests/responses very well structured in WSDL, we could not help feeling annoyed by it being XML, and very verbose. In REST there is no WSDL file where it relies upon the HTTP standard.</h6>

<h4>4. Endpoints</h4>
<img src="./RESTCustomerEndpoint.png">
<img src="./RESTNamePathVariable.png">
<img src="./RESTCustomerNameBrowser.png">
<figcaption><li>endpoint for showing customer name and it's details in REST + shown on browser</li></figcaption>
<img src="./SOAPDepositEndpoint.png">
<figcaption><li>endpoint for deposit request in SOAP, which can only be referred to from the WSDL url</li></figcaption>
<h6>As seen, the REST implementation of the endpoints are very simple, however in SOAP you need to make both a request and response endpoint which ends up being alot of code.<h6>
<h4>5. Total lines of code</h4>

tool used for results: bash (<a href="https://stackoverflow.com/questions/3435581/how-to-count-lines-of-java-code-using-intellij-idea">reference</a>)
<img src="./LinesOfCodeREST.png">
<figcaption>lines of code in our REST project</figcaption>
<img src="./LinesOfCodeSOAP.png">
<figcaption>lines of code in our SOAP project</figcaption>

<h6>the results shows and proofs, that the SOAP project is much more verbose than the REST project.</h6>
</figure>

<h1>Evidence on usability in SOAP vs REST in the industry <g-emoji class="g-emoji" alias="chart_with_downwards_trend" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4c9.png">📉</g-emoji></h1>

<p> The digram is from :
<a>https://www.infoq.com/news/2011/06/Is-REST-Successful/</a></p>

<br>

<img src="./digrams.PNG" align="left">

<p>REST is successful since it is the most used service in the industy. 73% of the APis on Programmable Web use REST. SOAP is far behind but is still represented in 17% of the APIs. The reasoins that makes rest is more in use that it is much easier to implement since it requires less bandwidth and resources, and the uses standard HTTP in rest is much simpler. </p>

<p>REST supports diffrent data types one of the types is JSON, which allows better support for browser clients. One of the main reseans that REST is successful, that REST have better performance and scalability since it's reads can be cached, SOAP based reads cannot be cached. REST supports stateless CRUD operations, which gives the developer a better overview on the data. to read more by clicking <a href="https://medium.com/@LazaroIbanez/soap-vs-rest-68faf2ea970e
"> here</a>. </p>

<p>There is nothing useful in SOAP that can't be done with REST for transport, and JSON, XML, or even plain text for data representation, to read more take a look on that<a href="https://stackoverflow.com/questions/76595/soap-or-rest-for-web-services"> link</a>. </p>

<p>REST allows a better variety of data formats, whereas SOAP only allows XML. Coupled with JSON (which typically works better with data and offers faster parsing), REST is generally considered easier to work with. Thanks to JSON, REST offers better support for browser clients, you can read more by <a href="https://stackify.com/soap-vs-rest/"> clicking here</a>.</p>


<h1>Conclusion <g-emoji class="g-emoji" alias="memo" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4dd.png">📝</g-emoji></h1> 


## Consequences

https://github.com/Mokayed/Mini-Project-Web-Services

### BRAINSTORM: 
Problem definition: 
SOAP vs REST: our experiences with both(SOAP, high maintainence, complex protocol, outdated data transfer models(I.e SOAP envelopes), REST is the successor of SOAP)

here we attach some evidence from our project that has to do with proving the easier implmenatation of rest versus soap. First evidence has to do with lines of code comparably, and second the structure of the response of the data.

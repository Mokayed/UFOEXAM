# SI Project - SOAP/REST Services
<img src="SOAP-vs-REST-.png"/>

#####  REST vs. SOAP

SOAP services often suffer from the lack of flexibility in comparison to RESTful services. This leads to high maintainence and limits the overall possibilities because of its outdated protocol. Addressing these issues, is to give a clear understanding of the challenges with SOAP, and why REST is more common and flexible to use for developers. 
 

 overly verbose and hard to maintain
 ##### Notes (not part of abstract):
REST vs. SOAP: Why REST is more common & flexible to use than SOAP. This is relevant for a developer to have the knowledge for, since SOAP & REST are the most popular Web Service's Protocol in the IT-industry to integrat different systems.

cons for soap: old, not as simple as rest, soap relies only on XML, harder to develop, hard to setup, heavyweight, higher learning curve, expensive tools required, doesnt use get/post/put/delete http protocol, REST APIs are taking over, 



A WSDL file is hard to change, and if a SOAP web service needs to be extended, modified or deprecated in some small form, it’s a big change for both the internal developers and the users (who now must adapt to the new contract).


the XML used in SOAP can become complex and more difficult to program as it tends to be verbose with the XML messaging structure containing an envelope, header, body and fault elements. </p>.................................

## Introduction
In the old days, SOAP services were the main protocol to web-based services. Today, SOAP is taking a toll on the modern day developer because it is still used in legacy systems. Also, it is overly verbose and hard to maintain. Nowadays developers generally prefer RESTful web services since it is more widely known, new and easy to use.

## SOAP(Simple Object Access Protocol)
SOAP is a messaging protocol for the exchange of structured information(XML) in regards of web-service development. SOAP uses XML-structure for the format of messages, relies on protocols such as HTTP and SMTP for data transmission and message exchangement. XML communation consists of several elements to achieve messaging and its major characteristics: 

- An envelope, which indicates how the message is structured and how it gets processed. 
- Encoding rules, which specifies the accessible data-types.
- Collection of methods and responses
- SOAP operates over any protocol(Such as HTTP, SMTP, TCP, etc...)
- SOAP is programmable throughout any model, so it does not rely on a specific pattern.
- Extensibility 
  references: (https://en.wikipedia.org/wiki/SOAP)

  ![](/SOAP-envelope.png)
  ![](SOAP-message.png)
  Picture links:(https://www.studytonight.com/rest-web-service/types-of-webservices)
## REST(REpresentational State Transfer)
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

The problem lies in SOAP being overly verbose and hard to maintain. Other than problems such as these.

How does SOAP lack of flexibility in comparison to REST? 
Why is SOAP causing higher maintainence in comparison to REST? 
Why is REST more preferable than SOAP? 
we had 

#### notes:

Some of the problems we encounted during our experiment had mainly to do with SOAP. We had no freedom of choice when it came to the response (only XML) as we did with REST (JSON,XML etc.). Also we spent more time doing the SOAP part, because the lines of code was more than in REST. 

## Evidence, evidence, evidence

hallur: tag screenshots af projektet i områder som: response, wsdl, endpoints, SOAPUI envelope, tilhørende tekst på hvad der sker på screenshots/sammenligninger.

murched: make research to find some ecidence from the internet (related articles that proofs things that our own project does not)

hazem: Definition af SOAP, definition af REST. Find artikler omkring SOAP disadvantages.
reference to difference between SOAP and REST:(https://smartbear.com/blog/test-and-monitor/understanding-soap-and-rest-basics/) 

## Conclusion 
## Consequences

https://github.com/Mokayed/Mini-Project-Web-Services

### BRAINSTORM: 
Problem definition: 
SOAP vs REST: our experiences with both(SOAP, high maintainence, complex protocol, outdated data transfer models(I.e SOAP envelopes), REST is the successor of SOAP)

here we attach some evidence from our project that has to do with proving the easier implmenatation of rest versus soap. First evidence has to do with lines of code comparably, and second the structure of the response of the data.
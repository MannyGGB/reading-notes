# Reading 08

(https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)

- What does REST stand for? Representational State Transfer. "REST is an architectural style for building distributed systems based on hypermedia."
- REST APIs are designed around a _resource_, which is anything that can be accessed by the client.
- What is an identifier of a resource? An identifier is usually the URI (Uniform Resource Identifier) connected to the resource. Give an example--> https://adventure-works.com/orders/1
- What are the most common HTTP verbs? GET, POST, PUT, PATCH, and DELETE.
  - "GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
  - POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
  - PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
  - PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
  - DELETE removes the resource at the specified URI."
- What should the URIs be based on? Good URIs should be based on nouns or resources, not verbs or the action related to the resource.
- Give an example of a good URI. https://adventure-works.com/orders (In here, orders is the resource)
- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing? A chatty web API sends a lot of requests, which imposes a bigger load on the server. It should be avoided. Instead, it is better to combine related information into bigger resources.
- What status code does a successful GET request return? "HTTP status code 200 (OK)."
- What status code does an unsuccessful GET request return? "404 (Not Found)."
- What status code does a successful POST request return? "HTTP status code 201 (Created)."
- What status code does a successful DELETE request return? "HTTP status code 204 (No Content)."

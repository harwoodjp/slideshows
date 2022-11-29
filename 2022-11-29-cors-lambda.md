## Cors Implementation for AWS Lambda
* CORS fundamentals
* Securing Lambda endpoints
* Resources

---

## CORS fundamentals
### Origin
* Scheme + host name + port number
### CORS
* Cross-origin resource sharing
* Header-based security standard for server-to-server resource sharing
* Specifies, binarily, whether an origin should load resources from another origin 
### SOP
* Same-origin policy  
* Browser's default CORS implementation
* Specification that servers can only talk to themselves
### Validation
* Compare request origin against origin allowed by server
* Server responds with requested data or error
* Preflight check and in request/response headers

---

## Securing Lambda endpoints
* Add preflight OPTIONS check to API Gateway Resources
* Return CORS headers in all Lambda responses
* Add variable for allowed origin in TF/AWS environments



---

## Resources
* [Diagram](https://excalidraw.com/#json=7rPwN-shyapn0sY962jlR,8XcjNZK5ShOZYyRD9ufLIg)
* [CorsConfig](https://awslabs.github.io/aws-lambda-powertools-python/develop/core/event_handler/api_gateway/#cors)
* [Terraform and CORS-Enabled AWS API Gateway](https://mrponath.medium.com/terraform-and-aws-api-gateway-a137ee48a8ac)
* [CORS In Action](https://www.manning.com/books/cors-in-action)

<!-- 
~~~graph-easy --as=boxart
[ A ] - to -> [ B ]
~~~
 -->
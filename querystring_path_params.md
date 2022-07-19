# QueyString Params vs Path params in a rest api 

> QueryString Params

QueryString params are basically added at the end of the url using `?`. It is used to sort,filter the resources. 
The multiple querstrings can be passed in url by usig `&` symbol in most of the websites. 

**Example:**

https://example.com/users/?sort=DESC

https://example.com/users/?name=John&city=Southampton&sort=DESC


------------

> path Params

Path params are used to identify a resource. Basically path params used to find a resource that is fixed and don't change.
It is used with symbol `/`

**Example:**

https://example.com/users/yaswanth

https://example.com/cars/tata/ev

----------

> Resources 

https://stackoverflow.com/questions/30967822/when-do-i-use-path-params-vs-query-params-in-a-restful-api

https://stackoverflow.com/questions/4024271/rest-api-best-practices-where-to-put-parameters

https://aws.amazon.com/premiumsupport/knowledge-center/pass-api-gateway-rest-api-parameters/

https://www.geeksforgeeks.org/how-to-pass-the-query-string-parameters-to-aws-lambda-function-or-http-endpoint/

https://www.youtube.com/watch?v=r9IZnuZstXM


https://dzone.com/articles/understanding-the-uri-param-and-query-param-with-r#:~:text=URI%20parameter%20(Path%20Param)%20is,to%20sort%2Ffilter%20those%20resources.

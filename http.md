# HTTP Request
### GET
* GET Request doesn't have a body. If you want to query things by restrictions, please add them to the url with the following format
    * curl http:// IP:port/items?attribue1=abc&attribute2=xxx
* How to realize array in a url?
    * The idea of .csv(comma-seperated values) file
    * example: curl http:// IP:port/items?attribue1=abc,def,ghi,jkl&attribute2=xxx
        * abc,def,ghi,jkl = [abc,def,ghi,jkl]
        * If each element has comma within it, use "" to contain each elament
            * "a,b,c","d,e,f"
### POST
* POST Request has a body, and in Python, we need a model in the handler to handle the request
### PUT
### DELETE
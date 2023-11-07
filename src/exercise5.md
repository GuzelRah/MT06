# Activities
## 1. Эндпоинт GET​/api​/v1​/Activities 
__Эндпоинт:__ GET​/api​/v1​/Activities  
__HTTP-метод:__ GET   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Activities  
__Заголовки запроса:__ "accept: text/plain; v=1.0"     
__Тело запроса:__   
__Статус-код ответа:__ 200  
__Тело ответа:__   
[  
  {  
    "id": 1,  
    "title": "Activity 1",  
    "dueDate": "2023-08-16T18:07:29.0925434+00:00",  
    "completed": false  
  },  
  {  
    "id": 2,  
    "title": "Activity 2",  
    "dueDate": "2023-08-16T19:07:29.0925456+00:00",  
    "completed": true  
    }
]  
## 2. Эндпоинт POST ​/api​/v1​/Activities 
### В теле запроса id:0
__Эндпоинт:__ POST ​/api​/v1​/Activities  
__HTTP-метод:__ POST  
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Activities  
__Заголовки запроса:__ "accept: text/plain; v=1.0"  "Content-Type: application/json; v=1.0"   
__Тело запроса:__   
{  
  "id": 0,  
  "title": "string",  
  "dueDate": "2023-08-16T17:20:36.198Z",  
  "completed": true  
}    
__Статус-код ответа:__   200  
__Тело ответа:__    
 {  
  "id": 0,  
  "title": "string",  
  "dueDate": "2023-08-16T17:20:36.198Z",  
  "completed": true  
}  
### В теле запроса id:p
__Эндпоинт:__ POST ​/api​/v1​/Activities  
__HTTP-метод:__ POST  
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Activities  
__Заголовки запроса:__ "accept: text/plain; v=1.0" "Content-Type: application/json; v=1.0"   
__Тело запроса:__     
{  
  "id": р,  
  "title": "string",  
  "dueDate": "2023-08-17T17:37:28.418Z",  
  "completed": true  
}     
__Статус-код ответа:__   400  Error: Bad Request  
__Тело ответа:__    
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-e0fe5f350697a94fa24933df9de5bb49-774a2048494d014b-00",  
  "errors": {  
    "$.id": [  
       "'0xD1' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."  
    ]  
  }  
}  
## 3. Эндпоинт GET ​/api​/v1​/Activities​/{id}
#### ID: 1
__Эндпоинт:__ GET ​/api​/v1​/Activities​/{id}  
__HTTP-метод:__  GET      
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Activities/1  
__Заголовки запроса:__  "accept: text/plain; v=1.0"  
__Тело запроса:__ 
{  
  "id": 1,  
  "title": "Activity 1",  
  "dueDate": "2023-08-16T18:30:55.6885263+00:00",  
  "completed": false  
}    
__Статус-код ответа:__   
__Тело ответа:__   

#### ID: 35  
__Эндпоинт:__ GET ​/api​/v1​/Activities​/{id}   
__HTTP-метод:__ GET     
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Activities/35  
__Заголовки запроса:__ "accept: text/plain; v=1.0"  
__Тело запроса:__     
__Заголовки ответа:__  
 api-supported-versions: 1.0   
 content-type: application/problem+json; charset=utf-8; v=1.0   
 date: Wed16 Aug 2023 17:33:45 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 404 Error: Not Found  
__Тело ответа:__   
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",  
  "title": "Not Found",  
  "status": 404,  
  "traceId": "00-1f25a0ff0cac5b4ebedbac407107574b-d63f810d42902141-00"  
}    
## 4. Эндпоинт PUT​/api​/v1​/Activities​/{id} 
#### ID 1
__Эндпоинт:__ PUT​/api​/v1​/Activities​/{id}  
__HTTP-метод:__ PUT  
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Activities/1  
__Заголовки запроса:__ "accept: text/plain; v=1.0"  "Content-Type: application/json; v=1.0"   
__Тело запроса:__     
{  
  "id": 0,  
  "title": "string",  
  "dueDate": "2023-08-16T17:41:49.019Z",  
  "completed": true  
}      
__Заголовки ответа:__     
 access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Wed16 Aug 2023 17:43:06 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 200 	
Success  
__Тело ответа:__   
 {  
  "id": 0,  
  "title": "string",  
  "dueDate": "2023-08-16T17:41:49.019Z",  
  "completed": true  
}     
#### ID 10000000000
__Эндпоинт:__ PUT​/api​/v1​/Activities​/{id}  
__HTTP-метод:__  PUT   
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Activities/10000000000    
__Заголовки запроса:__ "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"    
__Тело запроса:__     
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-08-17T09:44:01.742Z",
  "completed": true
}   
__Заголовки ответа:__     
  access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 09:44:07 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
__Статус-код ответа:__ 400 Error: Bad Request 	  
__Тело ответа:__   
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-ce513b1103dc68459ddfbcde9dee0ab7-1cc8a943d6a64f43-00",  
  "errors": {  
    "id": [  
      "The value '10000000000' is not valid."  
    ]  
  }  
}       
## 5. Эндпоинт DELETE​/api​/v1​/Activities​/{id}
__Эндпоинт:__ DELETE ​/api​/v1​/Activities​/{id}    
__HTTP-метод:__ DELETE  
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Activities/1   
__Заголовки запроса:__  "accept: */*"  
__Тело запроса:__   
__Заголовки ответа:__   
access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-length: 0   
 date: Thu17 Aug 2023 09:22:37 GMT   
 server: Kestrel   
__Статус-код ответа:__  200   
__Тело ответа:__   

# Authors
## 6. Эндпоинт GET​/api​/v1​/Authors
__Эндпоинт:__ GET​/api​/v1​/Authors     
__HTTP-метод:__  GET   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors    
__Заголовки запроса:__  "accept: text/plain; v=1.0"   
__Тело запроса:__   
__Заголовки ответа:__  
api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 09:26:16 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 200   
__Тело ответа:__ 
[  
  {  
    "id": 1,  
    "idBook": 1,  
    "firstName": "First Name 1",  
    "lastName": "Last Name 1"  
  },  
  {  
    "id": 2,  
    "idBook": 1,  
    "firstName": "First Name 2",  
    "lastName": "Last Name 2"  
  }  
  {   
    ...    
    },  
  {  
    "id": 30,  
    "idBook": 1,  
    "firstName": "First Name 3",  
    "lastName": "Last Name 3"  
  },    
]  
## 7. Эндпоинт POST​/api​/v1​/Authors  
### В теле запроса id": 0
__Эндпоинт:__ POST​/api​/v1​/Authors   
__HTTP-метод:__  POST   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors   
__Заголовки запроса:__  "accept: text/plain; v=1.0"  "Content-Type: application/json; v=1.0"  
__Тело запроса:__   
{  
  "id": 0,  
  "idBook": 0,  
  "firstName": "string",  
  "lastName": "string"  
}    
__Заголовки ответа:__    
access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 09:30:16 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
__Статус-код ответа:__ 200     
__Тело ответа:__    
 {  
  "id": 0,  
  "idBook": 0,  
  "firstName": "string",  
  "lastName": "string"  
}  
### В теле запроса id": z
__Эндпоинт:__ POST​/api​/v1​/Authors   
__HTTP-метод:__  POST   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors   
__Заголовки запроса:__  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"  
__Тело запроса:__   
{  
  "id": z,  
  "idBook": 0,  
  "firstName": "string",  
  "lastName": "string"  
}    
__Заголовки ответа:__    
 access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 17:46:21 GMT   
 server: Kestrel   
 transfer-encoding: chunked        
__Статус-код ответа:__ 400 Error: Bad Request    
__Тело ответа:__      
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-7d73498f9003da44bbcd2344d96eac8e-7eb85da7a647b841-00",  
  "errors": {  
    "$.id": [  
      "'z' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."  
    ]  
  }  
}   
## 8. Эндпоинт GET ​/api​/v1​/Authors​/authors​/books​/{idBook} 
### ID 1
__Эндпоинт:__ GET
​/api​/v1​/Authors​/authors​/books​/{idBook}    
__HTTP-метод:__ GET         
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/1       
__Заголовки запроса:__  "accept: text/plain; v=1.0"  
__Тело запроса:__     
__Заголовки ответа:__    
api-supported-versions: 1.0    
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 09:3:24 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
__Статус-код ответа:__ 200     
__Тело ответа:__    
[  
  {  
    "id": 1,  
    "idBook": 1,  
    "firstName": "First Name 1",  
    "lastName": "Last Name 1"  
  },  
  {  
    "id": 2,  
    "idBook": 1,  
    "firstName": "First Name 2",  
    "lastName": "Last Name 2"  
  },  
  {  
    "id": 3,  
    "idBook": 1,  
    "firstName": "First Name 3",  
    "lastName": "Last Name 3"  
  },  
  {  
    "id": 4,  
    "idBook": 1,  
    "firstName": "First Name 4",  
    "lastName": "Last Name 4"  
  }  
]  
### ID 10000000000
__Эндпоинт:__ GET
​/api​/v1​/Authors​/authors​/books​/{idBook}  
__HTTP-метод:__ GET       
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/10000000000  
__Заголовки запроса:__ "accept: text/plain; v=1.0"       
__Тело запроса:__   
__Заголовки ответа:__    
 content-type: application/problem+json; charset=utf-8 
 date: Thu17 Aug 2023 09:38:43 GMT 
 server: Kestrel 
 transfer-encoding: chunked     
__Статус-код ответа:__ 400 Error: Bad Request     
__Тело ответа:__  
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-f55dfb15c0e4f44ca6cb7aeb658dcade-28fdddf8fbbc354c-00",  
  "errors": {  
    "idBook": [
      "The value '10000000000' is not valid."  
    ]  
  }  
}  
## 9. Эндпоинт GET /api/v1/Authors/{id}
### ID 1
__Эндпоинт:__ GET/api/v1/Authors/{id}   
__HTTP-метод:__ GET     
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors/1     
__Заголовки запроса:__  "accept: text/plain; v=1.0"  
__Тело запроса:__     
__Заголовки ответа:__    
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 10:03:37 GMT   
 server: Kestrel   
 transfer-encoding: chunked       
__Статус-код ответа:__ 200     
__Тело ответа:__    
{  
  "id": 1,  
  "idBook": 1,  
  "firstName": "First Name 1",  
  "lastName": "Last Name 1"  
}  
### ID 10000000000
__Эндпоинт:__ GET​/api​/v1​/Authors​/{id}  
__HTTP-метод:__  GET   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors/10000000000  
__Заголовки запроса:__  "accept: text/plain; v=1.0"   
__Тело запроса:__   
__Заголовки ответа:__      
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 10:05:26 GMT   
 server: Kestrel   
 transfer-encoding: chunked        
__Статус-код ответа:__ 400 Error: Bad Request     
__Тело ответа:__  
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-f55dfb15c0e4f44ca6cb7aeb658dcade-28fdddf8fbbc354c-00",  
  "errors": {  
    "idBook": [
      "The value '10000000000' is not valid."  
    ]  
  }  
}  
## 10. Эндпоинт PUT/api/v1/Authors/{id}
### ID 1
__Эндпоинт:__ PUT/api/v1/Authors/{id}     
__HTTP-метод:__  PUT   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Authors/1        
__Заголовки запроса:__  "accept: text/plain; v=1.0"  "Content-Type: application/json; v=1.0"    
__Тело запроса:__ 
 {  
  "id": 0,  
  "idBook": 0,  
  "firstName": "string",  
  "lastName": "string"  
}     
__Заголовки ответа:__ 
access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 10:10:55 GMT   
 server: Kestrel   
 transfer-encoding: chunked       
__Статус-код ответа:__ 200       
__Тело ответа:__   
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
### ID 10000000000
__Эндпоинт:__ PUT/api/v1/Authors/{id}    
__HTTP-метод:__  PUT      
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Authors/10000000000  
__Заголовки запроса:__ "accept: text/plain; v=1.0" "Content-Type: application/json; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__  
 access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 10:12:05 GMT   
 server: Kestrel   
 transfer-encoding: chunked         
__Статус-код ответа:__ 400 Error: Bad Request       
__Тело ответа:__   
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-4e17624206401c4d8a23ae94c6860bf5-1d1f739e89107b41-00",  
  "errors": {  
    "id": [  
      "The value '10000000000' is not valid."  
    ]  
  }  
}     
## 11. ЭндпоинтDELETE ​/api​/v1​/Authors​/{id}

__Эндпоинт:__ DELETE ​/api​/v1​/Authors​/{id}  
__HTTP-метод:__  DELETE       
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/Authors/1    
__Заголовки запроса:__  "accept: */*"  
__Тело запроса:__     
__Заголовки ответа:__ 
 access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-length: 0   
 date: Thu17 Aug 2023 10:15:46 GMT   
 server: Kestrel      
__Статус-код ответа:__ 200     
__Тело ответа:__   

# Books
## 12. ЭндпоинтGET​/api​/v1​/Books

__Эндпоинт:__ GET​/api​/v1​/Books  
__HTTP-метод:__   GET        
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/Books  
__Заголовки запроса:__  "accept: text/plain; v=1.0"  
__Тело запроса:__     
__Заголовки ответа:__   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 10:27:26 GMT   
 server: Kestrel   
 transfer-encoding: chunked    
__Статус-код ответа:__ 200     
__Тело ответа:__   
[  
  {  
    "id": 1,  
    "title": "Book 1",  
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,  
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-08-16T10:27:26.8826372+00:00"
  },  
    {  
      ....  
     },  
  {  
    "id": 2,  
    "title": "Book 2",  
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",  
    "pageCount": 200,  
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",    
    "publishDate": "2023-08-15T10:27:26.8826536+00:00"
  },
]
## 13. ЭндпоинтPOST​/api​/v1​/Books
### В теле запроса id:0
__Эндпоинт:__
__HTTP-метод:__  POST  
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Books    
__Заголовки запроса:__  "accept: */*" "Content-Type: application/json; v=1.0"  
__Тело запроса:__   
{  
  "id": 0,  
  "title": "string",  
  "description": "string",  
  "pageCount": 0,  
  "excerpt": "string",  
  "publishDate": "2023-08-17T10:30:56.404Z"  
}      
__Заголовки ответа:__    
 access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 10:31:03 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 200     
__Тело ответа:__  
{  
  "id": 0,  
  "title": "string",  
  "description": "string",  
  "pageCount": 0,  
  "excerpt": "string",  
  "publishDate": "2023-08-17T10:30:56.404Z"  
}  
### В теле запроса id:x
__Эндпоинт:__
__HTTP-метод:__  POST  
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Books    
__Заголовки запроса:__  "accept: */*"   "Content-Type: application/json; v=1.0"  
__Тело запроса:__   
{  
  "id": x,  
  "title": "string",  
  "description": "string",  
  "pageCount": 0,  
  "excerpt": "string",  
  "publishDate": "2023-08-17T10:30:56.404Z"  
}      
__Заголовки ответа:__      
  access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 17:57:46 GMT   
 server: Kestrel   
 transfer-encoding: chunked    
__Статус-код ответа:__ 400  Error: Bad Request   
__Тело ответа:__  
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-bbd54af5e68e3342a3e5b154b7c9010a-b50e4e8722ed0a4f-00",  
  "errors": {  
    "$.id": [  
      "'x' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."  
    ]  
  }  
}  
## 14. Эндпоинт GET​/api​/v1​/Books​/{id}
### ID 1
__Эндпоинт:__ GET​/api​/v1​/Books​/{id}  
__HTTP-метод:__  GET           
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Books/1    
__Заголовки запроса:__  "accept: text/plain; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 10:35:44 GMT   
 server: Kestrel   
 transfer-encoding: chunked    
__Статус-код ответа:__ 200     
__Тело ответа:__   
{  
  "id": 1,  
  "title": "Book 1",  
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",  
  "pageCount": 100,  
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",  
  "publishDate": "2023-08-16T10:35:44.8554568+00:00"  
}   
### ID 10000000000
__Эндпоинт:__ GET​/api​/v1​/Books​/{id}  
__HTTP-метод:__   GET        
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/Books/10000000000    
__Заголовки запроса:__   "accept: text/plain; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__     
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 10:37:23 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 400 Error: Bad Request         
__Тело ответа:__ 
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-550947243690c8488da18fb6839b4a93-14755a596226134f-00",  
  "errors": {  
    "id": [  
      "The value '10000000000' is not valid."  
    ]  
  }  
} 
 ## 15. Эндпоинт PUT​/api​/v1​/Books​/{id}
### ID 1
__Эндпоинт:__ PUT​/api​/v1​/Books​/{id}  
__HTTP-метод:__  PUT       
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/Books/1  
__Заголовки запроса:__  "accept: */*"  "Content-Type: application/json; v=1.0"   
__Тело запроса:__   
 {  
  "id": 0,  
  "title": "string",  
  "description": "string",  
  "pageCount": 0,  
  "excerpt": "string",  
  "publishDate": "2023-08-17T10:41:31.706Z"  
}     
__Заголовки ответа:__    
 access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 10:41:38 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
__Статус-код ответа:__ 200     
__Тело ответа:__    
{  
  "id": 0,  
  "title": "string",  
  "description": "string",  
  "pageCount": 0,  
  "excerpt": "string",  
  "publishDate": "2023-08-17T10:41:31.706Z"  
}  
### ID 10000000000
__Эндпоинт:__ PUT​/api​/v1​/Books​/{id}  
__HTTP-метод:__   PUT   
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/Books/10000000000  
__Заголовки запроса:__ "accept: */*"  "Content-Type: application/json; v=1.0"   
__Тело запроса:__    
{  
  "id": 0,  
  "title": "string",  
  "description": "string",  
  "pageCount": 0,  
  "excerpt": "string",  
  "publishDate": "2023-08-17T10:41:31.706Z"  
}   
__Заголовки ответа:__     
 access-control-allow-origin: *  
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 10:44:08 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 400 Error: Bad Request         
__Тело ответа:__   
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-6425dcb64209444a988648555e5d16d4-436cee6cfa655c44-00",  
  "errors": {  
    "id": [  
      "The value '10000000000' is not valid."  
    ]  
  }   
} 
 ## 16. Эндпоинт DELETE ​/api​/v1​/Books​/{id}
### ID 1
__Эндпоинт:__ DELETE​/api​/v1​/Books​/{id}  
__HTTP-метод:__ DELETE            
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Books/1       
__Заголовки запроса:__   "accept: */*"   
   __Тело запроса:__     
__Заголовки ответа:__    
access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-length: 0   
 date: Thu17 Aug 2023 10:56:04 GMT   
 server: Kestrel   
__Статус-код ответа:__ 200     
__Тело ответа:__  
# CoverPhotos
## 17. Эндпоинт GET /api/v1/CoverPhotos
__Эндпоинт:__ GET ​/api​/v1​/Users  
__HTTP-метод:__ GET           
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos   
__Заголовки запроса:__  "accept: text/plain; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__    
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 12:44:49 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 200     
__Тело ответа:__   
[  
  {  
    "id": 1,  
    "idBook": 1,  
    "url": "https://placeholdit.imgix.net/~text?  txtsize=33&txt=Book 1&w=250&h=350"   
  },  
{  
...  
},  
  {  
    "id": 200,  
    "idBook": 200,  
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"  
  }  
]   
## 18. Эндпоинт POST ​/api​/v1​/CoverPhotos
### В теле запроса id:0
__Эндпоинт:__ POST ​/api​/v1​/CoverPhotos  
__HTTP-метод:__     POST   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos      
__Заголовки запроса:__  "accept: text/plain; v=1.0" "Content-Type: application/json; v=1.0"  
__Тело запроса:__  
{  
  "id": 0,  
  "idBook": 0,  
  "url": "string"  
}   
__Заголовки ответа:__   
access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 12:51:33 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 200     
__Тело ответа:__  
{  
  "id": 0,  
  "idBook": 0,  
  "url": "string"  
}  
### В теле запроса id:a
__Эндпоинт:__ POST ​/api​/v1​/CoverPhotos  
__HTTP-метод:__     POST   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos      
__Заголовки запроса:__  "accept: text/plain; v=1.0"  "Content-Type: application/json; v=1.0"  
__Тело запроса:__  
{  
  "id": a,  
  "idBook": 0,  
  "url": "string"  
}   
__Заголовки ответа:__   
access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 18:03:05 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 400  	Error: Bad Request   
__Тело ответа:__  
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-7a1d4b749c12074c8e0768456c82955a-4a903ed8e8381443-00",  
  "errors": {  
    "$.id": [  
      "'a' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."  
    ]  
  }  
}    
## 19. Эндпоинт GET​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}
### ID 1
__Эндпоинт:__ GET​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}  
__HTTP-метод:__  GET        
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/1  
__Заголовки запроса:__  "accept: text/plain; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 12:54:27 GMT   
 server: Kestrel   
 transfer-encoding: chunked    
__Статус-код ответа:__ 200         
__Тело ответа:__  
[
  {
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  }
]
### ID 10000000000
__Эндпоинт:__ GET​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}  
__HTTP-метод:__  GET         
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/10000000000   
__Заголовки запроса:__   "accept: text/plain; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__      
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 12:56:32 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 400 Error: Bad Request         
__Тело ответа:__  
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-b63ad1caefc23c4aa15f227df68747df-cfbb4e5abd7a9a4b-00",  
  "errors": {  
    "idBook": [  
      "The value '10000000000' is not valid."  
    ]  
  }  
}  
## 20. Эндпоинт  GET​/api​/v1​/CoverPhotos​/{id}
### ID 1
__Эндпоинт:__  GET​/api​/v1​/CoverPhotos​/{id}  
__HTTP-метод:__     GET   
__Полный URL запроса:__     https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1  
__Заголовки запроса:__  "accept: text/plain; v=1.0"  
__Тело запроса:__     
__Заголовки ответа:__   
api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 13:03:02 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
   __Статус-код ответа:__ 200         
__Тело ответа:__  
{  
  "id": 1,  
  "idBook": 1,  
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"  
} 
### ID 10000000000
__Эндпоинт:__  GET​/api​/v1​/CoverPhotos​/{id}  
__HTTP-метод:__     GET         
__Полный URL запроса:__    https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/10000000000  
__Заголовки запроса:__  "accept: text/plain; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__     
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 13:04:54 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 400 Error: Bad Request         
__Тело ответа:__       
 {  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-2054d5060b82844384dfc41eee304f41-d11483e1a988304c-00",  
  "errors": {  
    "id": [  
      "The value '10000000000' is not valid."  
    ]  
  }  
}  
## 21. Эндпоинт PUT​/api​/v1​/CoverPhotos​/{id}
### ID 1
__Эндпоинт:__ PUT​/api​/v1​/CoverPhotos​/{id}   
__HTTP-метод:__  PUT   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1  
__Заголовки запроса:__  "accept: text/plain; v=1.0"  "Content-Type: application/json; v=1.0"  
__Тело запроса:__   
{  
  "id": 0,  
  "idBook": 0,  
  "url": "string"  
}    
__Заголовки ответа:__     
 access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 13:07:03 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
   __Статус-код ответа:__ 200         
__Тело ответа:__  
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
### ID 10000000000
__Эндпоинт:__  PUT​/api​/v1​/CoverPhotos​/{id}  
__HTTP-метод:__  PUT         
__Полный URL запроса:__   https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/10000000000    
__Заголовки запроса:__ "accept: text/plain; v=1.0" "Content-Type: application/json; v=1.0"   
__Тело запроса:__           
__Заголовки ответа:__    
 access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 13:10:13 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
__Статус-код ответа:__ 400 Error: Bad Request         
__Тело ответа:__     
{   
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-fd43c0cbea31f540a206e278b2c137ce-624b7ad46d798545-00",  
  "errors": {  
    "id": [  
      "The value '10000000000' is not valid."  
    ]  
  }  
}   
## 22. Эндпоинт DELETE ​/api​/v1​/CoverPhotos​/{id}
__Эндпоинт:__ DELETE ​/api​/v1​/CoverPhotos​/{id}       
__HTTP-метод:__   DELETE   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1  
__Заголовки запроса:__  "accept: */*"    
__Тело запроса:__     
__Заголовки ответа:__   
 access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-length: 0   
 date: Thu17 Aug 2023 13:13:09 GMT   
 server: Kestrel     
   __Статус-код ответа:__ 200         
__Тело ответа:__  


# Users 
## 23. Эндпоинт GET​/api​/v1​/Users
__Эндпоинт:__    GET​/api​/v1​/Users  
__HTTP-метод:__   GET     
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Users  
__Заголовки запроса:__  "accept: text/plain; v=1.0"  
__Тело запроса:__     
__Заголовки ответа:__   
api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 13:16:13 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
   __Статус-код ответа:__ 200         
__Тело ответа:__     
[
  {
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
  },
  {
   ...
  },
  {
    "id": 10,
    "userName": "User 10",
    "password": "Password10"
  }
]
## 24. Эндпоинт POST​/api​/v1​/Users
### В теле запроса id:0
__Эндпоинт:__ POST​/api​/v1​/Users     
__HTTP-метод:__  POST   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Users  
__Заголовки запроса:__  "accept: */*"  "Content-Type: application/json; v=1.0"  
__Тело запроса:__      
{  
  "id": 0,  
  "userName": "string",  
  "password": "string"  
}     
__Заголовки ответа:__   
access-control-allow-origin: *    
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 13:19:48 GMT   
 server: Kestrel   
 transfer-encoding: chunked     
   __Статус-код ответа:__ 200         
__Тело ответа:__    
{  
  "id": 0,  
  "userName": "string",  
  "password": "string"  
}  
### В теле запроса id:Q
__Эндпоинт:__ POST​/api​/v1​/Users     
__HTTP-метод:__  POST   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Users  
__Заголовки запроса:__  "accept: */*"  "Content-Type: application/json; v=1.0"  
__Тело запроса:__      
{  
  "id": Q,  
  "userName": "string",  
  "password": "string"  
}     
__Заголовки ответа:__   
 access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 18:12:03 GMT   
 server: Kestrel   
 transfer-encoding: chunked       
   __Статус-код ответа:__ 400 Error: Bad Request         
__Тело ответа:__  
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",  
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-b25285453b5b7948b84bb94864274624-faecf18192633f4c-00",  
  "errors": {  
    "$.id": [  
      "'Q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."  
    ]  
  }  
}  
## 25. Эндпоинт GET​/api​/v1​/Users​/{id}
### ID 1
__Эндпоинт:__ GET​/api​/v1​/Users​/{id}   
__HTTP-метод:__  GET     "accept: */*"  
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Users/1  
__Заголовки запроса:__  "accept: */*"  
__Тело запроса:__     
__Заголовки ответа:__    
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 13:23:00 GMT   
 server: Kestrel   
 transfer-encoding: chunked      
   __Статус-код ответа:__ 200         
__Тело ответа:__    
{  
  "id": 1,  
  "userName": "User 1",  
  "password": "Password1"  
}  
### ID 100
__Эндпоинт:__  GET​/api​/v1​/Users​/{id}  
__HTTP-метод:__  GET        
__Полный URL запроса:__  https://fakerestapi.azurewebsites.net/api/v1/Users/100     
__Заголовки запроса:__    "accept: */*"       
 __Тело запроса:__  
__Заголовки ответа:__    
 api-supported-versions: 1.0   
 content-type: application/problem+json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 13:26:52 GMT   
 server: Kestrel   
 transfer-encoding: chunked  
__Статус-код ответа:__ 404 Error:  Not Found      
__Тело ответа:__    
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",  
  "title": "Not Found",  
  "status": 404,  
  "traceId": "00-4e0c4beef285194c8781607c1206fb08-3e5a8a3710734a40-00"  
}  
## 26. Эндпоинт PUT​/api​/v1​/Users​/{id}
### ID 1
__Эндпоинт:__  PUT​/api​/v1​/Users​/{id}      
__HTTP-метод:__   PUT      
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Users/1    
__Заголовки запроса:__ "accept: */*" "Content-Type: application/json; v=1.0"   
__Тело запроса:__   
{  
  "id": 0,  
  "userName": "string",  
  "password": "string"  
}    
__Заголовки ответа:__     
 access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-type: application/json; charset=utf-8; v=1.0   
 date: Thu17 Aug 2023 13:30:49 GMT   
 server: Kestrel   
 transfer-encoding: chunked  
   __Статус-код ответа:__ 200         
__Тело ответа:__  
{  
  "id": 0,  
  "userName": "string",  
  "password": "string"  
}  
### ID 10000000000
__Эндпоинт:__  PUT​/api​/v1​/Users​/{id}  
__HTTP-метод:__    PUT   
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Users/10000000000        
__Заголовки запроса:__  "accept: */*"  "Content-Type: application/json; v=1.0"   
__Тело запроса:__     
__Заголовки ответа:__    
 access-control-allow-origin: *   
 content-type: application/problem+json; charset=utf-8   
 date: Thu17 Aug 2023 13:33:34 GMT   
 server: Kestrel   
 transfer-encoding: chunked   
__Статус-код ответа:__ 400 Error: Bad Request         
__Тело ответа:__ 
{  
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1", 
  "title": "One or more validation errors occurred.",  
  "status": 400,  
  "traceId": "00-daf7daa9f036e242bfb489d7906c0413-dcd18323a28af145-00",  
  "errors": {  
    "id": [  
      "The value '10000000000' is not valid."  
    ]  
  }  
}  
## 27. Эндпоинт DELETE ​/api​/v1​/Users​/{id}
__Эндпоинт:__  DELETE ​/api​/v1​/Users​/{id}  
__HTTP-метод:__ DELETE    
__Полный URL запроса:__ https://fakerestapi.azurewebsites.net/api/v1/Users/1  
__Заголовки запроса:__  "accept: */*"     
__Тело запроса:__     
__Заголовки ответа:__    
access-control-allow-origin: *   
 api-supported-versions: 1.0   
 content-length: 0   
 date: Thu17 Aug 2023 13:36:14 GMT   
 server: Kestrel    
   __Статус-код ответа:__ 200         
__Тело ответа:__  

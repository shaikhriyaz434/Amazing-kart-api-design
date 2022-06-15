## Amazing-kart-api-design

  # 1. Resources/collections:
    
    refer to api-spec.yaml file. you can you use https://editor.swagger.io for preview.

    
    list of resource:
      a. Users
      b. Products
      c. Categories
      d. Inventories
      e. Payments
      f. Addresses
      g. Orders
      h. checkout [function]
      i. refund [function but it can be a object depending on data model]


  # 2. Response codes/Payload:
    
    refer to api-spec.yaml file. you can you use https://editor.swagger.io for preview.
    
        '200': Response with content
       
        '204':
          description: No Content
        '400':
          description: Bad Request
        '401':
          description: Request Unauthorized
        '404':
          description: Not Found
        '406':
          description: Not Acceptable
        '500':
          description: Internal Server Error
        '502':
          description: Bad Gateway
        '504':
          description: Gateway Timeout

  # 3. Common Headers:

  3.1 Request Headers:

        a. accept
        b. timestamp
        c. Content-Type [for req payloads]


  3.2 Response headers

        a. Content-Type
        b. e-tag
        c. Date
        d. last-modified

  # 4. Security

      1. use https 
      2. jwt authorization
      3. timestamp in every request headers to tackle DDOS.

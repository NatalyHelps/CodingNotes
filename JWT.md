<h1>JSON Web Token</h1> 
<h2>3 Parts of JSON WEB TOKEN</h2>
<ol>
  <li>Header</li>
  <li>Payload</li>
  <li>Signature</li>
</ol>
<details>
    <summary>JWT Header</summary>
    Contains the type of token to be created, and the signing algorithm you're going to use. The type is always 'JWT'

</details>
      ```{
      'alg': 'HS256',  
      'typ': 'JWT'
    }

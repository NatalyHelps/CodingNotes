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
  
```
{
      'alg': 'HS256',  
      'typ': 'JWT'
}
```
</details>
<details>
    <summary>JWT Payload</summary>
  
      A JWT payload contains claims about an entity. A claim is a statement or piece of information and the entity is often a user. There are three claims: Registered, Public, and Private. Anyone can use Registered claim types. Public are created by the developer and can be used publicly. They should be registered to avoid collisions. (repeated claims) Private claims are not registered or public. They're only used between parties that have agreed to use them. 
  
```
{
       'sub': '1234567890',
       'name': 'Harine Cooper',
       'admin': false,
       'iat': 1620924478,
       'exp': 1620939187
}
```
</details>

<details>
    <summary>JWT Signature</summary>

</details>



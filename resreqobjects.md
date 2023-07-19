<h1>Commonly used methods on the req, res objects in Express</h1>
<br />
<br />
<table>
  <thead>
    <tr>
      <th>Request Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>req.params</b></td>
      <td>Provides access to route parameters in the URL.</td>
    </tr>
    <tr>
      <td>req.query</td>
      <td>Gives access to query parameters from the URL query string.</td>
    </tr>
    <tr>
      <td>req.body</td>
      <td>Allows access to the request body when using middleware like body-parser to parse incoming data.</td>
    </tr>
    <tr>
      <td>req.headers</td>
      <td>Provides access to the HTTP headers sent with the request.</td>
    </tr>
    <tr>
      <td>req.cookies</td>
      <td>Gives access to any cookies sent with the request.</td>
    </tr>
    <tr>
      <td>req.method</td>
      <td>Retrieves the HTTP method of the request (e.g., GET, POST, PUT, DELETE).</td>
    </tr>
    <tr>
      <td>req.path</td>
      <td>Retrieves the path portion of the URL.</td>
    </tr>
    <tr>
      <td>req.route</td>
      <td>Contains information about the current route matched for the request.</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Response Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>res.send()</td>
      <td>Sends a response to the client with a specified body.</td>
    </tr>
    <tr>
      <td>res.json()</td>
      <td>Sends a JSON response to the client.</td>
    </tr>
    <tr>
      <td>res.render()</td>
      <td>Renders a view template using a specified template engine.</td>
    </tr>
    <tr>
      <td>res.redirect()</td>
      <td>Redirects the client to a different URL.</td>
    </tr>
    <tr>
      <td>res.status()</td>
      <td>Sets the status code of the response.</td>
    </tr>
    <tr>
      <td>res.header()</td>
      <td>Sets an HTTP response header.</td>
    </tr>
    <tr>
      <td>res.cookie()</td>
      <td>Sets a cookie to be sent with the response.</td>
    </tr>
    <tr>
      <td>res.sendFile()</td>
      <td>Sends a file as the response.</td>
    </tr>
  </tbody>
</table>

<h1>Model→Controller→View</h1>
<details>
    <summary>Model</summary>
    In the MVC (Model-View-Controller) architectural pattern, the Model is a critical component that represents the data and the business logic of the application. It encapsulates the core functionalities and behaviors related to the application's data, often interacting directly with the database or other data sources.
</details>
<details>
    <summary>View</summary>
    The component that presents data to the user and handles how that data is displayed. It is the user interface of the application, and it renders the data from the Model in a way that is understandable and actionable for the user.
</details>
<details>
    <summary>Controller</summary>
    the Controller is a crucial component responsible for handling user input, updating the Model accordingly, and selecting the appropriate View for rendering to the user. It acts as an intermediary between the Model and the View, facilitating the flow of data and interactions within the application.

---
    
Routes are typically managed within the Controller layer, but are often defined separately for organizational purposes.

Routes: routes act as the entry points that map incoming HTTP requests to specfic controller actions.
When a request comes in, the routing mechanism determines which controller and action should handle the request. 

ACTIONS - Routes call the appropriate controller methods (actions) to handle the incoming requests.

The controller methods then interact with the Model to fetch or update data and pass this data to the view for rendering. 
</details>

<h1>Questions</h1>
<details>
    <summary>Which part of MVC are routes?</summary>
   CONTROLLER - However, they are typically defined separately for the sake of organization. 
</details>



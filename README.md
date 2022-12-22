# VIPERARCHIOS

VIPER is an architectural pattern like MVC or MVVM, yet it isolates the code further by single duty.

As Per the design it is clear that


View

will have access to Presenter It means that View will ask Presenter to perform any task like update UI,  Tap Events , Fetch data from api / Database


Presenter
will have access to Interactor and Router It means Presenter will handover the task to Interactor (Business Login Unit) and Router to Navigate to a specific location 

Interactor 
Interactor will have all the Business logic and do the network call or Local DB call now this Network Layer or Database layer will be having access to Entity

Router 
This is the entry point for any Module and Presenter will have access to it and it will point to the view 

Entity

This are the Model class now Network / Database Layer will have access to the Entity


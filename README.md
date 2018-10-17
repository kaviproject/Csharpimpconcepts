# C# concepts
LINQ TO SQL CONCEPTS
ENUM

C# Life Cycle
SessionContext

# Install LINQ to SQL tool 

1. Launch the visual studio launcher
2. Modify from the dropdown list
3. select linq to sql checkbox

In the visual studio open the server explorer
open the dbml file and drag drop from the left to right.

# TFS for database project
  1. Dackpack will give the comparision changes
  2. Schema Comparision
  3. click the publish
  4. it will generate the script
  5. SEED method used to deploy the static table
  6. Transform we can use precompiler and postcompiler
  
 # Rules engine
  1. Drools tool 
  2. SIMPLE WORFLOWS
  3. Nrules nuget packages

 # c#
 1. Differnece between the ref and out ?
    ref is used to initilize the value before passing in to the method.
    out is used to get the value during the runtime or initialization.
 2. ENUM types? what is mean by bitenum?
    Normal enum is used to map one-one relationship.
    bitenum is used to map one to many relationship(security roles 1,2,3...)
 3. PATTERNS (Factory,Absoulte,singleton,sequential,facade)
     Factory pattern can apply for multiple grids in the UI
 4. SIGNALIR used to sync the data between the 2 tabs.
 
 # Life cycle to display the data on the UI
  Integrate the STOREPROC using LINQ TO SQL;
  In the repository folder get the values and assign to the model;
  Create the properties in the model;
  In the controller call the repository integration method;
  Access the properties in the view.
 
# Telerik Grid related 
Refresh is not working?
Sorting is not working?
1. Add clientTemplate 
2. Add grid action in the controller
3. add the clientevent then it will call the grid action in the controller.
4. refesh will also work after integrating the clienttemplate and sorting..
Here is the URL:
https://docs.telerik.com/devtools/aspnet-ajax/controls/grid/data-binding/understanding-data-binding/webservice-binding/client-binding

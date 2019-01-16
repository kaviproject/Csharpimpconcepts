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
# Here is the URL:
https://docs.telerik.com/devtools/aspnet-ajax/controls/grid/data-binding/understanding-data-binding/webservice-binding/client-binding


# TODO
http://dotnetpattern.com/csharp-versions-features
http://venkatcsharpinterview.blogspot.com/2009/01/c-interview-questions.html

# C# 2.0 Features
# Generics
Generics are extensively used by collection classes availible in system.collection.namespace.generics
we have requirment to compare the 2 values either string or integer. C# is strongly typed so we have to give the data type.
we can use object type to compare 2 data type values using object type. >NET directly or indirectl calls the object type to campare the values. At that timeperformance will decrease because of boxing and unboxing.

Generic syantax <T> -->T means is type(we can give any name to indicate the generics)
  
  we can use Classes,interfaces, delegates and collections...
  
 # where can we use abstract classes and interface classes..
 Abstarct class no need to be instantiated..
 we have requirment to implement public employee class and private employee class..
 But boh have some common properties like id,firstname and lastname ..
 In yhis case better to use one common method to implement the functionality..to avoid duplicate code.. in the future if we want to add middle name we have to add in the 2 plavess(fulltime and contract)
 
 we can implemnt abstract class like below ..
 
 public abstract class BaseEmployee{
 public int Id{get;set;
 public string Firstname{get;set;}
 public string Lastname{get;set;}
 public string Fullname()
 {
 return this.firstName+this.LastName;
 }
 
 pvblic abstract getMonthlySalary()
 ;
 }
public class FullTimeEmployee:BaseEmployee{
public intAnnualSalary{get;set;}
public override int GetMontlySalary()
{
return this.AnnualSalary/12;
}
}
public class ContractEmployee:BaseEmployee
{
public int HourlyPay{get;set;}
public int TotalHoursWorked{get;set;}
public override int GetMontlySalary()
{
return this.HourlyPay*this.TotalHoursWorked;
}
}
}
# Interface concepts
we can create interface with the keyword .Just like classes interfaces also contains properties,methods,delegates and events but only declarations and no implementations.

Interface members are public by default and they do not allow explicit access modifiers.

Interface cannot contain fields.

If a class or struct inherits from an interface,it must provide implementation for all inteface members otherwise it will get the complie error.

**** click on the interface its automatically create the implemenatation method.
****Explicit interface method:

# Difference between Abstract class and Interface?

Abstract class can have implementations for some of its members(Methods),but the interface cant have implementaion for any of its members.
interface can have fields whereas abstarct class can have the fields.
An interface can inherit from another interface only and cannot inherit from an abstarct class, where as an abstarct class can inherit abstract class and interface.
A class can inherit from multiple interfaces at the same time, whereas class cannot inherit from multiple classes at the same time.
ABstarct classe members can have access modifiers where as interface members cannot have access modifiers by default its public.

# SQL BASIC
Open the store proc with command line:
sp_helptext procedurename
Exec command 
For executing the script we have to remove the header part and replce the declare and run each statement


https://www.infoq.com/presentations/code-documentation
SWAGGER
RESHARPER

find the table name based on column name

SELECT c.name AS ColName, t.name AS TableName
FROM sys.columns c
    JOIN sys.tables t ON c.object_id = t.object_id
WHERE c.name LIKE '%%';

SELECT c.name AS ColName, t.name AS TableName
FROM sys.columns c
    JOIN sys.tables t ON c.object_id = t.object_id
WHERE c.name='WINofEssentialPerson';

Get table schema for datatype 
select COLUMN_NAME, DATA_TYPE, CHARACTER_MAXIMUM_LENGTH, 
       NUMERIC_PRECISION, DATETIME_PRECISION, 
       IS_NULLABLE 
from INFORMATION_SCHEMA.COLUMNS
where TABLE_NAME=''
# GOOD WEBSITE FOR WRITING TECHNICAL DOCUMENTS
https://medium.com/machine-words/writing-technical-design-docs-71f446e42f2e

#React Tutorial

https://flaviocopes.com/page/ebooks/

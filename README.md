# Modifiers

There are 4 types of modifiers in java - 

        Default

        Public

        Private 

        Protected


## Default modifier

- If we dont write any modifier, it will be default modifier.

- The default modifier in java is deafult. 

- It is applicable to classes, methods, varibles and constructors.

- Within the package we can access the data by default modifier.

## Public Modifier

- All packages can access public data.

- It is applicable to classes, methods, varibles and constructors.


## Private modifier

- We can access the private data within the class only.

- It is applicable to methods, varibles and constructors.

- If the parent class contains private data then the child class cannot acess the data.

- The private modifier is the most restricted modifier in java.

Example:

 class Parent{
 
     private int num = 100;
     
 }

 class Child extends Parent{
 
    public void display(){
    
          System.out.println(num);       // error
          
    }
    
 }

 
## Protected modifier

- By protected modifier we can access the data within the package, and outside the package only child classes can access( like Inheritance ).

- It is applicable to methods, varibles and constructors.

## IN SHORT

public :      All packages can access

private :     Only within the class

protected :      Within the package + outside package only child class( like Inheritance )

default :      Only within the package

Modifier       -----                classes          ------          methods          -------        variables          -------     constructors

public          ----------              Yes           -----------            Yes            -----------         Yes             -------------      Yes

default          ----------              Yes          -----------             Yes            -----------          Yes           -------------     Yes

protected          ----------             No           -----------            Yes            -----------         Yes            -------------      Yes

private          ----------             No           -----------            Yes            -----------         Yes            -------------      Yes



Note: You can can make classes, methods, vairables, and constructors public. So, I said "yes".

You can can make classes, methods, vairables, and constructors default. So, I said "yes".

You can can make methods, vairables, and constructors protected except classes. So, I said "no".

You can can make methods, vairables, and constructors private except classes. So, I said "no".






# Package Coding Convention

Package is a folder. We create the package to maintain the data in proper format. So the code maintenece becomes easy.

- Instead of writing all codes in a single package, we create multiple foders in the application.

### Two Types 

1 - predefined packages

Predefined packages are the packages Jame Gosling made.

Ex:

java.lang

java.io

java.util

applet

awt

math

net

nio

rmi

security

text

sql

time

beans


2 - user defined package

- The packages declared by user

- Declare the package using package keyword

  Example:

  package shubha.pokharel;

  class A{
      logics
  }

    shubha
  
       ↳
         pokharel

             ↳

                A



  Note: In realtime this isnt good. It is valid but it is not recommanded.




  ## Package Coding Convention

  1 - The package should reflect with the company domain name

    Example:

       www.wipro.com     →      package com.wipro;
       www.pnc.com       →      package com.pnc;    

  - It will show that the package belongs to wipro/pnc.
 
2 - It should reflect with the project name

   Example:

     project name: tech, bank

        ↳    package com.wipro.tech;
         ↳   package com.pnc.bank;



3 - It should reflect with the module name.

- The module name is the segment of the project/ sub modules.

- For an example, in the bank we have loans, withdraws etc. Loans is a module here.

  Example:

   module name: loans

     ↳     package com.wipro.tech.loans;
     ↳     package com.pnc.bank.loans;

  - All the loan related classes should be present here.
 


If you don't work for a company. You can pretend you are in a company. It is not mandatory. But you have to follow this kind of convention.


## Eclipse IDE

- The workspace is the location of the data.

- Your project will be stored where your workspace is located.


Steps on creating a package in Eclipse IDE:

1 - Open eclipse IDE and click on "launch"

2 - On the top right, click on "Open prespective". It is a grid with a shine. Then, a pop up will open

3 - Select Java and then click on "Open"

4 - On the top left click on "File", right click "New" and click on "Java Project"

5 - Click on "project name" It asks you for the project name, so put the project name. Do not select anything.

6 - Inside the package Explorer, we have our project name. Click on the project name. We will have 2 folders which is "JRE System Library" and "src"(source code).

7 - Right click on src

8 - Click on "New"  → "Package"

9 - In the name feild, give package name.
Ex:
 ↳
    com.tcs.services

10 - Click on finish

11 - Right click on package → New → Class

12 - give the class name and select "public static void main"(you do not have to click on the main method).

13 - Right Click in the file that has main method → Run as → Java Application

Note:

The src folder contains java code.

The bin folder contains classes.



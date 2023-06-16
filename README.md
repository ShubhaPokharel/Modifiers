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

********************************IN SHORT***************************************************************

public :      All packages can access

private :     Only within the class

protected :      Within the package + outside package only child class( like Inheritance )

default :      Only within the package

 # JavaScript
 ## Print in Browser
 
    document.write( "Hello World");

 ## Variable declare,assign,add :
    var a = 12;
    var b =13;
    var c = a+b;
    document.write(a+ "+" + b + "=" + c);
##  Array

An array is an object that can store a  **collection of items**. Arrays become really useful when you need to store large amounts of data of the same type. Suppose you want to store details of 500 employees. If you are using variables, you will have to create 500 variables whereas you can do the same with a single array. You can access the items in an array by referring to its  **indexnumber**  and the index of the first element of an array is zero.
You can create an array in JavaScript as given below.

    var students = ["John", "Ann", "Kevin"];
If you want to add more elements to the students array, you can do it like this:

    students[3] = "Emma";
	students[4] = "Rose";
You can also create an array using Array constructor like this:

    var students = new Array("John", "Ann", "Kevin");
### JavaScript Array Methods
1.  **length property**  --> If you want to know the number of elements in an array, you can use the length property.
2.  **prototype property**  --> If you want to add new properties and methods, you can use the prototype property.
3.  **reverse method**  --> You can reverse the order of items in an array using a reverse method.
4.  **sort method -->**  You can sort the items in an array using sort method.
5.  **pop method**  --> You can remove the last item of an array using a pop method.
6.  **shift method**  --> You can remove the first item of an array using shift method.
7.  **push method**  --> You can add a value as the last item of the array.

        var no = [1,2,5,6,4,3,7,9,8];
        
        //Display Length
        document.write(no.length+ "<br/>");
        //Array Sort
        no.sort();
        document.write(no + "<br/>");
        //Array Reverse 
        no.reverse();
		document.write(no + "<br/>");
        //Pop
        no.pop();
        document.write(no + "<br/>");
        //Push
        no.push(10);
        document.write(no);
### Loop

Loops are useful when you have to execute the same lines of code repeatedly, for a specific number of times or as long as a specific condition is true.

### For Loop

    var vowels = ["a","e","i","o","u"];
        
    for(var i = 0 ; i<vowels.length ; i++)
    {
        document.write(vowels[i] + "<br/>") ;
    }
  
  ### While Loop
  

    var vowels = ["a","e","i","o","u"];
    var i = 0;
        
    while(i<vowels.length)
    {
        document.write(vowels[i] + "<br/>");
        i++;
    }
### Conditional Statements

Conditional statements are used to decide the flow of execution based on different conditions.

    var hours = new Date().getHours();
        
    if (hours<12)
    {
        document.write("AM");
    }
    else 
    {
        document.write("PM");
    }
### Function
A function is a block of code which will be executed only if it is called.

    function add(a , b)
    {
         return(a+b);
    }
    document.write(add(4,5));

###  Object Methods

Objects can also have  **methods**.Methods are  **actions**  that can be performed on objects.Methods are stored in properties as  **function definitions**.

    var person = {  
	firstName: "John",  
	lastName : "Doe",  
	id : 5566,  
	fullName : function() {  
		return  this.firstName + " " + this.lastName;  
		}  
	}
### This Keyword
In a function definition,  **this**  refers to the "owner" of the function. In the example above,   **this.firstName**  means the  **firstName**  property of  **this object**.

### Accessing Object Methods

    name = person.fullName();
    /* If you access a method **without** the () parentheses, it will return the function definition */
    name = person.fullName;

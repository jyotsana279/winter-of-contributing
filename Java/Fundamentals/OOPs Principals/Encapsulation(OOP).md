What is Encapsulation?
In object-oriented computer programming languages, the notion of encapsulation (or OOP Encapsulation) refers to the bundling of data, along with the methods that operate on that data, into a single unit. Many programming languages use encapsulation frequently in the form of classes. A class is a program-code-template that allows developers to create an object that has both variables (data) and behaviors (functions or methods). A class is an example of encapsulation in computer science in that it consists of data and methods that have been bundled into a single unit.

Encapsulation may also refer to a mechanism of restricting the direct access to some components of an object, such that users cannot access state values for all of the variables of a particular object. Encapsulation can be used to hide both data members and data functions or methods associated with an instantiated class or object.

Inheritance vs Abstraction vs Encapsulation: What's the Difference?
Along with inheritance, encapsulation and abstraction form the three central principles of object-oriented programming.

What is Inheritance in programming?
Inheritance is a mechanism that allows one class to gain the properties of another class, in the same way, that a child inherits some attributes from each of their parents. Inheritance allows programmers to create a new class that reuses the data members and methods of an existing class.

What is Abstraction in programming?
Abstraction occurs when a programmer hides any irrelevant data about an object or an instantiated class to reduce complexity and help users interact with a program more efficiently. The term abstraction vs encapsulation can be used to describe the process of hiding some of the information contained in an object or class, but it may also refer to the object itself. An abstraction is any named entity that contains a selection of data and behaviors specific to a particular usage of the originating entity.

Encapsulation in OOP and Containerization Explained
Containers are a relatively new type of software that can be used to virtually package a piece of code along with all of its libraries and other dependencies that it needs to execute. Containers create an encapsulated virtual environment where an application can be launched using the minimum amount of storage space and computing power. A group of containers can share access to a single operating system and draw their computing resources from a single piece of hardware.

Encapsulation in OOP: Containers vs Virtual Machines
Containerization has emerged as an alternative to virtual machines because of its highly efficient usage of computing resources. Virtualization allowed multiple operating systems and applications to run at the same time while sharing the resources of a single computer. Containers improved on this model by sharing a host operating system and installing the container runtime engine onto the host machine's operating system.

A computer running four virtual machines expends additional resources for each instance of the operating system that it runs, while a computer with an installed containerization engine could run the same number of applications on a single operating system. As a result, multiple containers can operate using the same computing capacity as a single virtual machine.

Containers are just one example of encapsulation in coding where data and methods are bundled together into a single package.

How is Information Hidden via Encapsulation Programming?
As we mentioned earlier, encapsulation in object oriented programming allows developers to bundle data and methods together but it can also be used to hide sensitive data that should not be exposed to users. In the Java programming language, and in many other languages, information hiding is controlled using getter/setter methods for data attributes that will be readable or that may be updated by other classes.

Encapsulation in OOP: Getter/Setter methods
A getter method is used to retrieve the value of a specific variable within a class. A setter method is used to set or update the value of a specific variable within a class. Programmers can use access modifiers to define the visibility and accessibility of classes, along with the data and methods that they contain. In the Java programming language, there are four types of access modifiers to choose from:

i) Private - When the private access modifier is applied to an attribute or method, it can only be accessed by code within the same class. As a result, the class will likely need to include getter and setter methods that can be used to access information about the attribute or to change its value. Variables that can only be accessed through getter and setter calls are encapsulated.
Protected - A variable or method that is protected can be accessed by code within the same class, by any classes that are in the same package and by all sub-classes in the same or other packages.
ii) Public - The public access modifier is the least restrictive of all. Methods, attributes, and classes that are coded with this access modifier can be viewed and accessed by code within the same class and within all other classes.
No Modifier - When a variable has no access modifier, it can be accessed or viewed from within the same class or from all other classes in the same package.
There are many benefits to hiding information about attributes and methods using encapsulation in programming. One is that it prevents other developers from writing scripts or APIs that use your code. With encapsulation, users of a class do not learn how a class stores its data and the developer can change the data type of a field without forcing developers and users of the class to change their code.
Code for understanding encapsulation
class EncapsulationDemo{
    private int ssn;
    private String empName;
    private int empAge;

    //Getter and Setter methods
    public int getEmpSSN(){
        return ssn;
    }

    public String getEmpName(){
        return empName;
    }

    public int getEmpAge(){
        return empAge;
    }

    public void setEmpAge(int newValue){
        empAge = newValue;
    }

    public void setEmpName(String newValue){
        empName = newValue;
    }

    public void setEmpSSN(int newValue){
        ssn = newValue;
    }
}
public class EncapsTest{
    public static void main(String args[]){
         EncapsulationDemo obj = new EncapsulationDemo();
         obj.setEmpName("Mario");
         obj.setEmpAge(32);
         obj.setEmpSSN(112233);
         System.out.println("Employee Name: " + obj.getEmpName());
         System.out.println("Employee SSN: " + obj.getEmpSSN());
         System.out.println("Employee Age: " + obj.getEmpAge());
    } 
}
Output:

Employee Name: Jyotsana
Employee SSN: 123256
Employee Age: 22
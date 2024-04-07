# TAUnotes9a-11b

public class Notes {

    //CONSTRUCTORS IN INHERITANCE
        //Superclass constructors run first
            //A superclass's constructor is run before the subclass's constructor.
        //use 'super' to call specific constructors
            //explicit calls can be made to superclass's constructors from one of the subclass's constructors by using 'super'.

                            public MyClass() {
                                super();
                            }

        //Super calls must be first
            //Calls to the superclass constructors must be the first statement in the subclass's constructor.
        //Some constructors must be executed
            //If a superclass does not have a default constructor, the subclass must explicitly call one of its other constructors.


    //LIMITING ACCESS IN INHERITANCE
        //Constructors are not inherited
        //Public and protected members
            //These two methods and fields are inherited by its subclasses
                public int publicField;
                protected String protectedField;

                public void publicMethod() {
                }
                protected void protectedMethod() {
                }

        //Private members
            //These methods and fields are not inherited
                private double privateField;

                private void privateMethod() {
                }

        //Final methods
            //These methods are inherited but cannot be overridden
                    public final void myFinalMethod() {
                    }


    //POLYMORPHISM KEY POINTS
        //Type VS Instance
            //Objects have a superclass type and a subclass instance
    // Superclass Type
    class Animal {
        void makeSound() {
            System.out.println("Some sound");
        }
    }

    // Subclass Instance
    class Dog extends Animal {
        void makeSound() {
            System.out.println("Woof");
        }
    }

        //Access
            //Polymorphic objects can only access the methods of their type, not their instance. CASTING is required to access the methods of their instance.
        if (dog instanceof Dog) {
        Dog myDog = (Dog) dog;
        myDog.fetch(); // Accessing Dog-specific method
    }
        //Overridden Methods
            //When a method is overridden by the subclass, the polymorphic object will execute the overridden method at runtime.
        @Override
        void makeSound() {
            System.out.println("Woof");
        }
        //InstanceOf operator
            //The 'instanceOf' operator is used to determine if an object is an instance of a certain cass.


    //ABSTRACTION KEY POINTS
        //Templates
            //Abstract classes and methods are templates that are meant to be implemented by their subclasses.
        //Reserved Word
            //Classes and methods are declared abstract by using the 'abstract' keyword.
        //Implementation Required on Inheritance
            //if a subclass extends from an abstract class, it MUST implement its abstract methods, or be declared 'abstract' itself.
        //Abstract Classes
            //These classes cannot be instantiated, it is only to be used as a superclass. If even one method in a class is abstract, the class must be declared abstract as well.


    //INTERFACE KEY POINTS
        //Not for instantiation
            //Interfaces cannot be instantiated
        //Implement
            //Interfaces are implemented, not extended.
        //Abstract if not implemented
            //Any class that implements an interface MUST implement all of its methods, or it must declare itself abstract.
        //Abstract Methods
            //Methods in an interface must be 'abstract' or default.







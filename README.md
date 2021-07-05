# ruby-for-java-dev

#### Showing Ruby syntax and the Java equivalent

### **- Comments**

```// Java:```

```
// Single line comment

/** Multi
    Line
    Comment
**/
```

```// Ruby:```

```
# Single line comment

=begin
    Multi
    Line
    Comment
=end
```

### **- Variables**

```// Java:```

```
int num = 1;
float numFloat = 1.0;
int[] numArray = {1,2,3};
String text = "Random text";
final CONSTANT_VALUE = "random-value";
// Java 9 or higher ->
Map<Object, Object> dictionary = Map.of(
"a", "b",
"c", "d"
);
```

```// Ruby:```

```
num = 1
num_float = 1.0
num_array = [1,2,3]
text = "Random text"
CONSTANT_VALUE = "random-value"
dictionary = {"a" => "b","c" => "d"}
```

Note: From Java 10 local variables can be defined using the 'var' keyword e.g;

```var text = "Random text"```

### **- Methods**

```// Java:```

```
public String returnText(String text){
    return text;
}
```

```// Ruby:```

```
def return_text(text)
    text
end
```

### **- Class**

```// Java:```

```
public class Animal{
}
```

```// Ruby:```

```
class Animal
end
```

### **- Class Inheritance**

```// Java:```

```
public class Dog extends Animal{
}
```

```// Ruby:```

```
class Dog < Animal
end
```


### **- Constructor **
```// Java:```

```
  public class Animal {
    public Animal(){
        // contructor behaviour here
    }
  }
      
```

```// Ruby:```

```
  class Animal
    def initialize
        # contructor behaviour here
    end
  end
```

### **- Creating Instance of a Class**

```// Java:```

```
Person person = new Person();
```

```// Ruby:```

```
person = Person.new
```

### ** Getters And Setters **
```// Java:```

```
  public class Animal {
    private String name;
    
    public getName(){
        return this.name;
    }
    
    public setName(String name){
        this.name = name;
    }
  }
      
```

```// Ruby:```

```
  # One way  
  class Animal
    
    def get_name
        @name
    end    
    
    def set_name(name)
        @name = name
    end
    
  end
  
  # Another way 
  class Animal
    # for getters
    attr_reader :name
    # for setters
    attr_writer :name
    
    # or for both getters and setters
    attr_accessor :name
    
  end
  
```

### **- Reference To Current Instance of an Object**

```// Java:```

```
public class Animal{
 private void eat(){
    // eat
 }
 
 public void callEat(){
    this.eat();
 }
}
```

```// Ruby:```

```
class Animal
    def eat
        # eat
    end

    def call_eat
        self.eat
    end    
end
```

### **- (Switch) Case (When) statements **

```// Java:```

```
int age = 10;

switch(age){
    case 10:
    // do something
    break;
    case 18:
    // do something
    break;
    case 50:
    // do something
    break;
    default:
    // do something default
}
```

```// Ruby:```

```
age = 10

case age
    when 10:
    # do something
    when 18:
    # do something
    when 50:
    # do something
    else
    # do something default
end    
```

### **- If/Else Statements **
```// Java:```

```
  if(age < 18){
    // do something
  } else if (age > 50){
    // do something
  } else {
    // do something
  }
      
```

```// Ruby:```

```
  if(age < 18)
    # do something
   elsif (age > 50)
    # do something
   else
    # do something
  end
```

### **- Print/Print Line **
```// Java:```

```
  System.out.print("Hello World");
  System.out.println("Hello World");
      
```

```// Ruby:```

```
  print "Hello World"
  puts "Hello World"
```


### **- Throw/Catch Exceptions **
```// Java:```

```
  public void methodThatThrows(){
    throw new CustomException("Custom Error");
  }
  
  public void methodThatCatches(){
    try {
        methodThatThrows();
    } catch (CustomException e){
        // handle exception here
    }
  }
      
```

```// Ruby:```

```
  def method_that_throws
    raise CustomError, "Custom Error"
  end
  
  def method_that_catches
    method_that_throws()
    rescue CustomError
        # handle exception here
  end
```
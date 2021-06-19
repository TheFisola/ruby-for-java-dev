# ruby-for-java-dev

#### Showing Ruby syntax and the Java equivalent


**- Variables**


```// Java:```

```
int num = 1;
float numFloat = 1.0;
int[] numArray = {1,2,3};
String text = "Random text";
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
dictionary = {"a" => "b","c" => "d"}
```


Note: From Java 10 local variables can be defined using the 'var' keyword e.g;

```var text = "Random text"```


**- Methods**

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


**- Class**

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

**- Class Inheritance**

```// Java:```

```
public class Dog extends Animal{
}
```

```// Ruby:```

```
class Dog > Animal
end
```

**- Creating Instance of a Class**

```// Java:```

```
Person person = new Person();
```

```// Ruby:```

```
person = Person.new
```


# Ruby-training-session
### Ruby | Operators
An operator is a symbol that represents an operation to be performed with one or more operand
There are different types of operators used in Ruby as follows: 
1. Arithmetic Operators
2. Comparison Operators
3. Logical Operators
4. Assignment Operators
5. Bitwise Operators
6. Ternary Operator
7. Range Operators

### Arithmatic Operators
These are used to perform arithmetic/mathematical operations on operands. 

    Addition(+): operator adds two operands. For example, x+y.
    Subtraction(-): operator subtracts two operands. For example, x-y.
    Multiplication(*): operator multiplies two operands. For example, x*y.
    Division(/): operator divides the first operand by the second. For example, x/y.
    Modulus(%): operator returns the remainder when first operand is divided by the second. For example, x%y.
    Exponent(**): operator returns exponential(power) of the operands. For example, x**y.
Excercises:
##### Addition
puts ("Addition:")
puts (10 + 20)
 
##### Subtraction
puts ("Subtraction:")
puts (40 - 20)
 
##### Division
puts ("Division:")
puts (100 / 20)
 
##### Multiplication
puts ("Multiplication:")
puts (10 * 20)
 
##### Modulus
puts ("Modulus:")
puts (20 % 7)
 
##### Exponent
puts ("Exponent:")
puts (2 ** 4)

### Comparison Operators
Comparison operators or Relational operators are used for comparison of two values. Let’s see them one by one:
 

    1. Equal To(==) operator checks whether the two given operands are equal or not. If so, it returns true. Otherwise it returns false. For example, 5==5 will return true.
    2. Not Equal To(!=) operator checks whether the two given operands are equal or not. If not, it returns true. Otherwise it returns false. It is the exact boolean complement of the ‘==’ operator. For example, 5!=5 will return false.
    3. Greater Than(>) operator checks whether the first operand is greater than the second operand. If so, it returns true. Otherwise it returns false. For example, 6>5 will return true.
    4. Less than(<) operator checks whether the first operand is lesser than the second operand. If so, it returns true. Otherwise it returns false. For example, 6<5 will return false.
    5. Greater Than Equal To(>=) operator checks whether the first operand is greater than or equal to the second operand. If so, it returns true. Otherwise it returns false. For example, 5>=5 will return true.
    6. Less Than Equal To(<=) operator checks whether the first operand is lesser than or equal to the second operand. If so, it returns true. Otherwise it returns false. For example, 5<=5 will also return true.
    7. Combined combination (<=>) operator return 0 when first operand equal to second, return 1 when first operand is greater than second operand, and return -1 when first operator is less than second operand.
    8. Case Equality Operator(===) It will test equality in case statement.
    9. ‘.eql?’ This operator returns true if the receiver and argument have both the same type and equal values.
    
### Excercises:
puts "Equal To Operator:"
puts (10 == 20)
  
puts "Not Equal To Operator:"
puts (40 != 20)
  
puts "Greater than Operator"
puts (100 > 20)
  
puts "Less than Operator"
puts (10  < 20)
  
puts "Less than Equal To Operator"
puts (2  <=  5)
 
puts "Greater than Equal To Operator"
puts (2  >=  5)
  
puts "Combined combination operator"
puts(20 <=> 20)
puts(10 <=> 20)
puts(20 <=> 10)
### Ternary Operator

It is a conditional operator which is a shorthand version of the if-else statement. It has three operands and hence the name ternary. It will return one of two values depending on the value of a Boolean expression. 
Syntax : 
 

condition ? first_expression : second_expression;

#### Excercise: 
 

condition: It be evaluated to true or false.

If the condition is true
 first_expression is evaluated and becomes the result. 

If the condition is false, 
 second_expression is evaluated and becomes the result. 
### Logical Operators
They are used to combine two or more conditions/constraints or to complement the evaluation of the original condition in consideration. They are described below:
 

    Logical AND(&&) operator returns true when both the conditions in consideration are satisfied. Otherwise it returns false. Using “and” is an alternate for && operator. For example, a && b returns true when both a and b are true (i.e. non-zero).
    Logical OR(||) operator returns true when one (or both) of the conditions in consideration is satisfied. Otherwise it returns false. Using “or” is an alternate for || operator. For example, a || b returns true if one of a or b is true (i.e. non-zero). Of course, it returns true when both a and b are true.
    Logical NOT(!): operator returns true the condition in consideration is not satisfied. Otherwise it returns false. Using “not” is an alternate for ! operator. For example, !true returns false.
 ### Bitwise Operators

In Ruby, there are 6 bitwise operators which work at bit level or used to perform bit by bit operations. Following are the bitwise operators : 
 

    1.Bitwise AND (&) Takes two numbers as operands and does AND on every bit of two numbers. The result of AND is 1 only if both bits are 1.
    2. Bitwise OR (|) Takes two numbers as operands and does OR on every bit of two numbers. The result of OR is 1 any of the two bits is 1.
    3. Bitwise XOR (^) Takes two numbers as operands and does XOR on every bit of two numbers. The result of XOR is 1 if the two bits are different.
    4. Left Shift (<<) Takes two numbers, left shifts the bits of the first operand, the second operand decides the number of places to shift.
    5. Right Shift (>>) Takes two numbers, right shifts the bits of the first operand, the second operand decides the number of places to shift.
    6. Ones Complement (~) This operator takes a single number and used to perform complement operation of 8-bit.
  ![image](https://user-images.githubusercontent.com/83069160/166434255-81c59541-fb13-4810-839f-8ecf9c84f120.png)

    https://medium.com/rubycademy/ruby-bitwise-operators-da57763fa368
  ### Operator Precedence
  
  ![image](https://user-images.githubusercontent.com/83069160/166415090-d49ae0dc-fe04-488b-ac59-beae48f36243.png)
  
  ## Blocks
  Block consist of chunks of code.
  A block is always invoked with a function or can say passed to a method call.
  To call a block within a method with a value, yield statement is used.
  Blocks can be called just like methods from inside the method that it is passed to.
  #### Excercise:
    ["Geeks", "GFG", 55].each do |n|   
      puts n   
    end 
### Inline between the curly braces {}

#### Syntax:

block_name { #statements_to_be_executed }

#### Excercise:

 Ruby program to demonstrate the block
 Inline between the curly braces {}
  
 here 'each' is the method name 
 n is the variable
 
["Geeks", "GFG", 55].each {|i| puts i}  

##### Output:.

Geeks
GFG
55

### yeild

The yield statement is used to call a block inside the method using the **yield** keyword with a value
**Note**: Parameters can be passed to the yield statement.
#### Excercise
def shivi
  puts "Inside Method!"
    
    yield "p1"
      
  puts "Again Inside Method!"
    
  yield "p2" 
    
end

shivi{ |para| puts "Inside Block #{para}"}
![image](https://user-images.githubusercontent.com/83069160/166419093-e251c38b-f280-46b1-973e-80351d216796.png)

### Proc Vs Lambda

proc behaves like a block - yield semantics, where as lambda behaves like a method - method call semantics. Also return, break, et
important but subtle difference between procs created with lambda and procs created with Proc.new is how they handle the return statement:

    In a lambda-created proc, the return statement returns only from the proc itself
    In a Proc.new-created proc, the return statement is a little more surprising: it returns control not just from the proc, but also from the method enclosing the proc!

Here's lambda-created proc's return in action. It behaves in a way that you probably expect:

def whowouldwin

  mylambda = lambda {return "Freddy"}
  mylambda.call

  #mylambda gets called and returns "Freddy", and execution
  #continues on the next line

  return "Jason"

end


whowouldwin
#=> "Jason"

Now here's a Proc.new-created proc's return doing the same thing. You're about to see one of those cases where Ruby breaks the much-vaunted Principle of Least Surprise:

def whowouldwin2

  myproc = Proc.new {return "Freddy"}
  myproc.call

  #myproc gets called and returns "Freddy", 
  #but also returns control from whowhouldwin2!
  #The line below *never* gets executed.

  return "Jason"

end


whowouldwin2         
#=> "Freddy"

![image](https://user-images.githubusercontent.com/83069160/166428442-80b4cbd0-a666-465e-9eee-6947979d6cc6.png)


![image](https://user-images.githubusercontent.com/83069160/166428578-75ce2a05-114f-4854-8579-8cbe5185e2b9.png)

##Exception Handling 

SYNTAX:

begin
  CODE THAT MIGHT BREAK THINGS
rescue
    CODE THAT WILL RUN IF THINGS BREAK
end


#### Excercise
1.
def divider(num1, num2)
    begin
      return num1/num2
    rescue
      puts "Zero division error"
    end
end

puts divider(1,0)


2.
def divider(num1, num2)
    begin
      return num1/num2
    rescue
      puts "Zero division error"
    end
end


begin
    puts divider(1,0, 3)
rescue => e
    puts e
end


$e.message
$e.class
$e.backtrace


def string_validator(input)
    if input.class! = String
        raise StandardError, "message"
    end
    return input
end

puts string_validator(9)
puts string_validator("Im string")



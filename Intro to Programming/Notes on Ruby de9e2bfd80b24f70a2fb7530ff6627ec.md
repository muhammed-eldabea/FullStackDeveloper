# Notes on Ruby

# Hello World "

```ruby
p "Hello"       # will print the code to the screen with no formating  >> "Hello" 
print "Hello"   # will print the code to the screen with no formating   >> Hello
puts "Helloo "  # will print the code to the screen with auto formating
```

# Numbers In Ruby

```ruby
p 9/2                 #  output >>  4
p 9/2.5               #  output >>  4.5  
p 1 == 2              #  output >> flase 
p 1||0                #  output >> 1 
p true || false       #  output >> true 
```

# Strings in Ruby

```ruby
puts "Hello".length # to get the length 
#index in string start with 0  
# H[0]   o[4]    
puts "Hello"[0]   #  output will  be << H >>
#contact two string 
"Hello" + " World!" + " ," + "How are you "
```

# Variable In Ruby

```ruby
#we use variable to start data 
#as we know that programming is sabout data manuplation 
#all what we do is that we proccesing data 
var_numType = 45 
var_strType = "Mohammed" 

#variable is not assigned to its type this mean 

data = "mohammed " 
data = 45 
puts data  # output will be 45 

```

## Number operation

```ruby
count = 1  
count +=1  #  equal count = count +1  
#to check if a number is zero 
is_even = count & 0 == 0 # true or false 
 
```

# Method In Ruby

if you get your hand dirty in any programming language before I'm sure you hear about methods or functions in your language : 
they are used to prevent repeat a part of code many times this will reduce the code size but calling a functions or a function many times may lead to some problems like stack overflow as we know all the data in the function including the function parameter are local to the function so they will be stored in the stack  . 

give us the power to reefer to the code many times ant control the internal behavior of the code depending on the parameters we send to it  

 

```ruby
#simple defination of method 
def print_UserName(name) 
puts "Hello" + " " + name
end 

#all what we need to call it is to write it name with a locaal parameters send to it 
print_UserName("Mohammed") 

#outout willbe 
Hello Mohammed 
```

and an example of the behavior  change depending in the local parameters : 

 

```ruby
def select_Hello_masseage(massegeType,name) 
	if (massegeType == 1 ) 
		puts "Helloioa " + name 
	else 
		puts "Hello ! " + name 
	end 
end  

select_Hello_masseage(1,"Mohammed") #output >> Helloioa Mohammed 
select_Hello_masseage(0,"Mohammed") #output >> Hello ! Mohammed 
#we can see that depening on the parameters messageType value the message format will be changed 

```

method also can return data 

```ruby
def Average (num1 , num2) 
	avg = (num1 + num2) / 2 
	return avg 
end 
```
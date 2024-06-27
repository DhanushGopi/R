# R
For the Vasanth


intha da 

#returning value from a function

add = function(a,b)
{
  #body of the function
  #c is a local variable
  #a and b are called the formal parameter
  c = a+b
  return(c)
}

x = 5 #x is an actual parameter
y = 6 #y is an actual parameter
z = add(x,y)
print(paste('X = ', x, 'Y = ', y, 'Sum = ', z), quote=FALSE)

#multi-return statements
# to check the sign of the number

check_sign = function(d)
{
  if (d > 0){
    print("It is positive")
    return("Positive")
  }else if (d < 0){
    print("It is negative")
    return("Negative")
  }else{
    print("It is Zero")
    return("zero")
  }
}

f = as.numeric(n)
outcome = check_sign(f)
print(paste("Sign of the given ", f , " is ", outcome),quote=FALSE)

number1 = readline("Enter the number")
number1 = as.numeric(number1) #convert the character datatype to numeric
print(number1)

# No default arguement

nodisplay = function(h,k)
{
  print(h)
  print(k)
  
}

nodisplay(12,23)

#default arguement

oneval = function(z)
{
  return(z)
}

display = function(f=oneval(13),g=23,l="வண்ணகம்S")
{
  print(f)
  print(g)
  print(l)
  
}
display(g=100,f=14)
display(13)#one argument passed and two default values used.
display(23,24) #two argument passed and one default value used. 
display(1,2,3)#three argument passed and no default value taken.
display() #only default argument and no value passed

#note: if the two variable passed then default arguments will not be used but if the one value is passed the default arguement will be used.
#note: if there n argument in the function there will the n-1 is the default arguemnt
#note: default arguments should be given from right to left and non default arguement should be precieved in the the starting.


#named arguments

display(g=100,f=14) #default arguement can be manipulated by the use  of named arguement.
#we can't use the same named actual arguement for other arguement name in the same function. 
#named arguement can be passed in any order.


#one function calling another function
#solving a problem using functions


#similary write functions for the other arithmetic operator



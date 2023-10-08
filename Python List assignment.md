## Intention of assignment: 
Give students a basic introduction/review of lists in python, but particularly on iterating through a list using for loops. 
At the end, we introduce the list len() method. The assumption for this assignment is that this is going to be one of the first times that students work with lists, which is why it's so simple.
A follow up to this would include things like using list comprehension, using a for loop with range(), and also a for loop with enumerate(). I think it would be more helpful to have students learn this
in the presence of a teacher, which is why they are not included in the assignment.

## Type of assignment: coding exercise. 
In terms of length, I think it could be a bit longer than what I have now, but not so much longer that it becomes "busy work". 
Something like asking students to do practically the same excercise but for a second or third list (list_b or list_c) to give them more practice could be a compromise --
once they've finished the question prompts for list_a, it won't take them too much time or work to complete similar questions and would just end up being more practice for students.

I provided a hint for the first for loop, so that students realize that they will be using for loops. This can be differentiated -- if a class seems to be very advanced, remove the scaffolding, and if a class seems to be
a little slow, we can provided more provided lines of code to scaffold them better.



## Students will be given:
```python

list_a = ["apple", "bannana", "peach", "orange", "watermelon", "cherries"]

#Given this list, answer the following questions:

# print out the list


# print out items in the list, but on a separate line 
for item in list_a:     #hint!


# go through the list and print out "bannana", and nothing else


#what about cherries?


# at this point, the output of your program should look like:
# ["apple", "bannana", "peach", "orange", "watermelon", "cherries"]
# apple
# bannana
# peach
# orange
# watermelon
# cherries
# bannana
# cherries

#Pretend the list you were using was triple or even quadruple it's size.
#can you think of a way to count how many elements are in the list?






# Now that you've done that, uncomment the following code and run it:

#print("The len() method in python returns the number of elements in a list! : " , len(list_a))




```


## Solutions:
```python

list_a = ["apple", "bannana", "peach", "orange", "watermelon", "cherries"]

# print out the list
print(list_a)

# print out items in the list, but on a separate line
for item in list_a:
  print(item)

# go through the list and print out "bannana", and nothing else
for item in list_a:
  if item == "bannana":
    print(item)

#what about cherries?

for item in list_a:
  if item == "cherries":
    print(item)


#Pretend the list you were using was triple or even quadruple it's size.
#can you think of a way to count how many elements are in the list?

#expected answer that most students will produce:
counter = 0  

for item in list_a:
  counter += 1

print(counter)

###### Teacher note -- we expect students to do a for loop since they already did for the questions before
###### Now we can show them len()

print("The len() method in python returns the number of elements in a list! : " , len(list_a))
```

# Animesh2198-Hands-On-Lab-Lists-Python-Basics-
In this repository I have described about python basics (Lists) including indexing, list manipulation, and copy/clone list.

We are going to use a dataset based on a recommendation of an album which consists of the following : 

artist 
album 
released_year
length_min_sec
genre 
music_recording_sales_millions
claimed_sales_millions
date_released 
soundtrack - Indicates if the album is the movie soundtrack (Y) or (N)
rating_of_friends - Indicates the rating from your friends from 1 to 10

Lists 
1) It is a sequenced collection 
2) Contains objects (stings, integer etc. )
3) Index is the address of the object. 
4) Index is used to access the objects present in the list.

Step 1 : create a list -  type the objects in the square brackets [ ]. The string should be inside the parenthesis and integers or float can be written directly objects are seperated by commas 
Ex. - Song = ["Amit Trivedi", 10.1, 2000]
from the above ex. index for "Amit trivedi" is 0, 10.1 is 1 and for 2000 is 2. In python we can assign negative indexing also which will be -3, -2, -1 respectively. 

We can perform nesting in the list. 
Nesting means to add list in a list. 

ex. - Song = ["Amit Trivedi", 10.1, 2000, [1, 2], ("A", 1)]

We can slice list 
ex - song[3:5]

# Use extend to add elements to list

L = [ "Michael Jackson", 10.2]
L.extend(['pop', 10])
L


L = [ "Michael Jackson", 10.2]
L.append(['pop', 10])
L 

The difference between append and extend is that extend will consider number of objects as number of index and append will take the objects as one index. 

Lists are mutable means we can change the objects inside a list. 
A = ["disco", 10, 1.2]
print('Before change:', A)
A[0] = 'hard rock'
print('After change:', A)

We can delete the object present in the list. 
print('Before change:', A)
del(A[0])
print('After change:', A)

We can convert sting into list. Where every character present in the string is seperated by space gets seprated in to list by commas. 
For example - 'hard rock'.split() output - ['hard', 'rock']
 
We use the delimiter (,) to seprate the string. 
for ex - 'A,B,C,D'.split(',') output - ['A', 'B', 'C', 'D']

We can copy/clone list 
A = ["hard rock", 10, 1.2]
B = A
print ("This is the value of A",A)
print ("This is the value of B",B)
 
Out put - This is the value of A ['hard rock', 10, 1.2]
This is the value of B ['hard rock', 10, 1.2]

Here the value of A and B are same. 

If we make a change in the list of A 
for an ex. - 
print("This is the value of B ( index 0 ) before changing the value of index of list B i.e : ", B[0])
A[0] = "Animesh" #Here we are making a change in the list of A in index 0 
print('B[0]:', B[0]) #The changes are made in list A but can be seen in list B  

We can clone the list 
B = A[:]
B
output - ['Animesh', 10, 1.2] 

After making a clone of list B the values are not changed in the list from A to B 
print('B[0]:', B[0])
A[0] = "hard rock"
print('B[0]:', B[0])
Output - The values of B will remain same and will not change if we change the object in A 





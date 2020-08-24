# Data-stuctures
A basic understanding of data structures\ 

## Arrays
I am using swift for the following:

var anArray=[0,3,5,0,7,64,7,8,1,4,0,7,5]
var numOfIndex = anArray.count

// now to get the item at any perticular index
print(anArray[4]) // output should be 7

// if we try and get an index out of bounds we get an index out of bounds error. Program tries to access an index that doesn't exist 
print(anArray[100]) // this will give an error as the given array does not have 100 items

// above we saw that the code will give an error if we try and get the 100th index. but how many indexes are there?

print(numOfIndex) // this will give us the count of all the items in the array, which in this case is 13. 

//Note that it tells us the number of items and not the index, so if there are 13 items in the given array, the index of the last item will be 12 as the index count starts from 0.

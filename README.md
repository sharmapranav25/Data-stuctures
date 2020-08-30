# Data-stuctures
A basic understanding of data structures

## Arrays
### Swift was used for the following:

var anArray=[0,3,5,0,7,64,7,8,1,4,0,7,5]

var numOfIndex = anArray.count

### To get the item at any perticular index
print(anArray[4]) 

output: 7

### If we try and get an index out of bounds we get an index out of bounds error. Program tries to access an index that doesn't exist 
print(anArray[100]) 

output: error as the given array does not have 100 items

### Above we saw that the code will give an error if we try and get the 100th index. but how many indexes are there?
print(numOfIndex) 

this will give us the count of all the items in the array

output: 13
#### Note that it tells us the number of items and not the index, so if there are 13 items in the given array, the index of the last item will be 12 as the index count starts from 0.

### To get the of all the indexes in an array
var sum=0
for i in anArray{
    sum=sum+i
}
print(sum)

output: 111

### To get the average of the sum of all indexes
var avg=sum/numOfIndex
print(avg)

output: 8


## Multidimensional-Arrays
### Javascript was used for the following:

var multiArray=[['dog', 'cat', 'hamster'],['meat','meat','fruit']]

### Assigning row indexes
let petIndex=0
let petFood=1
 
### Assigning all the indexes a variable
let pet1=multiArray[petIndex][0]
let pet2=multiArray[petIndex][1]
let pet3=multiArray[petIndex][2]
let food1=multiArray[petFood][0]
let food2=multiArray[petFood][1]
let food3=multiArray[petFood][2]

### Printing indexes from different rows together
console.log(pet1,'=',food1)
console.log(pet2,"=",food2)
console.log(pet3,"=",food3)

output:
dog = meat
cat = meat
hamster = fruit






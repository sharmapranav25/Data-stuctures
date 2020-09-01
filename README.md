# Data-stuctures
A basic understanding of data structures

## Arrays
### Swift was used for the following:
    
    var anArray=[0,3,5,0,7,64,7,8,1,4,0,7,5]

    var numOfIndex = anArray.count

### To get the item at any perticular index
    print(anArray[4]) 

output: 
   
    7

### Try and get an index out of bounds. Program tries to access an index that doesn't exist 
    print(anArray[100]) 

output: 

    Fatal error: Index out of range

### Number of indexes
    print(numOfIndex) 

this will give us the count of all the items in the array

output: 
    
    13
    
Note that it tells us the number of items and not the index, so if there are 13 items in the given array, the index of the last item will be 12 as the index count starts from 0.

### To get the of all the indexes in an array
    var sum=0
    for i in anArray{
    sum=sum+i
    }
    print(sum)

output: 

    111

### To get the average of the sum of all indexes
    var avg=sum/numOfIndex
    print(avg)

output: 

    8


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


### Updating an item multiArray
    multiArray[petFood][1]='fish'
    let updateFood2=multiArray[petFood][1]
    console.log(pet2,"=",updateFood2)

output: 

    cat = fish

### The Multidimensional Array
    console.log(multiArray)

output:

    [ [ 'dog', 'cat', 'hamster' ], [ 'meat', 'fish', 'fruit' ] ]

## Jagged Arrays
### C# was used for the following:
C# natively differentiates between jagged and multidimentional arrays, which some other languages don't.
    
    using System;

    class Program
    {
        static void Main() {

         int[][] jagged= new int [4][];

         //row 0

         jagged[0]=new int[5];


         jagged[0][0]= 1;

         jagged[0][1]= 10;

         jagged[0][2]= 11;

         jagged[0][3]= 3;

         jagged[0][4]= 8;



         //row 1

         jagged[1]= new int[9];


         //row 2

         jagged[2]= new int[3] {10,20,30};



         //row 4

         jagged[3]= new int[1];

         jagged[3][0]= 100;


         Console.WriteLine("At row 4, col 0: "+jagged[3][0]);
         Console.WriteLine("At row 3, col 3: "+jagged[2][2]);
         Console.WriteLine("At row 2, col 8: "+jagged[1][7]);
         Console.WriteLine("At row 1, col 2: "+jagged[0][1]);


        }

    }

output:
     
    At row 4, col 0: 100
    At row 3, col 3: 30
    At row 2, col 8: 0
    At row 1, col 2: 10
 

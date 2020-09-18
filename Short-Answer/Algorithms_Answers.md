#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) Notation should be O(n^3), The loop is going through n and doing multiple calculations using n.

b) Notation shout be O(n^2), there are 2 loops going through n and two slots of memory being used.

c) Notation should be O(n), the function is reccursively looping though the length of n, with very few other steps

## Exercise II

We first need to find out what f is, and since we dont have technically have to keep the egg safe, we can drop one egg at a time until it breaks. When it does break, we will hae found f.

while x < building.length():
....if egg != broken:
..../....drop_egg()
..../....x += 2
....else:
..../....n = f
..../....break

This solution is assuming that we dont have to get to the end of the building in order to find f. It also allows us to negate if the building length is even or odd by skipping a floor everytime we drop an egg, which lets us minimize the number of broken eggs as well.

Runs with O(log n)

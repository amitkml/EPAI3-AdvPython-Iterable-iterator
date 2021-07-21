# EPAI3-AdvPython-Iterable-iterator

## Iterator and Iterable
Iterable is an object, which one can iterate over. It generates an Iterator when passed to the iter() method. Lists, tuples, dictionaries, strings and sets are all iterable objects. They are iterable containers that you can convert into an iterator.

Note that every iterator is also an iterable, but not every iterable is an iterator. For example, a tuple is iterable, but it is not an iterator. An iterator can be created from an iterable by using the function iter(). Thus, when we pass this tuple to an iter() function, we will get an iterator. Actually, this is possible because the class of an object has a method __iter__, which returns an iterator. 
- An iterator protocol is nothing but a specific class in Python which further has the __iter__()  and __next__()  methods.
    - __iter__() This method returns the iterator object itself as mentioned above.
    - __next__() This method returns the next item from the container. If there are no further items, raise the StopIteration exception. 

![im](https://d1m75rqqgidzqn.cloudfront.net/wp-data/2020/08/28190200/Iterators-in-Python.jpg)

## Project: Description
The starting point for this project is the Polygon class and the Polygons sequence type we created in the previous project.

The code for these classes along with the unit tests for the Polygon class are below if you want to use those as your starting point. But use whatever you came up with in the last project.

## ONLY Goal
Refactor the Polygons (sequence) type, into an iterable. You'll need to implement both an iterable, and an iterator.

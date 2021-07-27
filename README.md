## Collections

Collection refers to a group of objects or values into a single entity

To represent collection in java, Collections framework is used which provides certain classes and interfaces

In brief, a "Collections Framework" is a unified architecture for representing and manipulating collections, enabling collections to be manipulated independently of implementation details.


## Why Collections when we have arrays

We might wonder why to use to collection when we have arrays. Even they can store multiple objects or data as single entity.

There are few limitations with arrays like:

1. Array size is fixed, we cannot change it dynamically
1. It stores only similar data types (of course we have a workaround using object array which stores any value or object we want)
1. They do not have readily available data structure methods like searching largest value, finding a particular value. We have to define them

## Collections Chart

![image](https://github.com/krishna-surisetty/collections_overview/blob/master/collections_actual_chart.PNG)

## Collection Interface and Collections class

While both are from java.util package, Collection is an interface which can be considered as root interface.
The usual interfaces like List, Queue and Set extends this interface
Collections class provide several utility methods (methods which are common, often reused functions) like sort, search etc., which are usually used to operate on a Collection

## Common classes used that implement List, Set and Queue interface

1. List - ArrayList, LinkedList
1. Set - HashedSet, LinkedHashSet
1. Queue - PriorityQuue

## Map interface and why it is different from Collection interface part but part of Collection framework

Map is a special type of interface which stores information in the form of key-value pair which clearly differentiates Map from other Collection types which store each single value.

It makes sense when we think of it in that way. Collection interfaces has add(), remove() methods which take single input which doesn't work for Map and as Collection extends Iterable interface, it has an iterator to iterate over their elements which for Map does not work as it can't have Key iterator and value iterator

To know more about why we use iterator refer to <https://github.com/krishna-surisetty/iterator_design_pattern>
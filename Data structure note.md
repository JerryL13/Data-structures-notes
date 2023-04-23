
## B01

###tuples
- list comprehension: method to concisely create lists 
- allows for 2D arrays and materices efficiently by using fundamental notation 
- use when a new list: is a result of some operation applised to all of its member of another sequence/iterable or an element that satifys a certain condition 
- list comprehension consistr of [] containning an expression, for clause, then a zero or more for or if clauses
- Tuples: Immutable sequenceable data-type object, declared with parenthesis( () is an empty tuple) , they are also sliceable thus meaning they are indexable by using square brackets
- can use built in function like max or min

### Map and Filter
- Map and filter comes from lambda, this will be seen a lot in list comprehension 
- iterator Function: returns an object that is iterable 
- map() -> built in function that applies a given function to every item in the given sequence and returns a result
- filter() -> built in function that filters out items in a sequence would end in true and will return the result 

## B02
- sets: a well_deined collection of distinct objects, considered as an object in its own right. a set can be denoted withg {}
- sets dont need to be ordered {a,b,c} is the same as {b,c,a} they are considered the same 
- sub set: any set whoes its members are elements of another set 
- union: is when two sets get added to make a union(U)
- Intersection: The intersection of set A and B is members that are present in both sets
- Subtraction: it doesn't really exist, The act of A - B results to removing the members that exist in set B from set A.
- Symmetric Difference: Elements that are in either set, BUT they cannot intersect 
- Universe: A set that is defined to contain every possible members, all the values in our data set.
- Complement: A complement of set A will be the set that contain members from the Universe set that doesn’t exist in set A
 
### Sets in Python 3 
- set: an unordered collection with no duplicate elements (Operations; union,intersection, difference, symmetirc difference)

#### List of set built in functiuons 
- # Let s be a set
- len(s) → returns the size of the set
- x in s ; x not in s → membership comparison
- s.isdisjoint(a) → isdisjoint checker
-  s.issubset(a) OR s <= a → subset checker
- s < a → proper subset checker
- s.union(a) OR s | a → union operation
- s.intersection(a) OR s & a → intersection operation
- s.difference(a) OR s - a → difference operation
- s.symmetric_difference(a) OR s ^ a → symmetric difference
- s.copy() → provides a shallow copy

#### built in statments for sets 
- # Let s be a set
- s.add(elem) # adds elem to the set
- s.remove(elem) # removes elem from the set; error if elem DNE
- s.pop() # removes the last element from the set, and returns it (error when set is empty)
- s.discard(elem) # removes elem from the set if elem exists
- s.clear() # empties the set
- DNE → “Does Not Exist”

### set logical properties
- associatitve:If A,B, and C are sets, then the ((A union B) union C) is equal to (A union (B union C))
- distributive law: if A,B, and C are sets, then (A intersection (B union C)) is equal to:
((A intersection B) union (A intersection C))

## BO3
- dictionary: (associative Array, Map, symbol table) stores a collection of keys, each key apppears once in the collection 
- common operation are adding pair's removing pair's, modifying etc.
- useful because the keys don't need to be ordered  
- "dict" create a dictionary by using {} (empty dict)
- our index which are called keys, doesnt need to be ordered 
- keys have a unquie address for an item in a dictionary(must be ummutable, strings numbers etc.), there cannot be two keys with the same value 
- python contains an eddicient key/value "hash table"

####FUNCTIONS AND METHODS
- len(A) # returns the length of dictionary = data set size
- str(A) # returns the dictionary as a string
- type(A) # returns that A is a dict
- # To search for an existing key, we use membership
- x in A # True if x is a key/address in A
- x not in A # True if x is not a key/address in A

- built in functions like A.clear() or A.copy
- A.keys() # Returns a sequence of keys/addresses in A
- A.values() # Returns a sequence of item values in A
- A.items() # Returns a sequence of key,item pairs in A
- A.get(address) # Returns the item value at address
- A.update(B) # Extends A with the dictionary of key,value pairs of B
- del A[address] # deletes the (key,value) object at that location

#### dict() constructor 
- list tuple can be turned to a dictionary item(key value) by using dict()

### examples
students = {} # Empty dictionary

students[‘GWSS01’] = ‘Jake’
students[‘GWSS02’] = ‘Audrey’

# If printed → {'GWSS01': 'Jake', 'GWSS02': 'Audrey'}

marks = dict.fromkeys(students)

print(marks[‘GWSS02’]) # None
marks[‘GWSS02’] = 92
print(marks[‘GWSS02’]) # 92


# List of Data Structures

## Table of Contents

- [List of Data Structures](#list-of-data-structures)
  - [Table of Contents](#table-of-contents)
  - [Preface](#preface)
  - [Data Types](#data-types)
    - [Primitive Types](#primitive-types)
    - [Composite or Non-Primitive Types](#composite-or-non-primitive-types)
    - [Abstract Data Types](#abstract-data-types)
  - [Linear Data Structures](#linear-data-structures)
    - [Arrays](#arrays)


## Preface

This is a cheat-sheat for data structures. I made this for my personal curiosity and usage. I don't know if it's useful for anyone else. All of the data structure and order is taken from [this](https://en.wikipedia.org/wiki/List_of_data_structures) Wikipedia article about data structures. 

I added some short definitions about all of them. *I want to add images and code sniplets* to advance the intelligibility. I did this to see all data structures in one place and quickly look-up.

Most of the data strucures and algorithms textbooks cover basic data structures and their implementations. Also some books cover great amount of them indepth. Here are my favorites:

- **Algorithms** by *Robert Sedgewick*, *Kevin Wayne*
- **Algorithms in a Nutshell** by *George T. Heineman*, *Gary Pollice*, *Stanley Selkow*
- **Grokking Algorithms** by *Aditya Bhargava*
- **Introduction to Algorithms** by *Thomas H. Cormen*, *Charles E. Leiserson*, *Ronald L. Rivest*, *Clifford Stein*
- **The Algorithm Design Manual** by *Steven S. Skiena*
- **The Art of Computer Programming** by *Donald E. Knuth*
- **Advanced Algorithms and Data Structures** by *Marcello La Rocca*
- **Advanced Data Structures** by *Peter Brass*

I hope you like these books and find them useful.

Also i want to implement all of these data structures in several languages. But [The Algotihms](https://the-algorithms.com/) already covers all of them. So my purpose is to implement them for my own development. 

I hope you find this cheat-sheet useful. Feel free to correct my mistakes if you find any and add missing information.

## Data Types

### Primitive Types

- **Boolean**:

    Boolean is a data type that can only be either `true` or `false`.
    
    Booleans are usually used in logical expressions, such as conditions in if-then statements and for loops.

- **Character**:

    Character, char for short, is a data type that can only be a single character. It is usually used to represent a single character in a string. For example, the character `'a'` is a single character string that contains the letter `'a'`. The character `'a'` is also a single character string.

- **Floating-Point Numbers**:

    Floating-point data types are used to store real numbers with a decimal point.

    There are two types of floating-point numbers:
    - **Single-precision**:
        - `float`: 32-bit floating-point number.
        
        Single-precision floating-point numbers are 32-bit floating-point numbers.
        
    - **Double-precision**:
        - `double`: 64-bit floating-point number.

        Double-precision floating-point numbers are 64-bit floating-point numbers.
    
    Single precision floating-point numbers are used when the precision of the number is not important and there is a need for fast calculations.

    On the other hand, double precision floating-point numbers are used when the precision of the number is important and there is a need for accurate calculations.

- **Fixed-Point Numbers**:

    Fixed-point data types are used to store real numbers with a fixed number of decimal places.

    A fixed-point number is a data type that can be used to store any real number, but only in a limited range.

- **Integer**:

    Integer is a data type that can only be a whole number.
    
    Integers are usually used to store the number of items in a collection, or the number of times a loop will be executed.

- **Pointer (Reference)**:

    Pointer (reference) is a data type that can be used to store a memory address.
    
    A memory address is a number that represents the location of a memory location in memory.

- **Enumerated**:

    Enumerated is a data type that can only be one of a set of predefined values.
    
    Enumerated data types are used to store a value that is one of a set of predefined values.
    
    For example, the enumerated data type `Days_of_the_Week` can only be one of the seven days of the week: `'Monday'`, `'Tuesday'`, `'Wednesday'`, `'Thursday'`, `'Friday'`, `'Saturday'`, and `'Sunday'`.

- **Date & Time**:

    Date and time data type is a data type that stores date and time values.

    The date and time data type is used to store a range of values from January 1, 1970 to December 31, 9999.

    It also has the ability to store fractional seconds for the end of each day.

### Composite or Non-Primitive Types

- **Array**<a id="array" name="array"></a>:

    An array is a data type that can store a collection of data.
    
    Array stores the date in an ordered sequence. Each datum in the array is called an element and each element has a unique index.

    The index of an element in an array is called its position.

    The index of the first element in an array could be 0 or 1, and the type of the elements must ot mustn't be the same based on the language.

    Also array elements stored in the memory in **contiguous memory locations**. This means that the elements are stored in order and there is no gap between them.
    
    <a id="dynamic-array" name="dynamic-array"></a>
    
    An array could be `static` or `dynamic`. *Static* arrays are created at compile time and *dynamic* arrays are created at run time. Difference between *static* and *dynamic* arrays is that *static* arrays could store fixed number of elements and *dynamic* arrays could store unlimited number of elements theoroticly. But each time the *dynamic* array reached its maximum capacity, a new memory location is allocated to store the new elements and all the old elements are copied to the new memory location.

- **Structure (Record)**:

    A record, structure or struct for short is a collection of data that is used to store data. Record is a collection of fields, possibly of different data types, typically in a fixed number and sequence.

    The fields of a record are called members and the members are accessed by name.

    Size of the memory block that stores the record is the **sum of the sizes of all the members**.

- **Union**:

    A union is a value that may have any of several representations or formats within the same position in memory.

    The union data type is used to store data that can be of different types. 

    A union can be pictured as a chunk of memory that is used to store variables of different data types. 
    
    Once a new value is assigned to a field, the existing data is overwritten with the new data. 
    
    The memory area storing the value has no intrinsic type, but the value can be treated as one of several abstract data types, having the type of the value that was last written to the memory area.

    Size of the memory block that stores the union is the size of the **largest member**.

### Abstract Data Types

- **Container**:

    A container or collection is a data type that can store a collection of data. 

    - **Lineer Containers**:
        - `List`
        - `Stack`
        - `Queue`
        - `Priority Queue`
        - `Double-Ended Queue`
        - `Double-Ended Priority Queue`
    
    - **Associative Containers**:
        - `Set`
        - `Multi-Set (Bag)`
        - `Map (Associative Array)`

- **List**:

    List or squence is a dynamic data type that can store a collection of data in a linear order.

    The elements of a list are called nodes and the nodes are linked together to form a chain.

    The first node in the list is called the head and the last node in the list is called the tail.

    A list could be used like an `array` but the main differences between them are the following:
    - The elements of a list are **not stored** in *contiguous memory locations*.
    - List is not fixed in size.
    - The elements in the list can be added and removed at any position.

- **Tuple**:

    Tuple is a finite collection of data that is used to store a collection of data in a fixed number and sequence.

- **Map (Associative Array)**:

    A map, associative array, symbol table, or dictionary is a data type that can store a collection of data in a key-value pair.

    The key is used to access the value and each **key has to be unique**.

    Also each key can **have only one value**.

- **Multimap**:

    A Multimap, multihash, multidict or multidictionary is a data type that can store a collection of data in a key-value pair.

    It is a generalization of the map data type. With multimap **more than one value** may be associated with and returned for a given key.

    The key is used to access the value or values and each key has to be unique.

- **Set**:

    A set is a data type that can store a collection of data in a unordered sequence that does **not allow duplicates**.

    Some sets are desigend to be *static* or *frozen* and cannot be modified at runtime. Frozen sets are also called *immutable* sets and they only allow querying operations.

    Other types of sets are called *dynamic* or *mutable* sets and they allow adding and removing elements.

- **Multiset (Bag)**:

    A multiset or bag is a data type that can store a collection of data in a unordered sequence, like a set, that **allows duplicates**.

- **Stack**:

    A stack is a data type that can store a collection of data in a linear order.

    It is a list-like structure in which elements may be inserted or removed from only one end.

    Stack is a **LIFO** *(Last In First Out)* data structure. The last element added to the stack is the first element to be removed.

    It has 2 main and 1 additional operations:
    - **`Push`**: Adds an element to the top of the stack.
    - **`Pop`**: Removes the top element from the stack.
    - **`Peek`**: Returns the top element from the stack.

- **Queue**:

    A queue is a data type that can store a collection of data in a linear order.

    It is a list-like structure in which elements are inserted only at one end, and removed only from the other one end.

    Queue is a **FIFO** *(First In First Out)* data structure. The first element added to the queue is the first element to be removed.

    The beginning of the queue is called the *head* and the end of the queue is called *back*, *tail* or *rear*.

- **Double-ended queue**:

    A double-ended queue or *deque* is a data type that can store a collection of data in a linear order.

    It is a generalization of the queue data type. It allows adding and removing elements from both ends of the queue.

- **Graph**:

    A graph is a data type that used to show the relationship between two or more objects. Graph is collection of nodes that have data and are connected to other nodes.

    A graph consists of a finite set of vertices, *nodes*, together with a set of unordered pairs of these vertices, *edges*, for an undirected graph or a set of ordered pairs for a directed graph.

    A graph is defined with its vertices and edges; 
    $$ G = (V, E) $$
    where V is the set of vertices and E is the set of edges.

## Linear Data Structures

A data structure said to be linear if its elements are stored in a sequential order.

### Arrays

- **Array**:

    Go to the [Array](#array) section.

- **Bit Array**:

    A bit array, bit map, bit set, bit string or bit vector is an array that compacly stores a set of bits.

- **Bit Field**:

    A bit field is an array of bits that each bit or group of bits has a specific purpose. A bit field is used to store data in a compact way.

    The most known bit field is the flag registers in the CPU.

- **Bitboard**:
  
    A bitboard is a special type of bit array that used in games like chess. Bitboard represents the game board where each bit represents a square or a piece. This allows parallel bitwise operations to set or query the game state, or determine moves or plays in the game.

- **Bitmap**:

    A bitmap is a bit array that is used to store a set of bits. It is a representation in which each item corresponds to one or more bits of information, especially the information used to control the display of a computer screen.

- **Circular Buffer**:
  
    A circular buffer, circular queue, cyclic buffer or ring buffer is uses a single, fixed-size buffer(temprory memorry area) as if it were connected end-to-end.

    It is a **FIFO** data structure that is full when the last element is inserted and the first element is removed.

- **Control Table**:

    *TODO*

- **Image**:
  
    *TODO*

- **Dope Vector**:

    Dope vector is a data structure to store information about a set of objects. It is commonly used by compilers to store metadata about the objects such as arrays like length, type and capacity.

    Dope vectors help compilers to access the arrays with ease.

    Different controls such as out of bound and insertion type made thanks to dope vectors.

- **Dynamic Array**:

    Dynamic array, growable array, resizable array, dynamic table, mutable array, or array list. Go to the [Dynamic Array](#dynamic-array) section.

- **Gap Buffer**:

    *TODO*

- **Hashed Array Tree**:

    *TODO*

- **Lookup Table**:

    *TODO*

- **Matrix**:

    *TODO*

- **Parallel Array**:

    *TODO*

- **Sorted Array**:

    *TODO*

- **Sparse Matrix**:

    *TODO*

- **Iliffe Vector**:

    *TODO*

- **Variable-length Array**:

    *TODO*

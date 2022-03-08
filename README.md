```
                                      _(_)_                          wWWWw   _
                          @@@@       (_)@(_)   vVVVv     _     @@@@  (___) _(_)_
 |  __ \        | |      @@()@@ wWWWw  (_)\    (___)   _(_)_  @@()@@   Y  (_)@(_)
 | |__) |__ _ __| |       @@@@  (___)     `|/    Y    (_)@(_)  @@@@   \|/   (_)\
 |  ___/ _ \ '__| |        /      Y       \|    \|/    /(_)    \|      |/      |
 | |  |  __/ |  | |     \ |     \ |/       | / \ | /  \|/       |/    \|      \|/
 |_|   \___|_|  |_|     \\|//   \\|///  \\\|//\\\|/// \|///  \\\|//  \\|//  \\\|//
```


- [1. Hello World](#1-hello-world)
- [2. Perl scripts](#2-perl-scripts)
- [3. Variables](#3-variables)
  - [3.1. Scalar data](#31-scalar-data)
  - [3.2. List data](#32-list-data)
  - [3.3. Scalar variables](#33-scalar-variables)
  - [3.4. Array variables](#34-array-variables)
  - [3.5. Hash variables](#35-hash-variables)
  - [3.6. Variable declaration syntax](#36-variable-declaration-syntax)
    - [3.6.1. Scalar variable declaration](#361-scalar-variable-declaration)
    - [3.6.2. Array variable declaration](#362-array-variable-declaration)
    - [3.6.3. Hash variable declaration](#363-hash-variable-declaration)
- [4. Variable operations](#4-variable-operations)
  - [4.1. Scalar variables](#41-scalar-variables)
    - [4.1.1. Accessing data from scalar variables](#411-accessing-data-from-scalar-variables)
    - [4.1.2. Modifying data in scalar variables](#412-modifying-data-in-scalar-variables)
    - [4.1.3. Inserting data in scalar variables](#413-inserting-data-in-scalar-variables)
  - [4.2. Array variables](#42-array-variables)
    - [4.2.1. Accessing data from array variables](#421-accessing-data-from-array-variables)
    - [4.2.2. Inserting data in array variables](#422-inserting-data-in-array-variables)
    - [4.2.3. Removing data from array variables](#423-removing-data-from-array-variables)
    - [4.2.4. Modifying data in array variables](#424-modifying-data-in-array-variables)
  - [4.3. Hash variables](#43-hash-variables)
    - [4.3.1. Accessing data from hash variables](#431-accessing-data-from-hash-variables)
    - [4.3.2. Inserting data in hash variables](#432-inserting-data-in-hash-variables)
    - [4.3.3. Updating data in hash variables](#433-updating-data-in-hash-variables)
    - [4.3.4. Deleting data from hash variables](#434-deleting-data-from-hash-variables)
    - [4.3.5. Undefining Hash elements](#435-undefining-hash-elements)
  - [4.4. Nested data](#44-nested-data)
    - [4.4.1. References](#441-references)
    - [4.4.2. Anonymous arrays and hashes](#442-anonymous-arrays-and-hashes)
    - [4.4.3. Dereferences](#443-dereferences)
- [5. Context](#5-context)
  - [5.1. Arithmetic context and operation](#51-arithmetic-context-and-operation)
  - [5.2. String context and operation](#52-string-context-and-operation)
  - [5.3. Boolean Context](#53-boolean-context)
  - [5.4. Scalar Context](#54-scalar-context)
    - [5.4.1. Example](#541-example)
  - [5.5. List Context](#55-list-context)
    - [5.5.1. Examples](#551-examples)
  - [5.6. Void context](#56-void-context)
- [6. Flow Controls](#6-flow-controls)
  - [6.1. Conditionals](#61-conditionals)
    - [6.1.1. Boolean values](#611-boolean-values)
    - [6.1.2. Comparisons](#612-comparisons)
      - [6.1.2.1. Arithmetic comparisons](#6121-arithmetic-comparisons)
      - [6.1.2.2. String comparisons](#6122-string-comparisons)
    - [6.1.3. Logical operators](#613-logical-operators)
    - [6.1.4. ```if```, ```if```...```else```, ```if```...```elsif```](#614-if-ifelse-ifelsif)
    - [6.1.5. ```unless```](#615-unless)
    - [6.1.6. Postfix](#616-postfix)
    - [6.1.7. Ternary operator](#617-ternary-operator)
    - [6.1.8. Short-circuit](#618-short-circuit)
      - [6.1.8.1. Example](#6181-example)
    - [6.1.9. Hash Examples](#619-hash-examples)
    - [6.1.10. Array Examples](#6110-array-examples)
  - [6.2. Loops](#62-loops)
    - [6.2.1. Condition controlled loop](#621-condition-controlled-loop)
    - [6.2.2. list controlled loop](#622-list-controlled-loop)
    - [6.2.3. Count-controlled loop](#623-count-controlled-loop)
    - [6.2.4. Loop within loop](#624-loop-within-loop)
    - [6.2.5. Loop control](#625-loop-control)
      - [6.2.5.1. Label](#6251-label)
      - [6.2.5.2. ```next```](#6252-next)
      - [6.2.5.3. ```last```](#6253-last)
      - [6.2.5.4. ```redo```](#6254-redo)
    - [6.2.6. Topic](#626-topic)
    - [6.2.7. Postfix](#627-postfix)
    - [6.2.8. ```continue```](#628-continue)
- [7. Subroutines](#7-subroutines)
  - [7.1. argument variable ```@_```](#71-argument-variable-_)
  - [7.2. ```return```](#72-return)
  - [7.3. Passing arguments](#73-passing-arguments)
  - [7.4. Pass by Reference](#74-pass-by-reference)
- [8. Package](#8-package)
- [9. Special subroutines - ```BEGIN```, ```END```, ```CHECK``` and ```INIT```](#9-special-subroutines---begin-end-check-and-init)
  - [9.1. ```BEGIN```](#91-begin)
  - [9.2. ```CHECK```](#92-check)
  - [9.3. ```INIT```](#93-init)
  - [9.4. ```END```](#94-end)
- [10. Modules](#10-modules)
- [11. Variable scope](#11-variable-scope)
- [12. CPAN](#12-cpan)
- [13. Input and output](#13-input-and-output)
  - [13.1. Command input](#131-command-input)
  - [13.2. Read from file](#132-read-from-file)
  - [13.3. Exception handling in Files](#133-exception-handling-in-files)
  - [13.4. Command line arguments](#134-command-line-arguments)
  - [13.5. Input Filenames in command line](#135-input-filenames-in-command-line)
  - [13.6. Writing into files](#136-writing-into-files)
  - [13.7. Reading from STDIN](#137-reading-from-stdin)
- [14. List operations - map, grep, sort](#14-list-operations---map-grep-sort)
- [15. Regex](#15-regex)
- [16. Importing subroutines](#16-importing-subroutines)
- [17. File and Directory management](#17-file-and-directory-management)
- [18. Process management](#18-process-management)
- [19. Object Oriented Programming](#19-object-oriented-programming)
- [20. Debugging](#20-debugging)
- [21. Idioms](#21-idioms)
- [22. Tail calls](#22-tail-calls)
- [23. some cool programs](#23-some-cool-programs)

# 1. Hello World
- Run perl in the command line

    ```perl
    perl -e 'print "Hello World\n"'
    ```

# 2. Perl scripts
- Scripts have extension *.pl*
- use pragmas to force us to write good code and also get info about how we can correct errors
    ```perl
    use strict;
    use warnings;
    use diagnostics;
    ```

- force the script to run on specific version
    ```perl
    use v5.16;
    ```

- Put comments in the file using #. There is no block comment syntax
    ```perl
    # comment
    ```

- print data using ```print``` or ```say``` functions
  - ```say``` appends a new line at the end, ```print does not```
    ```perl
    print("hello");
    say("Hi");
    # we can skip the parentheses for function calls
    print "hello";
    say "Hi";
    ```

- Run the script using
    ```bash
    perl scriptname.pl;
    perl scriptname.pl [arg0 [arg1 [arg2 ...]]]
    ```

# 3. Variables
- variables are used to hold value
- A variable may hold 
  - an individual item or 
  - a ordered list of items or 
  - unordered set of key-value pairs or
  - *undef* - represents an unassigned, undefined, and unknown value

## 3.1. Scalar data
- a scalar a single unit of data
- a single unit of data can be:
  - a number - 4
  - a string - "4", '4'
  - a reference to another variable

## 3.2. List data
- a list is collection of scalar values
- Comma and parentheses are used to define a list
- Examples:<br>
    ```perl
    (); #empty list
    (1, 2, 3); #list of three numbers
    ('bright', "lights", "big", "city"); #list of strings
    (99, "red", "balloons"); #list of mixed data
    (1..10); # list of sequence from 1 to 10
    (1) x 10; # a list of 10 1s i.e. (1,1,1,1,1,1,1,1,1,1)
    ```
- a list of strings can also be created using qw function<br>
  ```qw(red green blue)``` is same as ```('red', 'green', 'blue')```
- Instead of comma *,*, we can use fat comma *=>* to make lists<br>
  ```("roses" => "red", "violets" => "blue")```
- lists cannot be nested
  - if a list is put inside another list, the internal list is automatically flattened and a single long list is created

## 3.3. Scalar variables
- scalar variable can contain scalar data
  - number
  - string
  - reference to another variable<br>
- the same scalar variable can hold a string and later hold a number
- Perl internally infers whether the data is string or number
- if the string is created with single quotes, then the 
*Examples are provided later*

## 3.4. Array variables
- array variable is a list of scalars
- individual data is addressed by an index
  - indexes are integers
  - the index starts at 0

*Examples are provided later*

## 3.5. Hash variables
- hash variables store key-value pairs
- scalar values are mapped to strings key
- individual *values*(data) are addressed by a *key*
  - keys are strings
  - keys are unique
- Using keys, we can retrieve the mapped value stored in Hash

*Examples are provided later*

## 3.6. Variable declaration syntax
- every variable has a sigil associated with it. 
  - Sigils can be one of ($@%)
  - sigils help differentiate between a noun and a verb in our code.
  - sigils help define how a variable must behave according to context.<br>
    *More on that later.*
- variables are declared as ```my <sigil><variable_name>;```
  - variables are given the default value of *undef*
- variables can be also be assigned values as ```my <sigil><variable_name>```;
- variables must start with a number or underscore
- We do not need to specify the data type of a variable 

### 3.6.1. Scalar variable declaration
- $ is sigil for scalar variable
- scalar variables are declared as ```my $<variable_name> = <value>;```
  - if no value is provided, i.e. ```my $<variable_name>;```, then ```undef``` is assigned
    - undef means no value or null or absence of value
  
  
  <br>
- Examples:
```perl
my $scalar_integer = 1; # Integer
my $scalar_float = 1.001; # Floating point number
my $scalar_neg = -1; # negative integer
my $scalar_string = 'Roses are Red'; # string

my $scalar_variable = "Violet is Purple"; # variable is assigned a string
$scalar_variable = 123; # variable now holds a number

my $scalar_undef; # variable has undef
my $scalar_undef2 = undef; # variable has undef

```

### 3.6.2. Array variable declaration
- @ is sigil for array variable
- array variables are declared as ```my @<variable_name> = <list>```
  - it expects a list as value
  - if no value is provided, i.e. ```my @<variable_name>;``` 
    - an empty list is assigned

  <br>
- Examples
```perl
my @array_int = (1,2,3);
my @array_str = qw(roses are red);
my @arr_mix = (221, 'B', 'Baker', 'Street');
```

### 3.6.3. Hash variable declaration
- % is the sigil for hash variables
- hash variables are declared as ```my %<variable_name> = <list>```
  - if no value is provided, i.e. ```my %<variable_name>;``` 
    - an empty list is assigned

- Examples
```perl 
my %hash = ('roses', 'red', 'violets', 'blue'); # this will map roses with red and violets with blue
my %hash2 = ('roses' => 'red',
             'violets' => 'blue'); # uses fat comma. this will map roses with red and violets with blue
my %hash3 = qw(roses red violets blue sunflower yellow);
my %hash4 = %hash3{'roses', 'violets'}; # create hash from another hash

```

# 4. Variable operations
## 4.1. Scalar variables

### 4.1.1. Accessing data from scalar variables

- printing a scalar variable - 
    ```perl 
    print $scalar_var;
    ```

### 4.1.2. Modifying data in scalar variables
    
  ```perl
  my $number1 = 12;
  $number1 = 10;
  ```

### 4.1.3. Inserting data in scalar variables
```perl
my $variable; # undef assigned to $variable
$variable = 23;
```

## 4.2. Array variables

### 4.2.1. Accessing data from array variables
- printing first element of array
    ```perl
    print $arr_var[0];
    ```
&emsp;&emsp;&emsp;*Since we are accessing a scalar data from array(which is a collection of scalar data), we use the sigil $*

- printing last element of array
    ```perl
    print $arr_var[-1];
    print $arr_var[$#arr_var]; # $#variable_name returns the index of the last element
    ```
- printing second last element of array - 
    ```perl
    print $arr_var[-2]
    ```
- printing full array
    ```perl
    print @array;
    ```
- accessing the first 3 elements of array
    ```perl 
    print @array[0..2];
    ```
- accessing the 2nd, 3rd, 5th and 8th element - 
    ```perl
    print @arr[(1,2,4,7)];
    # OR
    my @idx = (1,2,4,7);
    print @arr[@idx];
    ```

### 4.2.2. Inserting data in array variables
- Perl function ```unshift``` inserts scalar data or list at the start of the list
  - syntax - ```unshift(@array, list)```
- Perl function ```push``` inserts scalar data or list at the end of the list
  - syntax - ```push(@array, list)```
- Perl function ```splice  ``` can be used to insert data in the middle of list
  - syntax ```splice(@array, index, length, replacement_list)```

- Inserting a scalar data to the start of array
    ```perl
    my @arr = (8..11);
    my $item_to_be_inserted = 99;
    unshift @arr. $item_to_be_inserted;
    ```
- Inserting a list of data to start of array 
    ```perl
    my @arr = (8..11);
    unshift @arr, (2,4,4,1,1,3,9);
    ```
- Inserting items of an array variable to the start of array
    ```perl
    my @arr = (8..11);
    my @arr2 = ('a'..'d');
    unshift @arr, @arr2;
    ```

- Inserting a scalar data to the end of array
    ```perl
    my @arr = (8..11);
    my $item_to_be_inserted = 99;
    push @arr. $item_to_be_inserted;
    ```
- Inserting a list of data to end of array 
    ```perl
    my @arr = (8..11);
    push @arr, (2,4,4,1,1,3,9);
    ```
- Inserting items of an array variable to the end of array
    ```perl
    my @arr = (8..11);
    my @arr2 = ('a'..'d');
    push @arr, @arr2;
    ```
- Inserting data in the middle of array
    ```perl
    my @arr = (1,2,3,4);
    splice @arr, 1, 0, 'Test'; # @arr will now have (1, Test, 2, 3, 4)


- Inserting Item two or more locations after the end of string
    ```perl
    my @arr = (1,2,3);
    $arr[5] = 6; # array will be (1,2,3,undef, undef, 6)
    ```

### 4.2.3. Removing data from array variables
- Perl function ```shift``` removes items from start of the list
  - syntax - ```shift(@array);```
- Perl function ```pop```  items from end of the list
  - syntax - ```pop(@array);```
- Perl function ```splice``` can be used remove data from the middle of list
  - syntax ```splice(@array, index, length, replacement_list)```
  
- Removing a scalar data at the start of array
    ```perl
    my @arr = (8..11);
    my $data_removed = shift @arr; # $data_removed = 8 and @arr = (9,10,11)
    ```
- Removing a scalar data at the end of array
    ```perl
    my @arr = (8..11);
    my $data_removed = pop @arr; # $data_removed = 11 and @arr = (8,9,10)
    ```
- Removing 1 data from the middle of array
    ```perl
    my @arr = (1,2,3,4,5);
    my $index = 2;
    splice(@arr, $index, 1);; # @arr will now have (1, 2, 4, 5)
    ```
- Removing data from 3rd element to last
    ```perl
    my @arr = (1,2,3,4,5);
    my $index = 2;
    splice(@arr, $index);; # @arr will now have (1, 2)
    ```

### 4.2.4. Modifying data in array variables

- modify data at a specific index
    ```perl
    my @arr = qw(roses red violets blue);
    $arr[2] = 'sky'; # @arr = ('roses'. 'red'. 'sky'. 'blue')
    ```
- modify multiple records at different locations
    ```perl
    my @arr = (0,1,2,3,4,5,6,7,8,9,10,11);
    my @idx = (1,2,3,5,8); # list of indexes where data needs to be modified    
    my @val = qw(a b c d e); # list of values to be put
    @arr[@idx] = @val; # @arr = (0,a,b,c,4,d,6,7,e,9,10,11)
    ```
- replace 2nd and 3rd elements with 5 elements
    ```perl
    my @arr = (0..5); # @arr = (0,1,2,3,4,5)
    my @val = qw(a b c d e);  
    splice(@arr,1,2,@val); # @arr = (0,a,b,c,d,e,3,4,5)
    ```

- clearing up an array
    ```perl
    my @arr = (0..5); # @arr = (0,1,2,3,4,5)
    @arr = ();
    ```

## 4.3. Hash variables

### 4.3.1. Accessing data from hash variables

- Accessing value using a key
  - to access data associated with a key, we need to 
    - prefix the variable with $ sigil
    - place the key in braces {}
      - ```print $hash_variable{"key"};```


    ```perl
    my %flowers = ("roses"=>"red");
    say $flowers{"roses"}; # red is printed
    say $flowers{roses}; # quotes are not necessary for single word keys
    ```

- Accessing slices
  - to access the values associated with multiple keys in a single statement, we need to
    - prefix the variable with @ sigil. This is because we are trying to retrieve a list of data.
    - place the array of keys in braces {}
      - ```print @hash_variable{@array_of_keys};```
    ```perl
    my %flowers =                      
            ("roses" => "red", 
             "violets" => "blue",
             "sunflower" => "yellow");
    my @array_of_keys = qw(roses violets);
    say "@flowers{@array_of_keys}";
    ```


- Getting list of keys
  - to get the list of all the keys in hash use ```keys``` function
  - the keys will not be maintainted by Perl in the same order in which they were inserted. The key order is determined by Perl to facilitate quick access.
    ```perl
    my %flowers =                      
        ("roses" => "red", 
         "violets" => "blue",
         "sunflower" => "yellow");
    my @array_of_keys = keys %flowers;
    say "@array_of_keys";
    ```

- Getting list of values
  - to get the list of all the values in hash use ```values``` function
  - the keys will not be maintained by Perl in the same order in which they were inserted. The key order is determined by Perl to facilitate quick access.
    ```perl
    my %flowers =                      
        ("roses" => "red", 
         "violets" => "blue",
         "sunflower" => "yellow");
    my @array_of_values = values %flowers;
    say "@array_of_values";
    ```

### 4.3.2. Inserting data in hash variables
- to insert a key-value pair in an existing hash, we need to 
  - prefix the variable with $ sigil
  - place the key in curly braces {} 
  - place the value after the =
    - ```$hash_variable{"key"} = value```

- Inserting a new key-value pair
    ```perl
    my %flowers = ("roses"=>"red");
    $flowers{violets} = "blue";
    say $flowers{roses}; # prints red
    say $flowers{violets}; # prints blue
    ```

- mapping a set of new keys to new values
  - to insert multiple pairs
    - prefix the hash variable with @
    - place the list of keys in curly braces {}
    - place the list of values after the =
      - ```@hash_variable{@array_of_keys} = @array_of_values```
  
    ```perl
    my %flowers = ("roses"=>"red");    
    my @keys = ('violets', 'sunflower');    
    my @values = ('blue', 'yellow');    
    @flowers{@keys} = @values;     
    say $flowers{roses}; # prints red    
    say $flowers{violets}; # prints blue    
    say $flowers{blue}; # prints yellow 
    ```
  
- merging one hash into another
    ```perl
    my %flowers =
        ("roses" => "red", 
         "violets" => "blue",
         "sunflower" => "yellow");
    my %other_flowers =
        ("Marigold" => "Orange",
         "Carnation" => "Pink",
         "Iris" => "Purple");

    @flowers{keys %other_flowers} = values %other_flowers;
    say $flowers{Iris}; # prints Purple
    ```

### 4.3.3. Updating data in hash variables
- To update the value of a pair
  - prefix the variable with $ sigil
  - place the key in curly braces {} 
  - place the value after the =
    - ```$hash_variable{"key"} = value```

    *This is same as inserting new key-value pair. Only only difference is that the key already present in the hash*

    ```perl
    my %flowers =                      
        ("roses" => "red", 
         "violets" => "blue",
         "sunflower" => "yellow");
    $flowers{roses} = "white"; # roses are now of color white
    ```
### 4.3.4. Deleting data from hash variables
- To remove a key value pair from a hash use the ```delete``` function. 
  - Syntax - ```delete $hash_variable{key};```

    ```perl
    my %flowers =    
        ("roses" => "red", 
         "violets" => "blue",
         "sunflower" => "yellow");
 
    delete $flowers{roses}; # roses => red deleted from hash 
    ```

- To empty the whole hash
    ```perl
     my %flowers =
        ("roses" => "red",
         "violets" => "blue",
         "sunflower" => "yellow");
    
    %flowers = (); # hash is emptied
    ``` 

### 4.3.5. Undefining Hash elements 
- To undef a value associated to a key, use the ```undef``` function. 
  - Syntax - ```undef $hash_variable{key};```

    ```perl
    my %flowers =    
        ("roses" => "red", 
         "violets" => "blue",
         "sunflower" => "yellow");
 
    undef $flowers{roses}; # roses => undef 
    ```
## 4.4. Nested data

### 4.4.1. References
- arrays cannot contain other arrays as elements
- hashes cannot contain other hashes as elements
- arrays and hashes can only contain scalars
- Perl reference is a scalar data type that holds the memory address of another value
  - value can be a scalar, array or hash
- Within an array, we can put the reference to other multiple arrays. This way we can have an array of arrays.
  - Same can be done with hashes
  - Also, arrays can have references to hashes and vice versa

- A reference is created using a backslash
  - syntax 
    ```\<sigil><variable>;```

  - Example:
    ```perl
    # scalar holding reference to scalar    
    my $flower = "rose";    
    my $ref_to_flower = \$flower; # $ref_to_flower holds the address of $flower    
    
    # scalar holding reference to array    
    my @numbers = (1..10);    
    my $ref_to_numbers = \@numbers; # $ref_to_numbers holds the address of @numbers    
    
    # scalar holding reference to hash    
    my %flower_color = ("roses" => "red" , "violets" => "blue");
    my $ref_to_flower_color = \%flower_color; # $ref_to_flower_color holds the address of %flower_color    
    
    # array holding reference to scalar    
    my @book = (1);    
    my $first_line = "roses are red";    
    $book[1] = \$first_line; # $book[1] holds the address of $first_line    
    
    # array holding reference to array    
    my @array_rose = qw(roses are red);    
    my @array_violet = qw(violets are blue);    
    my @rhymes = (\@array_rose, \@array_violet); # @rhymes holds address of array_rose and array_violet    
    
    # array holding reference to hash    
    my %flower_prices = ("roses" => "5", "violets" => 3);      
    my %flower_count = ("roses" => "20", "violets" => 18);      
    my @flower_box = (\%flower_prices, \%flower_count); # @flower_box will have reference to %flower_prices and %flower_count    
    
    # hash holding reference to scalar    
    my $yellow_flowers = "Sunflower, Daffodils";    
    my %colored_flowers = ("yellow" => \$yellow_flowers); # reference to $yellow_flowers is stored in hash    
    
    # hash holding reference to array    
    my @red_flower_list = qw(roses chrysanthemum amaryllis);    
    my @white_flower_list = qw(camellia bouvardia magnolia);    
    my %flower_by_color = ("red" => \@red_flower_list, "white" => \@white_flower_list); # reference to @red_flower_list and @white_flower_list is stored in hsah %flower_by_color    
    
    
    # hash holding reference to hash    
    my %summer_flower_color = ("poppy" => "red", "salvia" => "blue");    
    my %fall_flower_color = ("camellia" => "white", "dianthus" => "pink");    
    my %seasonal_flowers = ("summer" => \%summer_flower_color, "fall" => \%fall_flower_color); # reference to %summer_flower_color and %fall_flower_color is saved 
    ```

### 4.4.2. Anonymous arrays and hashes
- In our earlier examples, in order to put an array/hash in a hash or an array, we followed the following steps:
  - assign a list to an array/hash variable
  - insert the reference of the array/hash variable into another array or hash
- We can skip the step of assigning a list to an array/hash variable
  - We can create a reference to an unnamed anonymous array or an anonymous unnamed hash
    - a reference to anonymous array can be created using [] operators
    - a reference to anonymous hash can be created using {} operators

  ```perl
  # array holding reference to anonymous arrays
  my @rhymes = (['roses', 'are', 'red'], ['violets', 'are', 'blue']);

  # array holding reference to anonymous hashes
  my @flower_box = ( 
                    {"roses" => "5", "violets" => 3},
                    {"roses" => "20", "violets" => 18}
                  );

  # hash holding reference to anonymous arrays
  my %flower_by_color = ("red" => ['roses', 'chrysanthemum', 'amaryllis'], 
                       "white" => ['camellia', 'bouvardia', 'magnolia']);

  # hash holding reference to anonymous hash
  my %flower_by_color2 = ("summer" => {"poppy" => "red", 
                                    "salvia" => "blue"},
                        "fall" => {"camellia" => "white",
                                  "dianthus" => "pink"});

  # Mixed nesting
  my %deliverables = 
        ("flowers" => {"red" => "rose",
                       "blue" => "violet"},
         "addresses" => ["221B Baker Street", "2311 North Los Robles Avenue"]
        );

  ```

### 4.4.3. Dereferences
- Dereferencing is accessing value stored in the memory pointed at by reference
- To dereference one of the following can be done:
  - put appropriate sigil in front of the reference.<br> 
    Depending on whether the reference is pointing to a scalar, array, or a hash, we need to use the correct sigil as prefix to the reference variable<br>
    Example:
    ```perl
    # scalar dereferencing
    my $scalar = "roses";
    my $scalar_ref = \$scalar;
    say ${$scalar_ref}; # dereferencing

    # array dereferencing
    my $array_ref = ["roses", "are", "red"]; # reference to anonymous array
    my @array = @$array_ref; # dereferencing
    say $$array_ref[0]; # dereferencing; prints roses
    
    # hash dereferencing
    my $hash_ref = {"red" => "roses", "violets" => "blue"}; # reference to anonymous hash
    my %hash = %$hash_ref; # dereferencing
    say $$hash_ref{"red"}; # dereferencing; prints roses
    ```

  - put appropriate sigil as prefix and enclose the reference variable in curly braces.<br>
    This is useful for dereferencing a reference stored in a hash or array<br>
    Example:
    ```perl
    # scalar dereferencing
    my $scalar = "roses";
    my $scalar_ref = \$scalar;
    say $$scalar_ref; # dereferencing

    # array dereferencing
    my $array_ref = ["roses", "are", "red"]; # reference to anonymous array
    my @array = @$array_ref; # dereferencing
    say ${$array_ref}[0]; # dereferencing; prints roses
    
    # hash dereferencing
    my $hash_ref = {"red" => "roses", "violets" => "blue"}; # reference to anonymous hash
    my %hash = %$hash_ref; # dereferencing
    say ${$hash_ref}{"red"}; # dereferencing; prints roses

    my %deliverables = 
      ("flowers" => {"red" => "roses",
                     "blue" => "violets"},
       "addresses" => ["221B Baker Street", "2311 North Los Robles Avenue"]
      );
    
    say ${$deliverables{"flowers"}}{"red"}; # dereferencing
    ```
  - using arrow operator **->**<br>
    it is mainly used for references to an array or a hash.
    - the reference variable is placed on the left side of the operator
    - the [<index>] operator are placed to the right of the arrow operator, if the reference is to an array.
    - the {<key>} operator are placed to the right of the arrow operator, if the reference is to a hash
  
  ```perl
  # array dereferencing
  my $array_ref = ["roses", "are", "red"]; # reference to anonymous array
  my @array = @$array_ref; # dereferencing
  say $array_ref->[0]; # dereferencing; prints roses
  
  # hash dereferencing
  my $hash_ref = {"red" => "roses", "violets" => "blue"}; # reference to anonymous hash
  my %hash = %$hash_ref; # dereferencing
  say $hash_ref->{"red"}; # dereferencing; prints roses

  my %deliverables = 
    ("flowers" => {"red" => "roses",
                   "blue" => "violets"},
     "addresses" => ["221B Baker Street", 
                     "2311 North Los Robles Avenue"]
    );
  
  say @deliverables{"flowers"}->{"red"}; # dereferencing      
  say $deliverables{"addresses"}->[0];  # dereferencing      
  ```

# 5. Context

- Every operation in Perl is evaluated according to context. This is a sort of overloading.
- Context is determined by the data type or amount of data that is expected.
- Perl internally converts data between different forms according to the context of operation.

## 5.1. Arithmetic context and operation
- Arithmetic operations can be performed on scalar variables
- Numbers are stored as double-precision floating-point numbers.
- When arithmetic operation is performed on a string, Strings are converted to number - '5' is converted to 5
- When arithmetic operation is performed on a undef, undef is converted to 0

    ```perl
    # With Numbers
    my $x = 5;
    say $x + 1; # prints 6.
    say $x - 2; # prints 3.
    say $x * 3; # prints 15.
    say $x / 4; # prints 1.25
    say int($x / 4); # prints 1
    say $x % 5; # prints 0
    say $x ** 2; # prints 25

    say $x++; # this is post increment. first 5 is printed. then $x is incremented to 6
    say ++$x; # this is pre increment. first $x is incremented to 7, then 7 is printed
    say $x--; # this is post decrement. first 7 is printed. then $x is decremented to 6
    say --$x; # this is pre decrement. first $x is decremented to 5, then 5 is printed

    $x+=10; # $x holds 15. add and assign
    $x-=10; # $x holds 5 subtract and assign
    $x*=2;  # $x holds 10 . multiply and assign
    $x/=5;  # $x hold 2 . divide and assign

    # With undef
    my $y; # undef is assigned to $y
    say 22 + $y; # undef in $y is converted to 0 and 22 is added to it. 22 is printed

    # With strings
    my $z = '5';
    say $z + 1; # prints 6.

    my $e = '5 e16';
    say $e + 1; # prints 6

    my $f = '5';
    my $g = 0 + $f; # force numeric context

    ```

## 5.2. String context and operation
- Strings ia a sequence of zero or more characters
- Strings can be expressed with single quotes or double quotes. 
  - Expressions and variables are interpreted if they are within double quotes
  - Expressions and variables are printed literally if they are in single quotes.
- When a string operation a being performed on a number and the operation expects a string, the number is converted to string
- When a string is expected from a variable and the variable contains *undef*, *undef* is converted to an empty string i.e. ""

  ```perl
  # With strings
  my $p = "Hello";
  say $p . " World"; # concatination operation. prints Hello World
  $p .= " Again, World"; # concatinate and assign operation. $p hold Hello Again, World
  say $p; # prints Hello Again, World

  my $q = "na";
  say $q x 3; # duplicate operation. prints nanana
  $q x= 4; # duplicate and assign operation. $p hold nananana
  say $q; # prints nananana

  # With numbers
  my $r = 3;
  my $s = "Half-Life ".$r; # $r is converted to string. the string '3' is then concatinated to Half-Life
  say $s; # prints Half-Life 3

  my $t = "ha" x $r; # since number is expected, $r is not converted to string
  say $t; # prints hahaha

  my $u = "4";
  my $v = "ho" x $u;   # $u is converted to number 4
  say $v; # prints hohohoho

  my $i = 4;
  my $j = ''.$i; # force string context

  # With undef
  my $w; # $w has undef
  say "This is the " . $w; # $w is converted to empty string "". the statement prints This is the
  ```

## 5.3. Boolean Context
- In a conditional statement, Boolean context is effective.
  *More on that later*


## 5.4. Scalar Context
- Scalar context means that an operation or expression is expected to produce a scalar value.
- an operation provides a scalar value according to its implementation, for example - the last element, size, etc
- If the variable sigil is $ in the left hand side of an expression(```$lhs = <sigil>rhs```) then also scalar context is imposed.
  - a list assignment in scalar context returns the number of elements on the right-hand side of the list assignment
    - syntax ```my $scalar = <List1> = <List2>```<br> number of elements in List2 is placed in $scalar
- we can also force scalar context on data by using ```scalar```

### 5.4.1. Example 
- when we assign a list to a scalar variable, the scalar variable stores the last element in the list.
  ```perl
  my $scalar_variable = (1,3,5,7); # $scalar_variable stores 7, which is the last number in the array
  ```
- when we assign an array to a scalar variable, the scalar variable stores the length of array
  ```perl
  my @array = (1,3,5,7);
  my $scalar_variable = @array; # $scalar_variable stores 4, which is the number of records in the array
  ```
- when we assign a hash to a scalar variable, it returns the number of elements
  ```perl
  my %hash = {"roses" => "red", "violets" => "blue"};
  my $scalar_variable = %hash; # $scalar_variable variable now has 2
  ```
- We can force scalar context, by using ```scalar```
  ```perl
  my @array = (1,3,5,7);
  say @array; # prints 1357
  say scalar @array; # prints 4
  ```

- list assignment in scalar context
```perl
my $scalar1 = qw(roses are red); # $scalar1 has red;
my $scalar2 = () = qw(roses are red); # $scalar2 has 3
say $scalar1;
say $scalar2;
```

- when an empty list is assigned to a scalar variable
  ```perl
  my $scalar_var = (); # undef is assigned to $scalar_var 
  ```
  
## 5.5. List Context
- List context mean that an operation or expression is expected to produce a list
- If the variable sigil is @ or % in the left hand side, then a list is expected
- if there is a list in the lvalue, then a list is expected

### 5.5.1. Examples
- when a list is assigned to an array
  ```perl
  my @arr = (1,2,3);
  ```

- when a list is assigned to an array
  ```perl
  my %arr1 = ('a',1,'b'); # this line will give error that 'Odd number of elements in hash assignment' because value is missing for key 'b'
  my %arr2 = ('a',1,'b',2); # hash will have 2 key value pairs
  ```

- when a list is assigned to another list
  ```perl
  my ($a, $b, $c) = (1,2,3,5); # since there are only 3 element on the left side, only the first 3 elements of the right side list is copied 
  say $a; # prints 1
  say $b; # prints 2
  say $c; # prints 3

  my ($x) = (13,21,34,55); # since there are only 1 element on the left side, only the first element of the right side list is copied
  ```

- when a scalar is assigned to a list
  ```perl
  my @array = "sunflower"; # the scalar is implicitly converted into a single-element list
  ```

- when an array is assigned to a list
  ```perl
  my @arr = qw(roses are red);
  my ($x) = @arr; # array is converted into a list in the right side. then only the first element is copied
  ```
## 5.6. Void context
- void context is effective when the value of an expression is not used. 
- common statements used in context are print and say.

# 6. Flow Controls
## 6.1. Conditionals
- conditional statements are used to control the flow of program according to some condition
- after a condition is evaluated, the subsequent activity depends on the result of the evaluations. The result of the evaluation can be either true or false.
- data is evaluated in scalar boolean context
- Perl provides following conditionals
  - if, if...else, if...elseif
  - unless
  - for-when
### 6.1.1. Boolean values
- Perl does not have any separate boolean type
- the following values are considered false
  - undef
  - 0
  - "0"
  - ""
  - empty list
- everything else is true
- ```!``` operator can be used to check invert the boolean value of a variable, i.e. true is converted to false and vice-versa. 

### 6.1.2. Comparisons
#### 6.1.2.1. Arithmetic comparisons

operator  | description
---       | ---
=         | returns true if both left and right arguments are equal, else false
!=        | returns true if both left and right are NOT equal, else false
\>        | returns true if left argument is greater than right argument, else false
\>=       | returns true if left argument is greater than or equal to right argument, else false
<         | returns true if left argument is lesser than right argument, else false
<=        | returns true if if left argument is lesser than or equal to right argument, else false
<=>       | returns<br>-1 if left argument is less than the right<br>0 if both are equal<br>1 if left argument is greater than the right argument

#### 6.1.2.2. String comparisons
operator  | description
---       | ---
eq        | returns true if both left and right arguments are stringwise equal, else false
ne        | returns true if both left and right arguments are NOT stringwise equal, else false
gt        | returns true if left argument is stringwise greater than right argument, else false
ge        | returns true if left argument is stringwise greater than or equal to right argument, else false
lt        | returns true if left argument is stringwise less than right argument, else false
le        | returns true if left argument is stringwise less than or equal to right argument, else false
cmp       | returns<br>-1 if left argument is stringwise less than the right<br>0 if both are stringwise equal<br>1 if left argument is stringwise greater than the right argument

### 6.1.3. Logical operators
- logical operators are used 
  - to combine multiple conditions
  - to invert the result of another condition

operator  | description
---       | ---
&&        | returns true when both conditions are true.
and       | returns true when both conditions are true. Has lower precedence
||        | returns true when any one of the conditions are true. Has lower precedence
!         | returns true when the result of a condition is false and vice-versa.
not       | returns true when the result of a condition is false and vice-versa. has lower precedence
//        | returns true when any one of expressions does not return an undef

### 6.1.4. ```if```, ```if```...```else```, ```if```...```elsif```
- To execute a set of statements when condition is true, use ```if```
  - syntax
  ```perl
  if ( test ) {
    #statements
  }
  ```
  The test is any expression that is evaluated in scalar context and converted to boolean to check its truth value.

- To execute a different set of instructions when the condition is false, the statements are placed after else
  - syntax
  ```perl
  if ( test ) {
    # statements to execute when condition is true
  } else {
    # statements to execute when condition is false
  }
  ```
- if.. else can be nested
  - syntax
  ```perl
  if ( test1 ) {
    if ( test2 ) {
      #statementstest2
    } else {
      #statementstest2_else
    }
  } else {
    if ( test3 ) {
      if ( test4 ) {
        # statementtest3
      } else {
        # statementtest3_else
      }
    }
  }
  ```
- ```elsif``` can be used when there are multiple decisions to take
  - syntax
  ```perl
  if ( test1 ) {
    # statement1
  } elsif ( test2 ) {
    # statement2
  } elsif ( test3 ) {
    # statement3
  } else {
    # statement_else
  }
  ```

### 6.1.5. ```unless```
- To execute a set of statements when condition is false, use ```unless```
  - syntax
  ```perl
  unless ( test1 ) {
    # statement1
  }
  ```
- using ```unless``` is not recommended due to readability issues. ```unless``` can be used when used in postfix form (later section)
- ```unless``` also has ```else```. However, using this is not advised, because it will make code harder to read

### 6.1.6. Postfix
- ```if``` and ```unless``` can be used as postfix to run single statements.
  - syntax
  ```statement1 if test1```<br>
  ```statement2 unless test2```
  - Example
  ```perl
  my $age = 18;
  say "can vote" if $age > 18;
  
  my $day = "Monday";
  say "it is not Sunday" unless $day eq "Sunday";
  ```

### 6.1.7. Ternary operator
- Ternary operators (?:) is a shorthand for ```if```..```else```
- syntax is ```test1? statement_for_true : statement_for_false```
- ternary operator can be nested
  ```perl
  my $flower = 'violets';
  my $color = $flower eq "roses"  ?"red":
              $flower eq "violets"?"blue":
                                   "Flower unknown";

  say $color;
  ```

### 6.1.8. Short-circuit
- short-circuit means that an expression is not evaluated completely once its final value is known.
- When multiple statements are combined with ```and``` or ```&&```, a statement is executed and evaluated only if its preceding statement evaluated to true.
  - the first statement is always evaluated
  - if any of the conditions evaluates to false, the whole combination of conditions will be false
- When multiple statements are combined with ```or``` or ```||```, a statement is executed and evaluated only if its preceding statement evaluated to false.
  - the first statement is always evaluated
  - if any of the conditions evaluates to true, the whole combination of conditions will be true
- When multiple statements are combined with ```//```, a statement is executed and evaluated only if its preceding statement evaluated to ```undef```.
  - the first statement is always evaluated
  - if any of the conditions evaluates to true, the whole combination of conditions will be true
- This feature can be used to chain multiple statements together.


#### 6.1.8.1. Example
- print if condition is true
  ```perl
  my $flower = "violets";
  
  $flower eq "roses" && say "roses are red";
  $flower eq "violets" && say "violets are blue";
  # prints "violets are blue"
  ```

- Assigning default value if there is no value in array
  ```perl
  my @flowers = qw(roses);
  my $customer1 = shift @flowers // "No flowers"; # assigns roses
  my $customer2 = shift @flowers // "No flowers"; # assigns No flowers
  say $customer1;
  say $customer2;
  ```

- Assigning default value if there is no value in hash
  ```perl
  my %flowers =    
      ("roses" => "red", 
       "violets" => "blue");


  $flowers{"sunflower"} //= "yellow";
  say $flowers{"sunflower"}; # prints yellow
  ```


### 6.1.9. Hash Examples
- check if hash is empty
  ```perl
  my %flowers =    
      ("roses" => "red", 
       "violets" => "blue",
       "sunflower" => "yellow");
  
  if (%flowers) {
    say "We have flowers";
  } else {
    say "We don't have flowers";
  }

  say "emptying the hash flowers";
  %flowers = ();

  if (%flowers) {
    say "We have flowers";
  } else {
    say "We don't have flowers";
  }
  ```
- check if key is present
    - use ```exists```

  ```perl
  my %flowers =    
      ("roses" => "red", 
       "violets" => "blue",
       "sunflower" => "yellow");
  
  if (exists $flowers{"roses"}) {
    say "roses are $flowers{'roses'}";
  }

  if (exists $flowers{"gerbera"}) {
    say "roses are $flowers{'gerbera'}";
  }
  ```

- check if value is undef or not
  - use ```defined``` to check if value is defined
  ```perl
  my %flowers =    
      ("roses" => "red", 
       "violets" => "blue",
       "sunflower" => "yellow",
       "tulip" => undef);
  
  if (defined $flowers{"roses"}) {
    say "We know the color of roses";
  } else {
    say "We don\'t know the color of roses";
  }

  if (defined $flowers{"tulip"}) {
    say "We know the color of tulip";
  } else {
    say "We don\'t know the color of tulip";
  }
  ```

### 6.1.10. Array Examples
- check if array is empty
  ```perl
  my @flowers = 
      ("roses", 
       "violets",
       "sunflower");
  
  if (@flowers) {
    say "We have flowers";
  } else {
    say "We don't have flowers";
  }

  say "emptying the array flowers";
  @flowers = ();

  if (@flowers) {
    say "We have flowers";
  } else {
    say "We don't have flowers";
  }
  ```

- check if value is defined
  - use ```defined```
  ```perl
  my @flowers = 
      ("roses", 
       "violets",
       "sunflower");
  
  if (defined $flowers[0]) {
    say "first flower is $flowers[0]";
  } else {
    say "We don\'t have flowers in the first position";
  }

  if (defined $flowers[5]) {
    say "sixth flower is $flowers[5]";
  } else {
    say "We don\'t have flowers in the sixth position";
  }
  ```

## 6.2. Loops
- loop is sequence of statements which is specified once and carried out multiple times in succession
- Perl provides following loops
  - ```while```, ```do..while```, ```until```
  - ```for```
  - ```foreach```

### 6.2.1. Condition controlled loop
- loops are repeated until a condition is met
- Perl provides ```while```, ```do...while```, ```until``` loops for this
- in case of ```while```, the condition is checked at the start of the loop.<br>loop runs as long as the condition is true
- in case of ```do...while```, the condition is checked at the end of the loop.<br>This means that the contents of the loop runs at least once.<br>Loop runs as long as the condition is true
- in case of ```until```, the condition is checked at the start of the loop.<br>loop runs as long as the the condition is false
  - having negative conditions in ```until``` should be avoided
- syntax
  ```perl
  while (test1) {
    # statements
  }

  do {
    # statements
  } while(test2);

  until (test3) {
    # statements
  }
  ```
Example:
- print numbers from 1 to 5
  ```perl
  my $i = 1;
  while($i <= 5) {
    say "while : $i";
    ++$i;
  }

  my $j = 1;
  until ($j > 5) {
    say "until : $j";
    ++$j;
  }

  my $k = 1;
  do {
    say "do while : $k";
    ++$k;
  } while ($k < 5);
  ```


### 6.2.2. list controlled loop
- loops are repeated over every item of a list
- ```for``` and ```foreach``` can be used
- A variable is used to hold individual elements of the list.
  - Any change made to the variable is also reflected in the list
- syntax
  ```perl
  for var (list) {
    # statements
  }

  foreach var (list) {
    # statements
  }
  ```

Example:
- print the content of a array
  ```perl
  my @flowers = qw(roses violets sunflowers);
  for my $flower (@flowers) {
    say "flower is $flower";
  }


  foreach my $flower (@flowers) {
    say "flower is $flower";
  }
  ```
- increase numbers in list by 5
  ```perl
  my @numbers = (1..5);
  say "Before loop: @numbers";
  for my $num (@numbers) {
    $num += 5;
  }
  say "After loop: @numbers";
  ```
- print the keys of hash
  ```perl
  my %flower_color = ("roses" => "red" , "violets" => "blue");
  foreach my $flower(keys %flower_color) {
    say $flower;
  }
  ```

- print the values in hash
  ```perl
  my %flower_color = ("roses" => "red" , "violets" => "blue");
  foreach my $color(values %flower_color) {
    say $color;
  }

  foreach my $flower(keys %flower_color) {
    say $flower_color{$flower};
  }
  ```

- print key value pairs in hash
  ```perl
  my %flower_color = ("roses" => "red" , "violets" => "blue");
  foreach my $flower(keys %flower_color) {
    say "$flower => $flower_color{$flower}";
  }


  my ($key, $value);
  while (($key, $value) = each(%flower_color))
  {
    say "$key => $value";
  }
  ```

### 6.2.3. Count-controlled loop
- loops are repeated for a specified number of times 
- syntax
  ```perl
  for (initialize; test; update) {
    # statements
  }
  ```

  Example:
  - print roses 5 times
  ```perl
  for (my $i = 0; $i < 5; ++$i) {
    say "roses";
  }
  ```

### 6.2.4. Loop within loop
- we can have loops within loops
  
  Example:
  ```perl
  my @names = qw(Monica Erica Rita);
  my @flowers = qw(roses violets);

  foreach my $name (@names) {
    foreach my $flower (@flowers) {
      say "A little bit of $flower for $name";
    }
  }
  ```

### 6.2.5. Loop control
#### 6.2.5.1. Label
- we can give name to different loops using labels
- the label is optional
- it can be any word. It must be followed by a colon
- labels are usually written in uppercase

  Example:
  ```perl
  my $i = 0;
  my @names = qw(Monica Erica Rita);
  my @flowers = qw(roses violets);

  LABEL: while ($i < 3) { 
    say $i;
    ++$i;
  }

  OUTER: foreach my $name (@names) {
    INNER: foreach my $flower (@flowers) {
      say "A little bit of $flower for $name";
    }
  }
  ```
#### 6.2.5.2. ```next```
- ```next``` starts the next iteration of the loop
- if a label is mentioned, the control goes to the label's loop. 
- if no label is mentioned, the control goes to the enclosing innermost loop

  Example:
  ```perl
  foreach my $n ((1..5)) {
    next if $n == 3; # if 3 is found, start the next iteration of the loop
    say $n;
  }

  my @names = qw(Monica Erica Rita);
  my @flowers = qw(roses violets sunflowers);

  OUTER: foreach my $name (@names) {
    INNER: foreach my $flower (@flowers) {
      next if $flower eq 'roses'; # if the $flower is roses, start the next iteration of the INNER loop
      say "A little bit of $flower for $name";
    }
  }


  OUTER: foreach my $name (@names) {
    INNER: foreach my $flower (@flowers) {
      next OUTER if $name eq 'Erica'; # if the name is Erica, start the next iteration of the OUTER loop
      say "A little bit of $flower for $name";
    }
  }
  ```

#### 6.2.5.3. ```last```
- ```last``` exits the loop
- if a label is mentioned. it exits the label's loop
- if no label is mentioned, it exits the innermost enclosing loop

  Example
  ```perl
  foreach my $n ((1..5)) {
    last if $n == 3; # if 3 is found, exit the loop
    say $n;
  }

  my @names = qw(Monica Erica Rita);
  my @flowers = qw(roses violets sunflowers);

  OUTER: foreach my $name (@names) {
    INNER: foreach my $flower (@flowers) {
      last if $flower eq 'violets'; # if the $flower is roses, exit the INNER loop
      say "A little bit of $flower for $name";
    }
  }

  say '-----';

  OUTER: foreach my $name (@names) {
    INNER: foreach my $flower (@flowers) {
      last OUTER if $name eq 'Erica'; # if the name is Erica, exit the OUTER loop
      say "A little bit of $flower for $name";
    }
  }
  ```

#### 6.2.5.4. ```redo```
- ```redo``` restarts the current iteration of the loop, without reevaluating the conditions
- if label is mentioned, it will restart the current iteration of the label's loop
- if no label is mentioned, it will restart the current iteration of the innermost enclosing loop

  Example:
  ```perl
  my $i = 0;

  while ($i < 5) {
    ++$i;
    redo if $i == 3; # when $i is 3, the iteration starts again
    say $i;
  }
  ```

### 6.2.6. Topic
- Perl has a default variable
- it is called topic
- it is represented by $_
- When an operation is expected to work on a variable and no variable is passed, the operation works on the default variable
- When an operation assigns a value to a variable, and no variable is provided, the operation assigns value to the default variable

  Example
  ```perl
  say "look at the roses";
  my @rose = qw(roses are red);
  # regular loop
  foreach my $word (@rose) {
    say $word;
  }

  say "look at the violets";
  my @violet = qw(violets are blue);
  # with topic variable
  foreach (@violet) { # skipped the variable in the foreach. each item is assigned to $_
    say $_;
  }

  say "look at the stars";
  my @stars = qw(they were all yellow);
  # another example with topic variable                                                                                                                                                                                                       
  foreach (@stars) {
    say; # skipped the variable in say. say uses the $_ variable
  }
  ```

- default variables are not recommended when they degrade the readability of code
  - like in nested loops, $_ can confuse the reader whether the $_ is working on the inner loop or outer loop

### 6.2.7. Postfix 
- the loops can be specified as postfix
- when loops are postfix, we cannot specify a variable name. We need to use $_
- syntax ```statement foreach(list)```

  Example:
  ```perl
  my @rhymes1 = qw(roses are red violets are blue);
  say foreach (@rhymes1);               

  my @rhymes2 = qw(my name is Dave Microwave);
  say '<'.$_.'>'  foreach(@rhymes2);
  ```

### 6.2.8. ```continue```
- ```continue``` block is executed before an condition is evaluated after the first iteration of loop.
- can be used with ```foreach``` and ```while``` loops
- syntax
  ```perl
  while (test) {
    # statements 1
  } continue {
    # statements 2
  }

  foreach $variable (list) {
    # statement 1
  } continue {
    # statement 2
  }
  ```
- in case of ```next```, ```continue``` block is run before the next iteration
- in case of ```last```, ```continue``` block is not run
- in case of ```redo```, ```continue``` block is not run

# 7. Subroutines
- a subroutine is a group of statements packed together as an unit.
- this unit can be used wherever we need the group of statements to be run
- the terms subroutine, function and method are used interchangeably
- usually, a list is passed to a subroutine, and the subroutine returns a list
- syntax
  - defining subroutine
    ```perl
    sub subroutine_name {
      # statements
    }
    ```
  - calling subroutine
    ```perl
    subroutine_name(list);
    subroutine_name list; # the parenthesis are optional
    ```


## 7.1. argument variable ```@_```
- the list passed to a subroutine is stored in the default argument variable ```@_```
  - the first item can be accessed via ```$_[0]```, the second item can be accessed by using ```$_[1]```
- example
  ```perl
  sub floral_print {   
    my $flower = $_[0]; # move the first element to $flower               
    say " U @    <--$flower";
    say "  \| () ";
    say " __|/_  ";
    say " \\    /";
    say "  \\__/ ";
    say "";
  }

  my @flowers = qw(roses violets sunflowers orchids);
  foreach my $flower(@flowers) {
    floral_print($flower); # call floral_print for each flower
  }
  ```

- when any item is updated in ```@_```, the item in the callee is also updated
  ```perl
  sub set_flower_to_gerbera {
    $_[0] = "gerbera"; # updates to gerbera
  }

  my $flower = "rose";
  say $flower; # prints rose
  set_flower_to_gerbera($flower);
  say $flower; # prints gerbera
  ```

## 7.2. ```return```
- ```return``` statement is used to exit subroutine
- ```return``` may specify a list or value
- If no ```return``` is found and if the last statement is an expression, its value is returned

  ```perl
  sub price_after_discount {
    my $cost_price = $_[0];
    my $discount_percentage = $_[1];
    return $cost_price*(1-$discount_percentage/100);
  }

  sub price_after_discount_shorter {
    $_[0]*(1-$_[1]/100); # even if return is not mentioned, the result is returned
  }
  
  my $discount = 20;
  my @flower_prices = (100, 150, 200);
  foreach my $price(@flower_prices) {
    say price_after_discount($price, $discount);
  }
  
  say "shorter version results";
  foreach my $price(@flower_prices) {
    say price_after_discount_shorter($price, $discount);
  }
  ```
## 7.3. Passing arguments
- an array or list can be passed to subroutine and the subroutine will hold it in @_ variable
  - if a combination of multiple lists or arrays or scalars are passed to a subroutine, the @_ will flatten the list/array and hold all the values a single long list
- a hash can be passed to subroutine, the hash will be converted into a list and the subroutine will hold it in @_ variable
- a reference can be passed to subroutine.
  - the reference can be dereferenced and the subroutine can work on the values
    
  <br>  
  Examples

  - find the maximum
    ```perl
    sub get_max_between_2_numbers {
      my ($a, $b) = @_;
      return $a>$b?$a:$b;
    }

    sub get_max_from_array {
      my @arr = @_;
      my $max = pop @arr;
      foreach my $number (@arr) {
        $max = get_max_between_2_numbers($max, $number);
      }
      return $max;
    }

    my @arr1 = (8,4,1,5,2,9);
    my @arr2 = (2,4,4,1,1,3,9);
    my $scalar_variable = 33;
    say get_max_from_array(@arr1); # prints 9
    say get_max_from_array(@arr1, (1..4), 22, $scalar_variable); # prints 33
    ```
  - printing out the diagonal 5x5 matrix
    ```perl
    sub print_diagonal {
      my $matrix_ref = $_[0];
      for my $idx (0..4) {
        # say " " x $idx, $matrix_ref->[$idx]->[$idx];
        say $matrix_ref->[$idx]->[$idx];
      }
    }

    my @row0 = (0..4);
    my @row1 = (5..9);
    my @row2 = (10..14);
    my @row3 = (15..19);
    my @row4 = (20..24);
    
    my @matrix = (\@row0,
                  \@row1,
                  \@row2,
                  \@row3,
                  \@row4);
    
    print_diagonal(\@matrix);
    ```

## 7.4. Pass by Reference
- Perl passes by reference
- any updates to the parameters made in the called subroutine is reflected in the calling location
  - when a scalar is passed to a subroutine, the scalar is placed in into @_ as a single element list.
    - changes made to the first element is reflected in the scalar variable in the calling location
  - when an array is passed to a subroutine, the array is aliased to @_.
    - changes made to the array will be reflected in the calling location
  - when a hash is passed to a subroutine, the hash is converted into a list and passed to the calling location
    - changes made to the keys in the called subroutine, is not reflected in the calling location
    - changes made to the values in the called subroutine, are reflected in the calling location
- when a list is assigned to the whole array @_, no changes are reflected in the calling  location


  Example
  ```perl
  sub updates_scalar1 {
    $_[0] = 'violets';
  }

  sub updates_scalar2 { 
    my $scalar_variable = $_[0];    
    $scalar_variable = 'sunflower';    
  }    
    
  sub updates_array1 {    
    ($_[0], $_[1], $_[2], $_[3]) = qw(an apple a day);    
  }                        
        
  sub updates_array2 {     
    @_ = qw(keeps the doctor away);       
  }                                                 
       
  sub updates_hash1 {    
    ($_[0], $_[1], $_[2], $_[3]) = ("apple" => "day", "doctor" => "away");          
  }                                                                                 
                          
  sub updates_hash2 {     
    my %hash_variable = @_;    
    %hash_variable = qw(stitch time saves nine);    
  }    
       
    
  my $scalar1 = "rose";    
  updates_scalar1($scalar1);    
  say $scalar1; # prints violets
      
  my $scalar2 = "rose";    
  updates_scalar2($scalar2);    
  say $scalar2; # prints rose
      
  my @array1 = qw(roses are red);    
  updates_array1(@array1);    
  say "@array1"; # prints an apple a
      
  my @array2 = qw(violets are blue);    
  updates_array2(@array2);    
  say "@array2"; # prints violets are blue
      

  my %hash1 = ("roses" => "red", "violets" => "blue");
  updates_hash1(%hash1);
  my ($key1, $value1);
  while (($key1, $value1) = each(%hash1))
  {
    say "$key1 => $value1"; 
  } # prints
    # roses => day
    # violets => away

  my %hash2 = ("stars" => "yellow", "cars" => "red");
  updates_hash1(%hash1);
  my ($key2, $value2);
  while (($key2, $value2) = each(%hash2))
  {
    say "$key2 => $value2";
  } # prints
    # stars => yellow
    # cars => red
  ```

# 8. Package
- a package is a collection of codes
  - has variables and functions within it
- prevents name collision with identifiers having same name but from outside the package
- variables of a package can be explicitly referred to using ```::```
- ```__PACKAGE__``` is a special variable which stores the current package's name 
- syntax
  ```perl
  package Pack;
  # code
  # subroutines
  # variables
  ```

  ```perl
  package Pack {
    # code
    # variables
    # subroutines
  }
  ```
  
  Example
  - define a package
  ```perl
  my %catalog = ("rose" => 10);
  say "1. In package <", __PACKAGE__, "> and cost of rose is <$catalog{rose}>";


  package Gotham 
  {
    my %catalog = ("rose" => 1);
    sub get_cost {        
      my $flower = $_[0];
      $catalog{$flower};
    }
    
    sub add_flower {
      my ($flower, $cost) = @_;      
      $catalog{$flower} = $cost;      
    }       
    say "2. In package <", __PACKAGE__, "> and cost of rose is <$catalog{rose}>";
  }

  package Winterfell 
  {
    my %catalog = ("rose" => 1000);
    sub get_cost {        
      my $flower = $_[0];
      $catalog{$flower};
    }
    
    sub add_flower {
      my ($flower, $cost) = @_;
      $catalog{$flower} = $cost;
    }
    say "3. In package <", __PACKAGE__, "> and cost of rose is <$catalog{rose}>";
  }

  say "4. In package <", __PACKAGE__, "> and cost of rose is <$catalog{rose}>";
  say "5. ", Gotham::get_cost("rose"); # prints 1                    
  say "6. ", Winterfell::get_cost("rose"); # prints 1000

  say "7. adding violets to Gotham's catalog";
  Gotham::add_flower("violet", 5);
  say "8. violet => ", Gotham::get_cost("violet");
  
  say "9. adding winter rose to Winterfell's catalog";                    
  Winterfell::add_flower("winter rose", 11);
  say "10. winter rose => ", Winterfell::get_cost("winter rose");
  ```

# 9. Special subroutines - ```BEGIN```, ```END```, ```CHECK``` and ```INIT```
- For these subroutines, ```sub``` keyword is optional
## 9.1. ```BEGIN```
- ```BEGIN``` is executed during the compilation time
- it is run before any other statement is executed
- if multiple ```BEGIN``` are defined, they are executed in a "first in first out" basis

## 9.2. ```CHECK```
- ```CHECK``` is executed at the end of the compilation process
- if multiple ```CHECK``` are defined, they are executed in a "last in first out" basis

## 9.3. ```INIT```
- ```INIT``` executed at the beginning of execution process
- if multiple ```INIT``` are defined, they are executed in a "first in first out" basis

## 9.4. ```END```
- ```END``` is executed at the end of the execution process, before the interpreter exits
- if multiple ```END``` are defined, they are executed in a "last in first out" basis

- Example
  ```perl
  BEGIN {
    say "In BEGIN";
  }

  INIT {
    say "In INIT";
  }

  CHECK {
    say "In CHECK";
  }

  END {
    say "In END";
  }

  say "In Normal"
  ```

- Output
  ```
  In BEGIN
  In CHECK
  In INIT
  In Normal
  In END
  ```

# 10. Modules
-  module is a reusable package
-  defined in a library file
   -  name of file is same as the package
   -  the file has an extension of *.pm*
-  the module returns a true value

- declaring a module
  ```perl
  # filename is Flower.pm

  use Modern::Perl;

  # declaring package
  package Flower;

  sub welcome {
    my $name = shift;
    say "Hello, World. Welcome to $name flower shop";
  }

  sub give {
    say '  @@@@  ';
    say ' @@()@@ ';
    say '  @@@@  ';
    say '   /    ';
    say '   |    ';
  }

  sub thank {
    say "Thank you for visiting. Please come again";
  }

  1; # need to end with a true
  ```

- ```use``` loads the module file 
  ```perl
  # filename is Flowershop.pl

  use Modern::Perl;

  # modules are searched in locations maintained in Perl's in-built variable @INC
  # however, I placed my file Flower.pm in the same directory as Flowershop.pl
  # so, I need to add the folder in @INC
  # this should be done at the start of compilation
  # so, the location is added to @INC at the start of compilation
  BEGIN { # had to add this block so that the folder path of the Flower  
   unshift @INC, '.'; #
  } 

  use Flower; # using package Flower

  # calling functions of the module
  Flower::welcome("Perldorado");
  Flower::give();
  Flower::thank();
  ```
  on running the above we get:
  ```
  Hello, World. Welcome to Perldorado flower shop
    @@@@ 
   @@()@@ 
    @@@@  
     / 
     | 
  Thank you for visiting. Please come again
  ```

# 11. Variable scope
- https://www.perlmonks.org/?node_id=66677
- https://perlmaven.com/scope-of-variables-in-perl


- scope of variable is the range of places where a variable is accessible
- a variable declared with ```my``` is visible only within the block it is declared in
  - a block is the code within braces {}
    - a variable declared with ```my``` within the {} is not accessible outside the {} block
  - files are also considered blocks
    - a variable declared with ```my``` within a file is not accessible outside the file
  - ```my``` variables are defined again on reentering their scope block. they are initialized again.
  ```perl
  sub give_rose {
    my $flower = "rose";
    say "give the customer : $flower";
  }

  sub give_violet {
    my $flower = "violet";
    say "give the customer : $flower";
  }

  my $flower = "lily";
  say "give the customer : $flower";
  give_rose;
  give_violet;
  say "give the customer one more $flower";
  ```

- a ```state``` variable is like ```my``` variable in the sense that they are visible only within the block it is declared in
  - ```state``` variables are not defined again on reentering their scope. They retain their old values
- Example
  ```perl
  sub count_customer {
    state $count = 0;
    ++$count;
    return $count;
  }

  say count_customer;
  say count_customer;
  say count_customer;
  ```

- a variable in package, that is declared with ```our```, will be visible to files using the package
  - the file must load the package using ```use package_name;```
  - the variable defined with ```our``` in the package will be accessible using ```<sigil><package_name>::<variable_name>```
  - Example:
    ```perl
    #in file FlowerOur.pm

    use Modern::Perl;

    package FlowerOur;
    our @flower_list = qw(roses violets sunflowers);
    1;
    ```
    ```perl
    #in file flower_our.pl
    use Modern::Perl;

    BEGIN {
            push @INC, ".";
    }
    
    use FlowerOur;

    for my $flower (@FlowerOur::flower_list) { # accessing an our variable from a different file
            say "I have $flower";
    }
    ```

# 12. CPAN
- large collection of Perl modules and documentation
- ```cpanm``` command downloads, tests and installs modules and their dependencies
- in order to use installed module, use the ```use <module>;```
- ```cpan -a``` prints the list of installed modules
- ```cpanm --uninstall <module_name>``` - used to remove distributions
- few curated list of modules
  - https://metacpan.org/pod/Task::BeLike::DAGOLDEN
  - https://metacpan.org/pod/Task::Kensho
  - http://neilb.org/reviews/
  - http://blog.kablamo.org/2015/09/08/mstpan/


# 13. Input and output
## 13.1. Command input
- command enclosed within backticks (\` or qx) are first interpolated and then executed 
  - the system executes the command
  - the output of the command can be captured in a variable
    - in scalar context, a single string of the command output is returned
    - in list context, each line of the output is treated as an individual element
- syntax
  - ```<sigil><variable> = \`command1\`;```
  - ```<sigil><variable> = qx(command1);```

  *Note: when qx is used with single quotes, i.e. qx'command1' the variables in the command are not interpolated*

## 13.2. Read from file
- has three steps - open file, read from file and close file
- ```open``` function is used to open a file
  - syntax - ```open(filehandle, mode, filename)```
  - filehandle is a variable that associates with a file
  - mode can be '<' for read
  - example - ```open (FH, '<' , 'some/directory/input-file.txt')```
  - ```open``` returns true if file is opened successfully and false otherwise
- ```readline``` function is used to read data from file
  - syntax - ```readline(*filehandle)```
  - <> can be used as an alternative to ```readline```
    - ```<filehandle>```
  - in scalar context, reads and returns the next line until end-of-file is reached
  - in list context, reads until end-of-file is reached and returns a list of lines
- file is closed using ```close``` function
  - syntax - ```close(filehandle)```

- example
  ```perl
  open(FH, "<", "input_file.txt");
  my @arr = readline(*FH);
  say "@arr";
  close(FH);


  open(FH2, "<", "input_file.txt");
  while (my $line = <FH2>) {
    chomp($line); # removes the newline at the end of line
    say $line;
  }       
  close(FH2);
  ```
## 13.3. Exception handling in Files
- in case of issue in opening a file, we can 
  - throw an exception if file cannot be opened
    - ```die``` is used to throw an exception
      - ```open(fh, '<', $filename) or die "Couldn't Open file $filename";```
  - give a warning if file cannot be opened and continue running 
    - ```warn``` is used to give warning
      - ```warn "Couldn't Open a file $filename";```

## 13.4. Command line arguments
- Perl has a special array ```@ARGV```
- all command line inputs are placed in the array ```@ARGV```
- for example, when ```perl script1.pl arg0 arg1 arg2``` is run, $ARGV[0] holds arg0, $ARGV[1] holds arg1, $ARGV[2] holds arg2
- another example -
  ```perl
  # filename is box_text.pl
  use Modern::Perl;

  my $text =  $ARGV[0]; # setting variable $text with the first argument in the command line
  my $length = length $text;

  say "*" x ($length + 4);
  say "* "," " x $length," *";
  say "* ".$text." *";
  say "* "," " x $length," *";
  say "*" x ($length + 4);
  ```
  we run the code using ```perl box_text.pl Welcome```
  we get the output as follows:
  ```
  ***********
  *         *
  * Welcome *
  *         *
  ***********
  ```


## 13.5. Input Filenames in command line
- diamond operator ```<>``` in ```while``` loop opens files mentioned in the command line
  - the files are read in the order they are mentioned in the command line
  - the files are read in scalar context, that is line-by-line
  - each line is stored in the topic variable ```$_```
- example
  ```perl
  while(my $line = <>) {
    chomp($line); # chomp removes the trailing newline at the end of the line
    say $line;
  }
  ```

## 13.6. Writing into files
- like reading from file, writing to file has three steps - open file, write to file and close file
- ```open``` function is used to open a file
  - syntax - ```open(filehandle, mode, filename)```
  - filehandle is a variable that associates with a file
  - mode can be '>' for write, '>>' for append
  - example - ```open (FH, '>' , 'some/directory/output-file.txt')```
  - ```open``` returns true if file is opened successfully and false otherwise
- ```print```, ```say``` functions are used to read data from file
  - syntax - ```say filehandle "text-to-be-written-in-file"```
  - if data is written to a file that has content, then the file is first truncated, and then the data is written (unless file is opened in append mode)
- file is closed using ```close``` function
  - syntax - ```close(filehandle)```

- example
  ```perl
  open(FH, ">", "output_file.txt");
  say FH "Roses are red";
  say FH "Violets are blue";
  close(FH);
  ```
## 13.7. Reading from STDIN
- if no file is mentioned as command line arguments, diamond operator ```<>``` in ```while``` loop reads from STDIN
- example
  - Let's implement a game of guess the price.
    - the user is asked to guess the price of rose.
    - if the guess is smaller than the actual price, then the program will respond with "Too small"
    - if the guess is greater then the actual price, then the program will respond with "Too large"
    - if the guess matches the actual price, the program will display "You guessed it right in <n> turns". n will be replaced with actual number of turns
  - let's say we invoke the Perl script with ```perl guess_price.pl```
  - the contents of the script is:
    ```perl
    my $number = int (rand (10)); # assign a random number to $number. rand function generates a random number
    my $turn = 0;
    while(my $guess = <>) {
      ++$turn;
      if ($guess == $number) {
        say "Puzzle master: You guessed the price right in <$turn> turns";
        last;
      } elsif ($guess < $number) {
        say "Puzzle master: Too small";
      } else {
        say "Puzzle master: Too large";
      }
    }
  ```

# 14. List operations - map, grep, sort

sort a hash
count number of words in a file

# 15. Regex



# 16. Importing subroutines

# 17. File and Directory management

- https://randu.org/tutorials/perl/filedir.php


# 18. Process management

- https://randu.org/tutorials/perl/process.php

# 19. Object Oriented Programming

# 20. Debugging

# 21. Idioms

# 22. Tail calls

# 23. some cool programs


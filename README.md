# Perl-interview-question-answers
Our Perl interview question and answer repository is a comprehensive collection of resources for anyone preparing for a Perl programming interview. In this frequently asked questions and their detailed answers, covering topics such as Perl syntax, data types, control structures, regular expressions, object-oriented programming, and more.
<table class="table">
  <thead>
    <tr>
      <th>NO</th>
      <th>Questions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th >1</th>
      <td><a href="#que1">What is Perl?</a></td>
    </tr> 
    <tr>
      <th >2</th>
      <td><a href="#que2">How do you comment a single or multiple lines of code in Perl?</a></td>
    </tr>
    <tr>
      <th >3</th>
      <td><a href="#que3">What is the difference between single and double quotes in Perl?</a></td>
    </tr>
    <tr>
      <th >4</th>
      <td><a href="#que4">What are the data types in Perl?</a></td>
    </tr>
    <tr>
      <th >5</th>
      <td><a href="#que5">Can you explain the scalar data type in Perl?</a></td>
    </tr>
    <tr>
      <th >6</th>
      <td><a href="#que6">Can you explain the hash data type in Perl?</a></td>
    </tr>
    <tr>
      <th >7</th>
      <td><a href="#que7">Can you explain the array data type in Perl?</a></td>
    </tr>
    <tr>
      <th >8</th>
      <td><a href="#que8">What are some scalar datatype operations in Perl?</a></td>
    </tr>
    <tr>
      <th >9</th>
      <td><a href="#que9">What are the array methods in Perl?</a></td>
    </tr>
    <tr>
      <th >10</th>
      <td><a href="#que10">How can you reset the starting index of an array in Perl?</a></td>
    </tr>
    <tr>
      <th >11</th>
      <td><a href="#que11">What is the difference between chop and chomp in Perl?</a></td>
    </tr>
    <tr>
      <th >12</th>
      <td><a href="#que12">How can you retrieve only values from a hash in Perl?</a></td>
    </tr>
    <tr>
      <th >13</th>
      <td><a href="#que13">How can you retrieve only keys from a hash in Perl?</a></td>
    </tr>
    <tr>
      <th >14</th>
      <td><a href="#que14">How can you check if a key exists or not in a hash in Perl?</a></td>
    </tr>
    <tr>
      <th >15</th>
      <td><a href="#que15">How can you check the size of a hash in Perl?</a></td>
    </tr>
    <tr>
      <th >16</th>
      <td><a href="#que16">How can you delete keys from a hash in Perl?</a></td>
    </tr>
    <tr>
      <th >17</th>
      <td><a href="#que17">How can you delete the last character from all the elements in an array in Perl?</a></td>
    </tr>
    </tbody>
</table>
<div class="common" id="que1" >
  <h3>1. What is Perl?</h3>
  <p>Perl is a high-level programming language that was originally designed for text manipulation and is known for its powerful regular expression capabilities. It was created by Larry Wall in 1987 and has since evolved into a versatile language used for a wide range of tasks, including system administration, web development, database programming, and more.<p/>

  <p>Perl is a cross-platform language, meaning that it can be run on a variety of operating systems, including Linux, Windows, macOS, and more. It is an interpreted language, which means that code written in Perl is executed directly by the interpreter, rather than being compiled into machine code beforehand.</p>

  <p>Perl is also notable for its large and active community of developers, who have created a vast library of modules and extensions to the language, making it easy to build complex applications quickly and efficiently. Overall, Perl is a powerful and flexible language that has become a staple of many industries and continues to evolve to meet new challenges.</p>
</div>
<div class="common" id="que2" >
  <h3>2. How do you comment a single or multiple lines of code in Perl?</h3>
  <p>In Perl, you can comment a single line of code by starting the line with the '#' character.</p>
  <p>Example :</p>
  
  ```
    # This is a comment in Perl
    print "Hello, World!\n"; # This line prints "Hello, World!"
  ```

  <p>To comment multiple lines of code, you can use the =head and =cut directives to create a block of documentation. Any code between these directives will be ignored by the interpreter.</p>
  <p>Example :</p>
  
  ```
    =head
    print "Welcome\n";
    print "Hello, World!\n"; 
    =cut
  ```
</div>

<div class="common" id="que3" >
  <h3>3. What is the difference between single and double quotes in Perl?</h3>
  <p>Single quotes</p>
  <p>Single quotes are not interpolated string literals, meaning that they lose their meaning.</p>
  <p>Example :</p>
  
  ```
    my $value = 45;
    print 'The value is $value \n';
  ```
  
  ```
    #output
    The value is $value #it will not print the 45 beacuse it lose their meaning.
  ```
  <br/>
  <p>Double quotes</p>
  <p>Double quotes are interpolated string literals, meaning that they not lose their meaning.</p>
  <p>Example :</p>
  
  ```
    my $value = 45;
    print "The value is $value \n";
  ```
  
  ```
    #output
    The value is 45 #it will print the 45 beacuse it not lose their meaning.
  ```

  <p>In double quotes we need to lose the meaning then use black slash (\)</p>
  <p>Example :</p>
  
  ```
    my $value = 45;
    print 'The value is \$value'
  ```
  
  ```
    #output
    The value is $value #it will not print the 45 beacuse it lose their meaning.
  ```
</div>
<div class="common" id="que4" >
  <h3>4. What are the data types in Perl?</h3>
  <p>There are 3 data types</p>
  <ul>
    <li>scalar</li>
    <li>hash</li>
    <li>array</li>
  </ul>
</div>
<div class="common" id="que5" >
  <h3>5. Can you explain the scalar data type in Perl?</h3>
  <p>In Perl, a scalar is a variable that can hold a single value of one of several different data types.</p>
  <p>scalars are variables that can hold a single value of various data types, including numbers, strings, booleans, and undefined values. They are declared using the $ symbol followed by the variable name and can be assigned and accessed using standard variable assignment and access syntax.</p>

  <p>Example :</p>
  
  ```
    my $name = "Suraj";  # Declares a scalar variable named $name with the value "Alice"
    my $age = 24;        # Declares a scalar variable named $age with the value 30
    my $is_developer = 1;  # Declares a scalar variable named $is_student with the value 1 (true)
    my $address;         # Declares a scalar variable named $address with an undefined value
  ```
  <p>You can assign a value to a scalar variable using the assignment operator " = "</p>
  <p>Example :</p>
  
  ```
    $name = "Vijay";      # Assigns the value "Vijay" to the $name variable
    $age = $age + 1;    # Increments the value of $age by 1
    $is_developer = 0;    # Assigns the value 0 (false) to $is_student
  ```
  <p>You can access the value of a scalar variable by simply using its name.</p>
  
  ```
    print $name;      # Prints the value of $name (currently "Bob")
    print $age;       # Prints the value of $age (currently 31)
    print $is_student # Prints the value of $is_student (currently 0)
  ```

</div>
<div class="common" id="que6" >
  <h3>6. Can you explain the hash data type in Perl?</h3>
  <p>In Perl, a hash is a data structure that allows you to associate keys with values, similar to a dictionary or map in other programming languages. Each key in a hash is unique and corresponds to a single value.</p>
  <p>Hashes are declared using the % symbol followed by the variable name</p>

  <p>Example :</p>
  
  ```
    my %person = (
      "name" => "Suraj",
      "age" => 24,
      "is_developer" => 1
    );
  ```
  <p>In this example, we have declared a hash named %person with three keys ("name", "age", and "is_student"), each of which corresponds to a value.</p>
  <p>You can access the value of a hash element using the key name in square brackets</p>
  <p>Example :</p>

  ``` 
    print $person{"name"};         # Prints the value of the "name" key (currently "Alice")
    print $person{"age"};          # Prints the value of the "age" key (currently 30)
    print $person{"is_student"};   # Prints the value of the "is_student" key (currently 1)
  ```

  <p>You can also assign a new value to a hash element using the key name and the assignment operator '='.</p>
  
  ```
    $person{"name"} = "Bob";      # Assigns the value "Bob" to the "name" key
    $person{"age"} = $person{"age"} + 1;  # Increments the value of the "age" key by 1
    $person{"is_student"} = 0;    # Assigns the value 0 (false) to the "is_student" key
  ```

</div>
<div class="common" id="que7" >
  <h3>7. Can you explain the array data type in Perl?</h3>
  <p>In Perl, an array is a data structure that can store a collection of values. Each value in an array is assigned a numeric index, starting from 0 for the first element, and increasing by 1 for each subsequent element.</p>
  <p>Arrays are declared using the @ symbol followed by the variable name.</p>

  <p>Example :</p>
  
  ```
    my @numbers = (1, 2, 3, 4, 5);

  ```
  <p>In this example, we have declared an array named @numbers with five elements, each of which corresponds to a numeric index.</p>
  <p>You can access the value of an array element using the numeric index in square brackets./p>
  <p>Example :</p>

  ``` 
    print $numbers[0];     # Prints the first element of the array (currently 1)
    print $numbers[2];     # Prints the third element of the array (currently 3)
    print $numbers[4];     # Prints the fifth element of the array (currently 5)
  ```

  <p>You can also assign a new value to an array element using the numeric index and the assignment operator '='.</p>
  
  ```
    $numbers[0] = 10;     # Assigns the value 10 to the first element of the array
    $numbers[2] = $numbers[2] + 1;   # Increments the value of the third element of the array by 1
    $numbers[4] = "five";  # Assigns the string "five" to the fifth element of the array
  ```

</div>
<div class="common" id="que8" >
  <h3>8. What are some scalar datatype operations in Perl?</h3>
  <p>Here are some of the most common scalar datatype operations in Perl:</p>

  <p>1. Assignment: The assignment operator "=" is used to assign a value to a scalar variable.</p>

  <p>Example :</p>
  
  ```
    my $num = 10;
    my $str = "Hello, world!";

  ```  
  <p>2. Arithmetic operators: Perl provides a variety of arithmetic operators for scalar variables, including "+", "-", "*", "/", and "%".</p>

  <p>Example :</p>
  
  ```
    my $a = 10;
    my $b = 5;

    my $sum = $a + $b;
    my $diff = $a - $b;
    my $prod = $a * $b;
    my $quot = $a / $b;
    my $mod = $a % $b;

  ``` 
  <p>3. String operators: Perl provides several operators for working with strings, including concatenation (".") and repetition ("x").</p>

  <p>Example :</p>
  
  ```
    my $str1 = "Hello, ";
    my $str2 = "world!";

    my $str3 = $str1 . $str2;   # Concatenation, Output : Hello, world!
    my $str4 = $str1 x 3;       # Repetition Output : Hello, Hello, Hello, 

  ```
  <p> 4. Comparison operators: Perl provides several comparison operators for scalar variables, including "==", "!=", "<", "<=", ">", and ">=".</p>

  <p>Example :</p>
  
  ```
    my $a = 10;
    my $b = 5;

    my $result1 = $a == $b;     # Equality
    my $result2 = $a != $b;     # Inequality
    my $result3 = $a > $b;      # Greater than
    my $result4 = $a <= $b;     # Less than or equal to 

  ```
  <p> 5. Logical operators: Perl provides several logical operators for scalar variables, including "&&" (logical AND), "||" (logical OR), and "!" (logical NOT).</p>

  <p>Example:</p>
  
  ```
    my $a = 10;
    my $b = 5;

    my $result1 = $a > $b && $a < 20;    # Logical AND
    my $result2 = $a < $b || $a == 10;   # Logical OR
    my $result3 = !($a == $b);           # Logical NOT
    
  ```


</div>

<div class="common" id="que9" >
  <h3>9. What are the array methods in Perl?</h3>
    <p></p>
<p>1. push() Adds one or more elements to the end of an array.</p>
  
    
      my @fruits = ('apple', 'banana');
      push(@fruits, 'orange');
      print "@fruits"; # Output: apple banana orange

   
<p>2. pop(): Removes and returns the last element of an array.</p>

   
      my @fruits = ('apple', 'banana', 'orange');
      my $last_fruit = pop(@fruits);
      print "$last_fruit"; # Output: orange

<p>3. shift(): Removes and returns the first element of an array.</p>

   
      my @fruits = ('apple', 'banana', 'orange');
      my $first_fruit = shift(@fruits);
      print "$first_fruit"; # Output: apple

   
<p>4. unshift(): Adds one or more elements to the beginning of an array.</p>

   
      my @fruits = ('banana', 'orange');
      unshift(@fruits, 'apple');
      print "@fruits"; # Output: apple banana orange

   
 <p>5. splice(): Removes or replaces a portion of an array.</p>

    
      my @fruits = ('apple', 'banana', 'orange', 'grape', 'kiwi');
      splice(@fruits, 2, 2, 'pear', 'peach');
      print "@fruits"; # Output: apple banana pear peach kiwi

  
 <p>6. join(): Concatenates the elements of an array into a single string, using a specified delimiter.</p>

   
      my @fruits = ('apple', 'banana', 'orange');
      my $fruits_string = join(', ', @fruits);
      print "$fruits_string"; # Output: apple, banana, orange

    

<p>7. split(): Splits a string into an array, using a specified delimiter.</p>

   
      my $fruits_string = 'apple, banana, orange';
      my @fruits = split(', ', $fruits_string);
      print "@fruits"; # Output: apple banana orange

   
<p>8. sort(): Sorts the elements of an array in ascending order.</p>


      my @fruits = ('banana', 'orange', 'apple');
      my @sorted_fruits = sort(@fruits);
      print "@sorted_fruits"; # Output: apple banana orange

    
<p>9. reverse(): Reverses the order of elements in an array.</p>


      my @fruits = ('apple', 'banana', 'orange');
      my @reversed_fruits = reverse(@fruits);
      print "@reversed_fruits"; # Output: orange banana apple

   
<p>10. grep(): Returns a list of all elements in an array that match a specified condition.</p>

    
      my @fruits = ('apple', 'banana', 'orange', 'pear', 'peach');
      my @selected_fruits = grep(/p/, @fruits);
      print "@selected_fruits"; # Output: apple grape peach

    
<p>11. map(): Returns a new list of elements that result from applying a function to each element in an array.</p>

    
      my @fruits = ('apple', 'banana', 'orange');
      my @uppercase_fruits = map(uc, @fruits);
      print "@uppercase_fruits"; # Output: APPLE BANANA ORANGE

    
<p>12. slice(): Returns a specified portion of an array as a new array.</p>

    
      my @fruits = ('apple', 'banana', 'orange', 'pear', 'peach');
      my @selected_fruits = @fruits[1..3];
      print "@selected_fruits"; # Output: banana orange pear

   

</div>
<div class="common" id="que10" >
  <h3>10. How can you reset the starting index of an array in Perl?</h3>
  <p>In Perl, you can reset the starting index of an array by changing the value of the $[ variable. By default, the starting index of arrays in Perl is 0, but you can change it to any integer value.</p>
  <p>However, it is not recommended to use `$[` in modern Perl programming because it can cause confusion and make code harder to maintain. Instead, you can use the use feature 'array_base'; pragma to set the starting index of arrays in a Perl script.</p>
  <p>Here's an example of how to reset the starting index of an array to 1 in Perl:</p>

  ```
    use feature 'array_base';
    $[ = 1; # set starting index of arrays to 1

    my @fruits = ('apple', 'banana', 'orange');
    print "$fruits[1]\n"; # Output: apple
    print "$fruits[2]\n"; # Output: banana
    print "$fruits[3]\n"; # Output: orange

  ```

</div>
<div class="common" id="que11" >
  <h3>11. What is the difference between chop and chomp in Perl?</h3>
  <p>chop and chomp are two Perl built-in functions that are used to remove characters from the end of a string. However, there is a difference in how they work.</p>
  <h5>chop:</h5>
  <p>chop removes the last character of a string, regardless of what it is. It modifies the string in place and returns the character that was removed.</p>

  <p>Example</p>

  ```
    my $string = "hello";
    my $last_char = chop($string);
    print "$string\n";     # Output: hell
    print "$last_char\n";  # Output: o

  ```
  <p>In this example, we use chop to remove the last character 'o' from the string "hello". The chop function modifies the string in place and returns the character that was removed, which is then printed to the screen.</p>

   <h5>chomp:</h5>
   <p>chomp, on the other hand, is used to remove the newline character(s) from the end of a string. It only removes the newline character(s) that appear at the end of the string, and leaves any other characters intact. Here's an example:</p>

   ```
      my $string = "hello\n";
      chomp($string);
      print "$string";   # Output: hello

   ```
   <p>In this example, we use chomp to remove the newline character \n from the end of the string "hello\n". The chomp function removes the newline character and modifies the string in place.</p>
</div>

<div class="common" id="que12" >
  <h3>12. How can you retrieve only values from a hash in Perl?</h3>
  <p>To retrieve only the values from a hash in Perl, you can use the values function. The values function returns a list of all the values in the hash.</p>

  ```
      my %person = (
          "name" => "John Smith",
          "age"  => 30,
          "city" => "New York"
      );

      my @values = values %person;  # Retrieve all values from hash

      print "Values: @values\n";

  ```
</div>

<div class="common" id="que13" >
  <h3>13. How can you retrieve only keys from a hash in Perl?</h3>
  <p>To retrieve only the keys from a hash in Perl, you can use the keys function. The keys function returns a list of all the keys in the hash.</p>

  ```
      my %person = (
          "name" => "John Smith",
          "age"  => 30,
          "city" => "New York"
      );

      my @keys = keys %person;  # Retrieve all keys from hash

      print "Keys: @keys\n";

  ```

</div>

<div class="common" id="que14" >
  <h3>14. How can you check if a key exists or not in a hash in Perl?</h3>
  <p>To check if a key exists or not in a hash in Perl, you can use the exists function. The exists function returns a true value if the specified key exists in the hash and a false value otherwise.</p>

  ```
    my %person = (
        "name" => "John Smith",
        "age"  => 30,
        "city" => "New York"
    );

    if (exists $person{"name"}) {
        print "Name exists in hash\n";
    } else {
        print "Name does not exist in hash\n";
    }

  ```

</div>

<div class="common" id="que15" >
  <h3>15. How can you check the size of a hash in Perl?</h3>
  <p>In Perl, you can use the scalar function to get the size of a hash. When used with a hash variable, the scalar function returns the number of key-value pairs in the hash.</p>

  ```
    my %person = (
        "name" => "John Smith",
        "age"  => 30,
        "city" => "New York"
    );

    my $size = scalar %person;  # Get size of hash

    print "Size of hash: $size\n"; #output: Size of hash: 3

  ```

</div>
<div class="common" id="que16" >
  <h3>16. How can you delete keys from a hash in Perl?</h3>
  <p>In Perl, you can use the delete function to remove a key-value pair from a hash. The delete function takes the hash and the key as arguments and returns the value associated with the deleted key.</p>

  ```
    my %person = (
        "name" => "John Smith",
        "age"  => 30,
        "city" => "New York"
    );

    delete $person{"age"};  # Delete key "age"

    print "After deleting 'age':\n";
    while (my ($key, $value) = each %person) {
        print "$key => $value\n";
    }

  ```
  <p>Output:</p>

   
    After deleting 'age':
    name => John Smith
    city => New York

</div>
<div class="common" id="que17" >
<h3>17. How can you delete the last character from all the elements in an array in Perl?</h3>
  
  ```
  my @array = ("apple", "banana", "cherry");
  chop(@array);
  print "@array\n"; #output: appl banan cherr
  
  ```
  <p>In the above example deleted all the last letters.
</div>

# CSE 2312 | Computer Organization and Assembly Programming Language Class | University of Texas at Arlington

## calculator.s | Description

Programmed a simple calculator for the Raspbian OS using ARM Assembly. The program consists of the following procedure calls: SUM, DIFFERENCE, PRODUCT and MAX.<br/>

The main function consists of a loop that continuously checks for keyboard input in the following pattern:<br/>
<OPERAND_1><ENTER><br/>
<OPERATION_CODE><ENTER><br/>
<OPERAND_2><ENTER><br/><br/>
  
where <OPERATION_CODE> can be any of the four characters {+, -, *, M}.<br/><br/>

Below are some example use cases:<br/>

|               |               |               |               |
| ------------- |:-------------:| -------------:| -------------:|
| 5             | 100           | 5             | 50            |
| +             | M             | *             | -             |
| 15            | 200           | 20            | 20            |
| 20 <- result  | 200 <- result | 100 <- result | 30 <- result  |
<br/><br/>

# integerPartition.s | Description

Implemented a recursive solution for computing the number of integer partitions of a positive integer *n* with parts up to *m*. In number theory, an integer partition is a way of writing *n* as a sum of positive integers (in this case, positive integers up to *m*). For example, the partitions for *n* = 5 and *m* = 3 are:<br/>
5 = 1 + 1 + 1 + 1 + 1<br/>
5 = 2 + 1 + 1 + 1<br/>
5 = 2 + 2 + 1<br/>
5 = 3 + 1 + 1<br/>
5 = 3 + 2<br/><br/>


The main function contains a loop that continuously checks for keyboard input in the following pattern:<br/>
<OPERAND_N><ENTER><br/>
<OPERAND_M><ENTER><br/><br/>

All input test cases will consist of positive numbers only, and OPERAND_M will always be less than or equal to OPERAND_N. Below is how the input/output should look for the example above:<br/>
<pre>       `5`</pre><br/>
<pre>       `3`</pre><br/>
Result ->   `There are 5 partitions of 5 using integers up to 3`<br/><br/>


# sortRandomNumbers.s | Description

iteratively populated a fixed-size array of 20 elements, "array_a", with values provided by a "generate" function. Once "array_a" has been populated by "generate", the program then stores and sorts the values in increasing order into "array_b", a second fixed-size integer array of 20 elements. The generate function is described (in C) below:<br/>

`void generate(int n) {`<br/>
<pre><code>  for(int i=0; i<20; i+=2) {</code></pre>
<pre><code>    array_a[i] = n+i;</code></pre>
<pre><code>    array_a[i+1] = -(n+i+1);</code></pre>
<pre><code>  }</code></pre>
`}`<br/>

# arrayFunctions.s | Description


Iteratively populated a fixed-size integer array of 10 elements, array_a, with integer values provided by scanf. The user will enter 10 integer values, one per line, and the program will store the 10 values in array_a[0], array_a[1], …, array_a[9]. Once all of the integers are entered, the program will then calculate the minimum and maximum values in the array, and also the sum of values in the array. Finally, the entire contents of the array will be printed followed by the minimum value, maximum value, and overall sum.

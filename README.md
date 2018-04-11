# CSE 2312 | Computer Organization and Assembly Programming Language Class | University of Texas at Arlington

## Calculator.s | Description

Programmed a simple calculator for the Raspbian OS using ARM Assembly. The program consists of the following procedure calls: SUM, DIFFERENCE, PRODUCT and MAX.<br/>

The main function consists of a loop that continuously checks for keyboard input in the following pattern:<br/>
<OPERAND_1><ENTER><br/>
<OPERATION_CODE><ENTER><br/>
<OPERAND_2><ENTER><br/><br/>
  
where <OPERATION_CODE> can be any of the four characters {+, -, *, M}.<br/><br/>

Below are some example use cases:<br/>

 | 5 | 100 | 5 | 50
 | + | M | * | -
 | 15 | 200 | 20 | 20
 result | 20 | 200 | 100 | 30

# | Description

Implemented a recursive solution for computing the number of integer partitions of a positive integer "n" with parts up to "m". In number theory, an integer partition is a way of writing "n" as a sum of positive integers (in this case, positive integers up to m). For example, the partitions for n = 5 and m = 3 are:
5 = 1 + 1 + 1 + 1 + 1
5 = 2 + 1 + 1 + 1
5 = 2 + 2 + 1
5 = 3 + 1 + 1
5 = 3 + 2


The main function contains a loop that continuously checks for keyboard input in the following pattern:
<OPERAND_N><ENTER>
<OPERAND_M><ENTER>

All input test cases will consist of positive numbers only, and OPERAND_M will always be less than or equal to OPERAND_N. Below is how the input/output should look for the example above:
            5
            3
Result ->   There are 5 partitions of 5 using integers up to 3


# | Description

iteratively populated a fixed-size array of 20 elements, "array_a", with values provided by a "generate" function. Once "array_a" has been populated by "generate", the program then stores and sorts the values in increasing order into "array_b", a second fixed-size integer array of 20 elements. The generate function is described (in C) below:
void generate(int n) {
  for(int i=0; i<20; i+=2) {
    array_a[i] = n+i;
    array_a[i+1] = -(n+i+1);
  }
}



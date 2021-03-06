# DBSys-lab-2

## Context

This is the git repository associed with the work of Victor MASIAK and Hugo DANET regarding the part 2 of DBSys Lab Assignments (EURECOM 2020).

## Structure

This repository contains 4 directories :
* Reference : contains the assignment and the original paper.
* Code : contains the .java files created/modified for the assignment purpose.
* Output : contains the output of the BMTest2020.java execution, and some notes from Victor MASIAK and Hugo DANET.
* Complete project : contains all the files required to run the project.

## How to run the project

In order to run the test file, the following command will NOT work:

`javac javaminibase/src/tests/BMTest2020.java`

Indeed, due to errors in some files unrelated to the assignment, the code will not compile.We advise you to open it in Eclipse, and to run the tests/BMTest2020.java file: Eclipse will allow you to ignore the errors since the concerned files are not executed.

## Explanation

### FIFO

With this approach, the first page that was read to the memory buffer is considered for page replacement if its pin count=0.

### LIFO

With this approach, the last page that was read to the memory buffer is considered for page replacement if its pin count=0.

### LRUK



## How we structured the project

We tried to respect as much as possible the concepts of encapsulation and of delegation. Therefore, we created some additional classes in order to make it extra simple to upgrade to other data structures as suggested in the paper.

HistoricDataStructure contains a list of historics of each page. A page historic is implemented with the class Historic.
LastDataStructure contains a list of the last time each page has been accessed. The Last class contains the last time (long) a specific page has been accessed.

We implemented the LRU-K pseudo-code of the paper. We also implemented the time correlation to correlate some references.


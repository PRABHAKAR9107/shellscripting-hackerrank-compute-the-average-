# shellscripting-hackerrank-compute-the-average-
It is the hackerank problem.

#!/bin/bash

read n     #input from user

arr=($(cat))  #make an array

arr=${arr[*]}

printf "%.3f" $(echo $((${arr// /+}))/$n | bc -l)


# Reverse Input Number

Purpose of the this coding challenge is to write a script that reverse the given numbers.

## Learning Outcomes

At the end of the this coding challenge, students will be able to;

- analyze a problem, identify and apply programming knowledge for appropriate solution.

- design, implement `ìf` and `else` effectively in bash script to solve the given problem.

- apply arithmetic operations on basic data types in Bash Scripting.

- demonstrate their knowledge of algorithmic design principles by using function effectively.

## Problem Statement

- Write a shell script to print the reverse of an input number.

Example:

input: 957105

output: 501759

## Solution1

#!/bin/bash

echo "Enter a number"

read n

sd=0

rev=0

while [ $n -gt 0 ]

do

    sd=$(( $n % 10 ))
    rev=`expr $rev \* 10 + $sd` 
    n=$(( $n / 10 ))
done

echo "Reverse number of entered digit is $rev"

## Solution2

#!/bin/bash


clear

read -p "Enter a number: " num

echo $num | rev



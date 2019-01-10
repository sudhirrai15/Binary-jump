# Binary-jump
Given a base-10 integer, , convert it to binary (base-2). Then find and print the base- 10 integer denoting the maximum number of consecutive 's in 's binary representation.
Pyhthon Programming Language:
import math
import os
import random
import re
import sys

if __name__ == '__main__':
    n = int(input())
    a = n
    count = 0
    max_val = 0
    while( a > 0):
        x = int(a%2)
        if (x == 1):
            count = count + 1
            if (count > max_val):
                max_val = count
        else :
            count = 0
        a = int(a/2)
    print(max_val)

        

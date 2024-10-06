#!/usr/bin/env python3
from sys import argv

# Open the file provided as the first argument
with open(argv[1]) as f:
    for line in f:
        num = int(line)
        print("{:d}=".format(num), end='')

        # Check if the number is even
        if num % 2 == 0:
            print("{}*2".format(num // 2))
            continue

        # Iterate through odd numbers to find factors
        for i in range(3, num, 2):
            if num % i == 0:
                factor = num // i

                # Find the next factor
                for j in range(3, factor, 2):
                    if factor % j == 0 or j == 0:
                        break

                print("{}*{}".format(factor, i))
                break

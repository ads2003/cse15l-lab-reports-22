# Lab Report 5

## Part 1

I'm attempting to develop a method that accepts an array as input and outputs a new array that has each and every entry from the input array. Instead of printing the first element in the original array, my code skips the first one and begins printing each subsequent element from the second one. I think there might be a problem with my for loop. This is a code screenshot.

Code:

<img width="1728" alt="Screenshot 2024-03-11 at 6 17 17 PM" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/ed1ff64d-e668-4eae-963f-518f405b5c3e">

Symptoms:

<img width="689" alt="Screenshot 2024-03-12 at 8 21 37 PM" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/5dd67d66-ee8f-4c94-88f7-2fc07ffb5efe">

## TA reponse 

Hello! Although your method appears to be OK, attempt to catch bugs in your loop while creating the new array.
Think about the way you are accessing elements by iterating across the input array. Verify again that you are accurately copying each additional piece into the result array! Tell me what you discover.

## Response of the Student after changes




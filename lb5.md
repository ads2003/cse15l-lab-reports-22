# Lab Report 5

## Part 1

I'm attempting to develop a method that accepts an array as input and outputs a new array that has each and every entry from the input array. Instead of printing the first element in the original array, my code skips the first one and begins printing each subsequent element from the second one. I think there might be a problem with my for loop. This is a code screenshot.

Code:

<img width="1728" alt="Screenshot 2024-03-11 at 6 17 17 PM" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/ed1ff64d-e668-4eae-963f-518f405b5c3e">

Symptoms:

<img width="570" alt="Screenshot 2024-03-12 at 8 34 22 PM" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/14c7e24b-ef8e-4d73-8846-71b1cd714ceb">


## TA reponse 

Hello! Although your method appears to be OK, attempt to catch bugs in your loop while creating the new array.
Think about the way you are accessing elements by iterating across the input array. Verify again that you are accurately copying each additional piece into the result array! Tell me what you discover.

## Response of the Student after changes

I appreciate the recommendations. After giving the code a closer look, I saw that it was adding 1 to the right mean, so I changed it to obtain the right mean.

## The directory Structures and the files

<img width="305" alt="Screenshot 2024-03-12 at 8 30 49 PM" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/8211a47d-4929-4dbe-b773-0263c0c50ea0">


## Correct Code 
<img width="493" alt="Screenshot 2024-03-12 at 8 33 38 PM" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/8c2357d3-b7b6-4cba-a636-2b1a26510546">

<img width="739" alt="Screenshot 2024-03-12 at 8 32 27 PM" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/55b98f1a-df42-45a4-8c0f-3f1d6589117d">

## Description of the edit code 

To fix the code I changed the code where 1 was added to the array length and removed the +1 

## Part 2

During the latter part of this quarter, I thoroughly acquired knowledge on using the vim command for editing. With this command, I discovered a variety of ways to alter my code and the keys I might hit to accomplish various tasks. 


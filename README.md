# Lab 4 – String Manipulation

This repo contains three scripts. All scripts were completed as Lab 4 String Manipulation for the Clark University course IDCE 302 Python Programming taught by Professor Shadrock Roberts. "Jess_Strzempko_String-Manipulation_Lab4-exercise1/2/3.ipynb" are based on the scripts "exercise 1/2/3.py" provided by the professor. 

### Problems Encountered

In script 1, I was having trouble coming up with the right approach to the function. Initially, I was planning to write a for loop with a counter and an if statement inside where if the index == 1 or 4 then I would use the `.upper()` function to modify this character. I realize when writing this that I can't re-assign values in strings while indexing, so I changed my approach to instead slice the string into the first 3 characters and the subsequent ones, use the `.capitalize()` function on both these segments, then concatenate the results. This method was best as it allows me to input strings of any length into the function. 

In script 2, I was having trouble understanding how I could apply a string manipulation technique to all the elements in the list using a for loop. My initial idea had been to index into the strings to add the necessary formatting characters, but as with script 1 this was not possible. After receiving help from the TA, I realized that I could apply the `.replace()` function to all the elements in the list because the function would essentially do nothing if the element did not contain the item it was set to replace. 

In script 3, I used indexing to slice the URL in the string. I was initially trying to think of an easier way to do so, or a method that was more generally applicable, but was unable to come up with such a method. I also used reverse indexing, as it was easier to count backward in the string than forward. 

## Script 1

This script contains a function that capitalizes the first and fourth letters of a name provided in a string. In this example, the function is called “old_macdonald” and takes a string for an argument. For example, running the function as `old_macdonald('macdonald')` would produce `MacDonald` as its output. Users are also given a change to run their own inputted string through the function. The function uses string indexing and capitalization to convert the string. 

## Script 2

This script works with a multiline string that has been scraped from the National Weather (NWS) Service website. Using string manipulation techniques, the multi-line string is edited to be outputted in a more understandable format. Specifically, the `.split()` and `.replace()` string manipulation functions are used within a for loop to place the multi-line string into a list before editing it through the addition of colons, spaces, and commas. The output appears as follows:
Tonight: Clear, Low: 55 F
Thursday: Sunny then Chance Showers, High: 77 F
Friday: Sunny, High: 73 F
Saturday: Mostly Sunny, High: 77 F
Sunday: Mostly Sunny, High: 71 F

## Script 3

This script takes a [Google Maps URL](https://www.google.com/maps/@42.2509428,-71.8249939,17z) as a string and extracts the latitude and longitude information from it. Reverse indexing is used to slice the string at relevant locations. Output text labels the values and appears as follows:
Latitude: 42.2509428
Longitude: -71.8249939

# The Code
Users can download and run the three python scripts "Jess_Strzempko_String-Manipulation_Lab4-exercise1/2/3.ipynb" in Colab notebooks. The first script takes a string and capitalizes certain portions of it. The second script parses and manipulates a multiline string. The third script extract a portion of a string and returns it in a way that is more understandable. These three scripts are created and edited from starter script included in the initial repo. If problems are encountered, users can contact Jess Strzempko at JeStrzempko@clarku.edu for more help and further information.

# Yelp, FourSquare, and Google Places APIs

### [Assignment](assignment.md)

## Project/Goals
The goal of this project was to compare and contrast the Foursquare and Yelp Places APIs, in terms of their ease of use, utility of the data (is it up to date, )

A secondary goal was to familiarize myself with sending GET requests in Python, parsing/wrangling the responses, and 
storing the results in a bespoke database.  

## Process
- ### Learning the APIs
    Not the most intuitive APIs I've ever used, and not the least intuitive either.  Getting a sample header from YELP
was insanely helpful, though, because there was a weird quirk in how they accept the key in the GET header.  
- ### Building the Get Requests
    See above. Was slightly more impressed by the ability to test the APIs than I was by the actual documentation of the
APIs.  The descriptions of the parameters may have been vague, but nothing clears up ambiguity like trial-and-error testing.
- ### Parsing/Wrangling the results
  The toughest part of the process.  Not because it was particularly difficult, but because it was time consuming.
It took some time to get a handle on how to parse the JSON contained in the response, because both APIs returned JSONs
with multiple levels, 
- ### Building & Populating a new Database
  SQLAlchemy and Pandas made this part straightforward, although I didn't quite figure out how to create primary/foreign
keys on related tables.  Definitely something to work on in the future.
- ### Querying the new Database
    I did this in two ways.  The first was using SQL directly in a Jupyter Notebook. The second was by using SQLAlchemy engines.
Doing it twice garnered the exact same results (as one would expect), I just felt it would be good practice to try
both methods!


## Results
(fill in what you found about the comparative quality of API coverage in your chosen area)

## Challenges 
By far, the biggest challenge in this project was combing through the API documentation 
## Future Goals
I would focus a bit more on database design, and see if there was a way to structure the database in the way that I 
wanted using SQLAlchemy rather than linking the tables and keys together the old fashioned way.  
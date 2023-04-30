Download Link: https://assignmentchef.com/product/solved-metcss521-homework5
<br>
For this week we are adding some new style requirements.

Up to this point, we have deducted for:

<ul>

 <li>Improper naming of programs or zip container

  <ul>

   <li>Among other things, names be all lower case</li>

  </ul></li>

 <li>Missing program docstring</li>

 <li>Inadequate # line comments

  <ul>

   <li>Just a few in each program – don’t excessively comment</li>

  </ul></li>

 <li>Going significantly over 80 characters for code/comment lines</li>

 <li>Using CamelCase or anything other than lower case plus underscores for variables and function names.

  <ul>

   <li>CONSTANT variables are the one exception and must be all upper case.</li>

   <li>Asking for input() without telling the user what is expected.</li>

  </ul></li>

 <li>Especially if asking for input that will be split(). Don’t make users have to check the code!</li>

 <li>x = input(‘Enter two numbers:’) # Vague</li>

 <li>Printing output that isn’t clearly explained (where necessary)</li>

</ul>




Starting with Homework 5, we will also be deducting for:

<ul>

 <li>Not providing a docstrings for functions and class objects</li>

 <li>Crashing uncontrolled on bad user input</li>

 <li>Having too large a scope for try blocks</li>

 <li>Not using format() to round output and add thousand separating commas (US standards)</li>

 <li>126 should be 123,456.13 è ‘{:,.2f}’.format(123456.126)</li>

 <li>Having a “main()” function, with no input arguments or return values</li>

 <li>Not using an if __name__ == ‘__main__’ block where appropriate</li>

</ul>

<strong> </strong>

<strong>Chapter 5 Exercises</strong>

<strong>5.5.1:</strong>  Write a python program that does the following:

<ul>

 <li>takes as input from the user an English sentence</li>

 <li>calls the function vc_counter() that:

  <ul>

   <li>takes a string argument</li>

   <li>counts the number of vowels and consonants in the string</li>

   <li>returns a dictionary of the counts, using the keys total_vowels and total_consonants</li>

  </ul></li>

 <li>Uses the return from vc_counter() to print the total vowels and consonants with appropriate descriptions.</li>

</ul>

Example:

Enter an English sentence: The quick brown fox’s jump landed past the lazy dog!Total # of vowels in sentence: 12Total # of consonants in sentence: 29

<strong>5.5.2:</strong>   Write a python program that does the following:

<ul>

 <li>takes as input from the user a date and time (24-hour clock) as “MM/DD/YYYY HH:mm:SS”

  <ul>

   <li>Assume that everything must be provided with leading zeros</li>

  </ul></li>

 <li>calls the function is_ validate_datetime () that:

  <ul>

   <li>takes a string argument</li>

   <li>validates that the string has all the elements to be a valid date and time</li>

   <li>returns 2 values:

    <ul>

     <li>Boolean true if valid or false if invalid date/time</li>

     <li>None if valid or an error message string if invalid</li>

    </ul></li>

   <li>If the input string is returned from the function as invalid, print the returned error message.</li>

   <li>If the input string is returned from the function as valid, use input string to print following:

    <ul>

     <li>MM/DD/YYYY</li>

     <li>HR:MIN:SEC</li>

     <li>MM/YYYY</li>

     <li>Whether the time is “AM” or “PM”</li>

    </ul></li>

  </ul></li>

</ul>




<strong>You must write your own algorithms. Do not use existing functions like datetime.strptime</strong>




Example 1:

Enter a date time (MM/DD/YYYY HR:MIN:SEC): 12/13/2020 11:31:41MM/DD/YYYY is 12/13/2020

HR:MIN:SEC is 11:31:41

MM/YYYY is 12/2020The time is AM




Example 2:

Enter a date time (MM/DD/YYYY HR:MIN:SEC): 122/04/1990 13:12:12Invalid: there can be only 12 months in a year.

<em>Think of all possible erroneous inputs and write code to handle them. </em>




<strong> </strong>

<strong> </strong>

<strong>Chapter 6 Exercise</strong>




<strong>5.6.3    </strong>Write a python program that does the following:

Prompts the user for three numbers in one request.<em>Be sure to specify the “delimiter” by which a user enters those three numbers.</em>Divides the first number by the second number and add that result to the third number.

Prints output that shows in one line the formula applied and the result of the calculation.

Validate input by:

<ul>

 <li>Checking the user entered 3 values</li>

 <li>Appropriately checking for the following errors: ValueError and ZeroDivisionError.</li>

 <li>Printing descriptive error messages to the console if validation fails.</li>

</ul>

<ul>

 <li>Remembering to have very granular testing blocks</li>

</ul>

<em>No Example Output provided for this question.</em><em></em>



<strong> </strong>

<strong> </strong>

<strong>Chapter 8 Exercise</strong>




<strong>5.8.4:</strong>   Write a python program that does the following:

Prompt for a file name of text words.Words can be on many lines with multiple words per line.

Read the file and convert the words to a list.

Call a function you created called list_to_words(), that takes a <strong>list</strong> as an argument and returns a <strong>list</strong> that contains only words that occurred once in the file.

Print the results of the function with an appropriate description.

<em>Think about everything you must do when working with a file.</em>

<em>No Example Output provided for this question.</em>

<strong> </strong>

<strong> </strong>

<strong>Chapter 15 Exercise</strong>




<strong>5.15.5: </strong>The formula for calculating the amount of money in a savings account that begins with an initial principal value (P) and earns annual interest (i) for (n) years is: P(1 + i)<sup>n</sup>Note that i is a decimal, not a percent interest rate: .1 NOT 10%




Write a python program that does the following:

<ul>

 <li>Prompt the user on three lines for principal, percent interest rate and number of years to invest (using descriptive prompts)

  <ul>

   <li>Use a while loop to keep prompting until entries are valid</li>

  </ul></li>

 <li>Call your function calc_compound_interest() that:

  <ul>

   <li>takes the arguments principle, int_rate, years</li>

   <li>uses the above formula to calculate the ending value of the account</li>

   <li>returns the value</li>

  </ul></li>

 <li>Call a second function calc_compound_interest_recursive() that:

  <ul>

   <li>takes the arguments principle, int_rate, years</li>

   <li>calculates the value <strong>recursively</strong> – calling a base calculation over and over instead of using the number of year as an exponent.</li>

   <li>return that value</li>

  </ul></li>

 <li>Print both values with clear descriptions and formatted with thousand commas and 2 decimal places. Then print whether the two values are equal when rounded to 4 decimal places.</li>

</ul>


















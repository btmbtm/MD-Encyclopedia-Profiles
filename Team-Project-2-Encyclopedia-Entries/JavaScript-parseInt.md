#JavaScript
##parseInt() function


In JavaScript, the `parseInt()` function is used to convert number strings to integers. If the argument passed is a number and not a string, the `parseInt()` function will convert the argument to a String and then convert it again to an integer. This function is useful when you need to retrieving and convert data from the DOM, which is always passed as strings. For instance, a form submission which contains a number might need to be converted to a number to apply a mathematical caluclation to it. 


###Syntax

`parseInt(string, radix);`

- The first parameter is the string to be passed. 

- The second parameter represents the mathematical base which you are using. 10 should be specified unless you are specifically using another base system for instance - octal or binary. It is good practice to include the radix, without doing so the results of the function might not be reliable, because `parseInt()`'s default base behavior varies by the supplied JavaScript implementation. 

 <hr>
 
 When supplied a different radix, `parseInt()` returns a calculation based on this radix rather than the default: 

 	
 	parseInt("0101",2) //5
 	
 	parseInt(0101,2) //NaN
    
    parseInt("0101.4",2) //5
	
	parseInt("00101.4",2) //5


###Things to remember:


**Rounding** - When passed a radix of 10, and a floating point number `parseInt()` only returns the integer which occurs before the decimal. (`parseInt(01.5) // Returns 1`)

**Whitespace** - leading whitespace is ignored. (`parseInt(     01.5) // Returns 1`)

**First Character** - If the first character cannot be converted to a number, parseInt() returns NaN.

<br>

###Browser Support
<table>
	<tr>
		<th>Feature</th>
			<th>Chrome</th>
			<th>Firefox / (Gecko)</th>
			<th>Internet Explorer</th>	
			<th>Opera</th>
			<th>Safari</th>
		<tr>
			<td>Basic support</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Unknown</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Parses leading-zero strings as decimal, not octal</td>
			<td>Yes</td>
			<td>Version 21 and up</td>
			<td>(Yes) (in standards mode)</td>
			<td>Unknown</td>
			<td>Yes</td>
		</tr>
</table>
			
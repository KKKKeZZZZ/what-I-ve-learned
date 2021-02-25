# what-I-ve-learned
This project is to record what I've learned during my working. May include .net, c#, js & css. (need to learn how to format this file)

//09022021

#1. using jQuery UI addon, if you import the add on script package before the main jQuery package, it will cause undefined type error.

   WIL: import package order matters!
   
//10022021   
#2. using jQuery to get an empty value of the html input, its value is ""(empty string), not null

   WIL: detect empty for empty value using .val() == ""
   
//12022021

#3. ajax using datatype json but in the handler page you return a value but not in json format, in the ajax side it will jump to error section. 

   WIL: so the functional code will be implemented in error scope using function(xht, status, error), 
   
   and the return value can be accessed via the xhr.responseText  
   
   p.s. i dont know which genius code in this way, it actually killed tons of my time
   
//17022021 

#4. when using json format data, the tab value is the poison, it will crush the whole json, but users ALWAYS like it.

   WIL: for my case, I will remove all tab values in the string I wanna write to db. here it is "	"
   
//23022021

#5. When using ajax, the 'success' section cannot be using as 'Success'!
   
   WIL: CASE SENSITIVE!

//26022021 

#6. attribute selector is useful. For example: 

   "$('td[name ="tcol1"]')   // matches exactly 'tcol1'
   $('td[name^="tcol"]' )   // matches those that begin with 'tcol'
   $('td[name$="tcol"]' )   // matches those that end with 'tcol'
   $('td[name*="tcol"]' )   // matches those that contain 'tcol'"

   Then use this.name.substring() to get the specific attibute of the element you want. Then you can set all elements at the same time.
 
   p.s. I hope I can know this two weeks ago

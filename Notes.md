Just in case reader doen't know:

HTML formates the web content.
CSS adds styling 

And JavaScript adds interaction.

1) Open Inspect -> Click console -> console.log("Hi!"); [It will display Hi! and in next line it will show undefined]

console.log() does the work of printing and is useful for debugging, NOTE THE SEMICOLON(;) at the end and undefined tells us 
that we donot have any data to save when running console.log()

document.URL gives string which is basically where url resides.

2) open [Udacity Static Site](http://udacity.github.io/js-basics/static-home/index.html), in console type:
        $(".super-header-wrapper").html("<img style='width:100%' src='http://goo.gl/WCrBmS'>");
        
        $("") indicates the use of jquery. in above code it grabs the element on the page identified by .super-hearder-wrapper
        and replace the given image by image provided in <img> tag by running html method on it. (see by pasting http://goo.gl/WCrBmS in your webbrowser)
        
        Note it will only make changes in local copy not the actual copy
3) Go to resumeBuilder.js and write $("#header").append() where # tells us we are looking for id name header. 
".append()" will put the content to end of the file(as is the case with python)

Do it like this,

$("#main").append("Shivangi")
this should display Shivangi on screen

Don't forget "$" sign is the jquery selector.

4) Like in python, in browser console one can do simple calculations

5) To declare a new variable in JS :
              var {{variable name}} = {{somevalue}}  #great new no worries about floating points :) and all numbers are stored as 64 bit floating point

In resumeBuilder.js type following:
    var awesomeThoughts = "Hey!"
    console.log(awesomeThoughts)
    
    save it and run index.html

#TO clear your console type clear()

Also note there is also  .prepend() method which seems to be self-explanatory.

6) Arrays in JavaScript:
    JavaScript Arrays are ZeroIndexed.(They are similar to list in python)
    var myArray = ["Hi","What's Up"]
    this creates an array
    
    And the using append it can be seen on page.
    
Quiz:

var sampleArray = [0,0,7];

var incrementLastArrayElement = function(_array) {
    var newArray = [];
    // Your code should make newArray equal to an array that has the same
    // values as _array, but the last number has increased by one.
    
    // For example:
    // _array = [1, 2, 3];
    // turns into:
    // newArray = [1, 2, 4];
    newArray = _array
    
    var lastnumber = newArray.pop();
    newArray.push(lastnumber + 1);
    
    //newArray.push(lastNumber + 1);
    // Don't delete this line!
    return newArray;
};

// Did your code work? The line below will tell you!
console.log(incrementLastArrayElement(sampleArray));


Arrays are objects in javascript, therefore its properties can be excessed.

7) There are NO CLASSES in javascript, just objects.

var bio = {

	"name" : "James",
	"age" : 32,
	"skills" : skills
};

$("#main").append(bio.name)

// with dot notation no need to add var, we are adding properties to object
bio.city = "Mountatin View";

8) JSON(JavaScript Object Notation): 













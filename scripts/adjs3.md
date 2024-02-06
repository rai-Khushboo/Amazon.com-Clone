**This reference is about the Amazon project**

dataset attribute gives all the properties related to that object

**data attribute starts with the name syntax for data attribute it's an attribute of an HTML have to start with data followed by any other name**


**The dataset property allows you to access the values of data attributes by converting them from the kebab-case format (e.g., data-product-name) to camelCase (e.g., productName).**


\\using script tag produces naming conflicts of variable within different files therefore to solve this problem a feature of javascript is used known as modules

<!-- To reduce naming conflicts modules are used  -->
modules contains variable inside a file therefore it's not going to cause conflict with anyone outside the file 
**How to create a module**
s1:Delete the script tag from your file or don't load file using script tag.
(by deleting this variable we are no longer creating a separate file therefore there is no chance of naming conflict.)

**getting a variable out of a file**
1.Add type="module" attribute
=>Let's this file get variables out of other file i.e dusre file ke variables ko access kr skte hain
2.Export 
=go to that fle and write the word export infront of the variable to get that.
3.Import
=import the variable by locating the path 
jha pe variable ko use krna ho vha pe import kr lo 

**../ is used to get out from that folder**

**./ represents the current folder**

**//modules always work when we open (file) it with live server else it'll not work.**

<!-- while using module in our file we rename the variable like:
cart as myCart here cart variable will be used as myCart. 
Now the same variable can be used with the different name-->


**Normalising the data or de-duplicating**
Here we use product id to access the data ,rest other things are accessed using the id we switched into the products arrays.

**To save our cart we'll use localstorage**
Local sorage can only saves strings therefore objects are converted into strings using JSON.stringify


**external libraries-code outside our project is known as external libraries**
Sometimes developers code and put their code on the internet and load from there for their project when required.
These code present outsidee our project is known as external libraries


//Gennerly we load external libraries first then we load other scripts tag 
**How to put an HTML website on internet--(iss video ko ek baar dekhoooo)****

**why to use external libraries**
>let us share code
>Instead of writing our own code we can use the code writenn by other people from the internet
>It saves time and avoid duplicate work

**How to get present date**
>Get today's date
>Do calculations
>Display the date in easy-to-read format

\\Therefore we'll use external library for this purpose

**Minification->It is the process of compression of js code, here extra spaces are removed and variables name are also shorten to one letter.Compression make our code smaller which makes faster access to the code**

**Instead of using script tag to load javascript external libraries, it is better to use javascript modules to load external libraries aviod the naming conflict**

.>>Here a special version of libraries are used that is ECMA VERSION
ESM-ecmascript module  (ecmascript is just another name of javascript)

\\**Default export**
another way of exporting .we can use it when we only want to export one thing.Here curly braces are not used.


**technique of updating the data and regenerating HTML is known as MVC(Model View Controller)**
1.model saves and manages the data.
2.view=takes the data and displays it on the page.
3.controller=runs the code when we interact with the page.

In MVC,(Model View Controller) we interact with these part with the help of loop

**MVC makes sure that the page always matches with the data**

**MVC is also known as design pattern**

mvc makes sure that the HTML always matches the data
or the view always matches the model

**Testing the code**
Manual testing - we manually open the websites and try our code.manual testing is useful when we want to check if everything is working fine or not.
**Disadvantage of manual testing**
1.Hard to test every situation
2.Hard to retest

TO overcome these features we have another testing method automated testing
**Automated testing means using code to test the code**
**automates test reduces time and efforts**

//There are two types of test cases
1.Basic test case=>tests if the code is working  or not
2.Edge test case->Testing the code with the values that are little bit tricky.


<!-- Automated tests uses the code to test the code to check if the code is working correctly-->

**Testing Framework**
Testing framework is the External libraries that helps us to write our code easily.
Testing framework allows us to do all the work automatically and gives us all the features that was initially done by the automates tests

**Jasmine is a testing framework**
Here we've used jasmine as a testing framework.

>>In jasmine spec is the another name for the tests

In jasmine 5 dots represent the 5 tests and the green color shows that all the test cases are passed

And each tests also has name which represent what the test does

**Testing framework is the external library that helps to write the tests easier**

>jasmine creates a nice website for us to see the result




**Test coverage means how much of a code is being tested**
maximizing test coverage is a good practice.


**Flaky test=>It is the test that sometimes passes and sometimes fails even if we don't change the code**


**Mocks is a feature of jasmin it let us replace a method with a fake version**
Mocks is used to avoid flaky nature of tests


**spyOn () records everytime a method is used**


**mock only last for 1 test**
*that's why in every test we have to mock localstorage set item*

Unit test
testing 1 piece of the code is known as unit test

Integration test is the more complicated test than the unit test cause it  is used to test the large no of test at a one go.
**Integration test tests many units/pieces of code working together**



*Hooks a shortcut in jasmine*
Hooks:let us run some code for each test.
It allows us to share the same code between different tests.

HOOKS IN JASMINE
beforeEach()=runs code before each test
afterEach()=runs code after each test
beforeAll()=runs code before all test
afterAll()=runs code after all test
# Interview-Questions
Questions I *hear* get asked in interviews

I have not been through a development interview yet. But I hope to be soon. 

As I listen to and learn from other developers, here are some interview questions I hear that can get asked.

I am making this list so I can make sure I have studied them before any interview. 

PLEASE NOTE: These answers might be wrong. I add to them as I find information in books and websites, but I sometimes later learn that I phrased things wrong or wrote down incorrect or old information, and so I need to come back here and update/correct the "answers."

1. What is polymorphism and give some examples of when it would be used?
2. What is encapsulation and explain why it is helpful for programming?
3. What is currying and how is it helpful for programming?
4. What is hoisting?
5. What are closures, and describe a time where you would use it.
6. Describe asynchronous js vs async. 

Code usually get executed in a linear fashion from top to bottom, with functions getting added to the callstack. Async javascript allows code to keep progressing, even as it waits for previously called functions to finish. This might be necessary due to a fetch request, or a timeout function, or something else that requires a long wait time.

7. Describe what happens when a script is run. (explain global execution context, event loops, code blocking tasks queue, the stack, etc). 
8. How would you setup/define a class component in react? 
9. Explain the four pillars of OOP. 
10. What does prototype mean, and explain prototype chaining.

A prototype is simply a property on a function (or object??) that points to an object. 
When added to an object, it sends JS to look to the prototype for any properties that failed in the lookup
Helpful: https://www.freecodecamp.org/news/a-beginners-guide-to-javascripts-prototype/ 

Prototype chaining means that the code looks on the instance of the object for the property that has been called. If it fails to find it, it looks on the prototype of that object. If it is not found there, it looks on the prototype's prototype, and so on, until there are no prototypes left. If the property is never located, then it returns undefined. 

11. What goes in the head tag? 
12. How do you debug? 
13. What are promises? 
14. What are 3 ways to create an object in js?
https://dzone.com/articles/easy-javascript-part-13-four-ways-to-create-object 

a. Object Literal:
  const ObjectLiteral = {
    properties here
  }

b. With an object function in connection with Object.create()
  function ObjectTemplate (param, eters) { 
    let objectName = {};
    objectName.param = param;
    objectName.eters = eters;  
    return objectName;
  }
  
   and then use Object.create() to make :
    let newObject = Object.create(ObjectTemplate);
    
  c. with object function and New:
    let newObject = New ObjectTemplate(, params):
    New, by default, includes BOTH the constructor and return statements from the ObjectTemplate, so you don't have to write them into the ObjectTemplate
  
  d. BONUS: With a class, and then New
  
15. What does the NEW keyword do?

See part c above.

16. List 5 or more ways to optimize a website for speed. 

a. Minimimize JS and CSS and images
b. Use a CDN
c. Async JS 
d. 


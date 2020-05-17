1. advantages to Test Driven Development
1. receive fast feedback.
2. creates a detailed specification.
3. spend less time in the debugger.

2. what case would you need to use beforeEach() or afterEach() in a test suite?

## beforeEach and afterEach are run before/after every it block in the current context and all nested contexts.

3. What is one downside of Test Driven Development

- Big time investment. For the simple case you lose about 20% of the actual implementation, but for complicated cases you lose much more.

- Additional Complexity. For complex cases your test cases are harder to calculate, I'd suggest in cases like that to try and use automatic reference code that will run in parallel in the debug version / test run, instead of the unit test of simplest cases.

- Design Impacts. Sometimes the design is not clear at the start and evolves as you go along - this will force you to redo your test which will generate a big time lose. I would suggest postponing unit tests in this case until you have some grasp of the design in mind.

- Continuous Tweaking. For data structures and black box algorithms unit tests would be perfect, but for algorithms that tend to be changed, tweaked or fine tuned, this can cause a big time investment that one might claim is not justified. So use it when you think it actually fits the system and don't force the design to fit to TDD.

4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
## The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.

5. Name a use case for a static method
## Use a static method when you want to be able to access the method without an instance of the class. Use static when you want to provide class level access to a method.

6. Write an example of a Higher Order function and describe the use case it solves
- Without Higher-order function
> const arr1 = [1, 2, 3];
const arr2 = [];
for(let i = 0; i < arr1.length; i++) {
arr2.push(arr1[i] * 2);
}
// prints [ 2, 4, 6 ]
console.log(arr2);

- With Higher-order function map

> const arr1 = [1, 2, 3];
const arr2 = arr1.map(function(item) {
return item * 2;
});
console.log(arr2);

# MDN this
- this will default to the global object, which is window in a browser.
# MDN class
> Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations.
## Class declarations:
> One way to define a class is using a class declaration. To declare a class, you use the class keyword with the name of the class.
## Class expressions
> s another way to define a class. Class expressions can be named or unnamed. 
## Class body and method definitions
- Constructor
- Prototype methods
- Static methods
- Boxing with prototype and static methods
## Sub classing with extends
> The extends keyword is used in class declarations or class expressions to create a class as a child of another class.
## Super class calls with super
> The super keyword is used to call corresponding methods of super class. This is one advantage over prototype-based inheritance.
# Jest 
- Install Jest
> npm install --save-dev jest



# tscoin
Mini Typescript project miming cryptocurrency.

### What is Typescript? 🤔

A script that is superset of Javascript.

When TS is compiled, it will be come Javascript.

Supports Type stricted rules, which prevents unintended bugs that do happend in Javascript.

Statically typed language, need to implicitly set types for every variables, like Java. 
<br>(Opposite, dynamically typed lanuage, Javascript)

### Pros ✔️

Able to find potential errors before excecuting or testing the code.
<br>
For larger projects, maintaining code will become less cumbersome.

Can used to transcompile modern JS codes to old JS codes, for running JS on the old browsers.

### Cons ❌

More codes need to be written.
<br>
If not used to other type-stricted languages, it may take some time to get used to this.

Typescript does not run on the browsers. (Unless, the browser supports TS)
<br>
To run TS files, they must be compiled to JS files, and the browser or node.js can read the JS files and excecute them.


### Setting related to Typescript 🛠️

`tsconfig.json`: Configuration of transcompiling TS to JS. <a href="https://www.typescriptlang.org/tsconfig">Document</a>


### Caution about declaring types

If assigned type, for a variable, has uppercase letter at the beginning, this means that TS will look for an object. (interface or class).
<br>
For number, string, and boolean types, must be written in lowercase.

### Type Alias / Interface

A blue print of an object, and this won't be shown in compiled JS code. This is for TS only.
<br>
If you want to show the structure of the `Alias` / `interface` in the compiled JS file, using `class` may be a good option.

<pre>
  type Human = {
    race: string,
    age: number,
    name: string
  }

  let person: Human;

  ---

  interface Human {
    race: string,
    age: number,
    name: string
  }

  let person: Human;
</pre>

### Union Type

A type that allows to have more than one type.

<pre>
  let variable: string | number | boolean = ...;
</pre>

### Generics

Tells TS that the there is a type that could be anything but `any`.

<pre>
  function do &#60;T&#62; (array: T[], value: T ) {...}
</pre>


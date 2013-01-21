# YOLO Guideline

  Parsify believes in the phrase **YOLO**. You only live once, so make your code beautiful.
  
# Information

**Author** 
Nijiko Yonskai, <nijikokun@gmail.com>, [@nijikokun](http://twitter.com/nijikokun)
  
**List of Contributors**:
  
  * Nobody, why not contribute today!

**Version** 
0.0.2

# Table Of Contents

  * [Generics](#generics)
    * [Spacing](#spacing)
    * [Newlines](#newlines)
    * [Licensing](#licensing)
  * [JavaScript](#javascript)
    * [Law of Whitespace](#law-of-whitespace) 
    * [Syntax](#syntax)
      * [Parenthesis](#parenthesis)

# Generics

  This section applies to any language we write or work with, simply generic rules we **must** follow.
  It's a hard pill to swallow, being so rigid in our ideals, the reason for this is to have consistency.
  Principals. Morals. You know, those things that build character, our code has character, lets keep it 
  sane.

## Spacing

  `2` Space, no tabs. 

### Excuses and Philosophies

  Two spaces will look the same in every editor, regardless of what you use.

  **Excuse** Maximises usage of limited whitespace, not everyone has a large monitor, some of us work on laptops.

## Newlines

  **Don't** be afraid of newlines. 
  Break where needed, but logically.

  On the other side of the fence: ( _Makes sense if you view the source_ )

  **Don't** be afraid of long lines. Break where needed, and logically.

## Licensing

  **Open-source:** Apache, BSD, MIT, or AOL
  
# Javascript

  JavaScript fuels a lot of projects here at Parsify, and we like to make sure our code is 
  always readable, even third-party scripts. A lot of people follow other specifications 
  that allow them to be flexible, and this is bad in a few ways.
  
  Being flexible in your ideals opens the doors to inconsistencies, bugs, and bad 
  habits. So we developed these laws we must abide by to code beautiful, and future 
  proof code.
  
  > **Sucking at something is the first step towards being sorta good at something**
  > \- Jake the Dog
  
## Laws of Whitespace

  Starting off with whitespace, quite possibly the most important part of your code, we 
  call this section laws, as they are to be enforced.
  
  1. Never mix tabs and spaces.
  2. When starting a new project, prefer **spaces** over tabs. **Always.**
    1. Indent size is as before: `2`

## Syntax

  The syntax of your code is the first thing that people will notice when they view the source, 
  it is the coat your code wears, the fedora that accentuates the face, or the style that sets 
  your hair to be unique or the same as others. 
  
  Here we will lay down the foundation of rules that guide our code to being beautiful. They 
  like all other rules will lie on-top of the ground we have provided in the previous section.
  
### Parenthesis
 
```javascript
// Example of "Even" Style, a single space between the keyword and parenthesis.
if (variable) 
  // Example of Method Invocation where the parenthesis touch the method name.
  method();
```

  Your parenthesis should not touch `keywords` such as `if`, `if else`, `while`, `for`, and `function`; 
  They can however touch an invocation.
  
```javascript
// Another example, exemplifying how one would declare a function.
// Just like before, single space between keyword, method name, and our 
// argument declarations.
function name ([arg[, ...]]) {
  return;
}

// Maybe an expression function, or value function if you will to further show 
// exactly how parenthesis should be handled.
var name = function ([arg[, ...]]) {
  return;
}
```

#### Examples of Bad Styles

  Invocation always is allowed to touch parenthesis.

##### Cramped

  Highly in-consistent in spacing, keywords do not touch function names, yet keywords can touch parens.

```javascript
if(variable) method();

function name([arg[,...]]){
  return;
}
```

##### Spaced-out Style
  
  Slower to type, not much of a readability gain, easier to make mistakes and create inconsistencies... 
  The list goes on.
  
```javascript
if ( variable ) method();

function name ( [arg[, ...]] ) {
  return;
}
```
 
#### Excuses and Philosophies

  We do not believe in *cramped*, *spaced-out* style. Instead for *truly* beautiful code that is 
  consistent, and always easy to read, less to type we prefer a mixture of both named *even* style.
  
  **Excuses**: Easier to adapt to, harder to mess up, easier to read.

### Braces

```javascript
// Like the previous statements we continue on the Even Style
if (variable) {
    // Expanded code
    // . . .
}
```

# jetbrains-live-templates-commentsjs

Coding human-readable code by using comment split code for Jerbrains IDE ie WebStorm and Idea.  It supports JavaScript and TypeScript.

The project inspired by facebook's [f8app](https://github.com/fbsamples/f8app). Their [code](https://github.com/fbsamples/f8app/blob/master/js/login/LoginScreen.js) uses a lot of split lines to make the structure clear so that I can locate the key position when I read the code for the first time. As my project became more complex, I decided to refactor my code. Therefore I built this tool.

## Install 

Clone code into your Jetbrains IDE configuration directory.

Syntax in Windows

`%HOMEPATH%\.<product><version>\config`

Example

`C:\Users\JohnS\.IntelliJIdea2019.2\config`

## How to use it

Typing `cmtline` and `Tab` to generate a comment line.

```javascript
/** 
 ================================================================ */
```

Then you can edit it to anything you like to split your code.

Besides, I provide some commonly used code for you.

```javascript
// for react app and nodejs

cmtinterface
/** interface ================================================== */

cmtconst
/** constant =================================================== */

cmtmock
/** mock data ================================================== */

cmtfunc
/** function =================================================== */

cmtcomp
/** component ================================================== */

cmtexport
/** export ===================================================== */

cmtmain
/** main ======================================================= */

// for test

cmtsetup
/** setup ====================================================== */

cmttest
/** test ======================================================= */
```

After you edited the code, it has a clear structure and easy to read.

Like this

```javascript
import React, {useState} from "react";

/** constant =================================================== */

const user = 'Stranger';

/** component ================================================== */

/**
 * <Hello />
 * A greeting component for user
 */
const Hello = () => {
    const [word, setWord] = useState(user);
    
    return (
        <div onClick={() => setWord('my friend')}>Hello {word}</div>
    )
};

/** export ===================================================== */

export {Hello}
```

Enjoy coding!

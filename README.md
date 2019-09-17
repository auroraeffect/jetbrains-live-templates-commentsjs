# jetbrains-live-templates-commentsjs

Coding human-readable code by using comment split code

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

cmtconst
/** constant =================================================== */

cmtdata
/** mockdata =================================================== */

cmtfunc
/** function =================================================== */

cmtcomp
/** <App /> ==================================================== */

cmtexport
/** export ===================================================== */
```

After you edited the code, it has a clear structure and easy to read.

Like this

```javascript
import React, {useState} from "react";

/** constant =================================================== */

const user = 'Stranger';

/** <Hello /> ================================================== */

const Hello = () => {
    const [word, setWord] = useState(user);
    
    const handleClick = () => {
        setWord('my friend')
    };
    
    return (
        <div onClick={handleClick}>Hello {word}</div>
    )
};

/** export ===================================================== */

export {Hello}
```

Enjoy coding!

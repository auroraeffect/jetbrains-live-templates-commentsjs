# jetbrains-live-templates-commentsjs

coding human readable code by using comment split code

## Install 

Clone code into your Jetbrains IDE configuration directory.

Syntax in Windows

`%HOMEPATH%\.<product><version>\config`

Example

`C:\Users\JohnS\.IntelliJIdea2019.2\config`

## How to use it

type `cmtline` and `Tab` to generate a comment line.

```javascript
/** 
 ================================================================ */
```

then you can edit it to anything you like to split your code

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

after you edited the code, it has more defined part and easy to read.

like this

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

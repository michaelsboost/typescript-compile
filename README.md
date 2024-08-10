TypeScript Compile 
================== 

[TypeScript](http://www.typescriptlang.org) is a brand new language which compiles on JavaScript. However, this operation has to be performed manually, using the command-line compiler `tsc` or other tools. But now it has drastically improved, thanks to TypeScript Compile! TypeScript Compile automatically transforms your TypeScript code into JavaScript on the fly! Just write your TS code between: 

    <script type="text/typescript"> 
        ... 
    </script>

or include your TS file: 

    <script type="text/typescript" src="demo.ts"></script> 

and add these two JS files **at the end of the HTML body**: 

    <script type="text/javascript" src="typescript.min.js"></script> 
    <script type="text/javascript" src="typescript.compile.min.js"></script> 

That's it! TypeScript will be compiled to JavaScript and immediately run, by appending the compiled script to the HTML body. You can see any compilation errors in the web console. 

How It Works! 
---- 

TypeScript Compile works by grabbing the typescript source from within the text/typescript tags (or via fetching the file(s)) and compiling it via TypeScript and then appending a new script of the compiled Javascript. By doing it this way Typescript Compile contains only 40 lines of Javascript and is only 4KB in size.

Inspired by the original [TypeScript Compile](https://github.com/niutech/typescript-compile) by Jerzy Głowacki.

Demo 
---- 

[Here is a live demo](http://michaelsboost.github.io/typescript-compile/demo/demo.html) 

Download 
-------- 

[TypeScript 5.5](https://raw.github.com/michaelsboost/typescript-compile/gh-pages/js/typescript.min.js) (minified JS)   
[TypeScript Compile 0.3](https://raw.github.com/michaelsboost/typescript-compile/gh-pages/js/typescript.compile.min.js) (minified JS)

License
-------------

MIT

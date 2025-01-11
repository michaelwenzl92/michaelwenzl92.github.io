---
layout: post
title: WebAssembly - The new era of web development
redirect_from:
- /webassembly-the-new-era-of-web-development/
date: 2020-03-22 05:54:00
description: WebAssembly - The new era of web development
tags: web
categories: software
---

On 5 December 2019 the World Wide Web Consortium made with this [article](https://www.w3.org/2019/12/pressrelease-wasm-rec.html.en) a major step towards a faster and more flexible web. They added a fourth language for client-side web development to the existing languages HTML, CSS, and Javascript. All major browsers already supported it since 2017. This language will not only enhance the performance and improves the available application areas, but it will also make the web more agnostic on which programming language you or your development team want to develop. This is the possibility to enter a completely new era of web development and this language is called **WebAssembly**.

## What is WebAssembly?

Let us start to analyse the term assembly. Regarding [Wikipedia](https://en.wikipedia.org/wiki/Assembly_language) the term refers to the good old low-level programming language only one abstraction layer above binary machine-code. Usually one assembly code statement stands for one machine instruction. This gives an insight on how low-level and how close to the machine this language really is.

WebAssembly basically is assembly for the browser. It is binary code that runs in the same sandbox and virtual machine like Javascript, but at a much lower level of abstraction. **One can say that it is the machine code of the web.** It is important to mention that this is not real machine code. It is in reality byte code and the browser is able to execute it independently on every platform. This has some major advantages against Javascript.

Because of the lower level of abstraction, it is possible to create much more efficient code. This not only applies to memory management, but also the optimization of execution steps. The very expensive interpretation step falls away. Furthermore, due to the static type system it is much more efficient than Javascript.

Programming that way may sound a bit laborious and more complex. It is basically really more laborious and complex, but no one have ever said that it have to be programmed in it directly. (There is also only very few people out there programming in assembly) Because it is basically the machine code of the web, it is possible to code in other languages and compile this code to WebAssembly. Now we have a powerful possibility to write interactive client-side code in any other language like C or C++. The compiler has the ability to optimize effectively and give the compiled files a much smaller file size and a better execution performance. On GitHub a list on which languages are currently supported for compiling to WebAssembly is available in [repository](https://github.com/appcypher/awesome-wasm-langs).

## New application areas with WebAssembly

With optimized code the browser is now able to compute complex and high-performance tasks. This elevates browser gaming to a new sphere and also enables porting big software suites to the web. A very good example is the added WebAssembly-support for the UnrealEngine. In the following video you can see a presentation of the Unreal Engine 4 executed inside the browser. Basically a top-notch gaming engine executed without any installation. On top of that it is executed in a piece of software that is more or less installed on every computer and smartphone on our planet.

{% include youtube.html id="eh-yy7f1bvQ" title="Unreal Engine 4 Web Asm Demo. implyingprogramming.com" %}

Another example would be the porting of the 30-year old AutoCAD code base to the web. It is possible to port an old C++ code base to the web. Because of that it is possible to benefit from the web's advantages like better a completely new customer target market or better CI/CD. (continuous integration / continuous delivery) If you want to hear more about this porting project you can watch the [talk](https://www.infoq.com/presentations/autocad-webassembly/?utm_source=presentations&utm_medium=ny&utm_campaign=qcon) from one of the developers.

Other possible use cases for WebAssembly are available in the following [link](https://webassembly.org/docs/use-cases/).

## Will WebAssembly replace Javascript?

In the short term it is very unlikely that WebAssembly will replace Javascript. It will much more likely complement JavaScript in its weaker parts for special use cases like gaming or computation heavy software.

Nonetheless, in the long term it will replace Javascript and Javascript will be used more for gluing the HTML-DOM and WebAssembly together. It will create a completely new ecosystem for web development. There will be the opportunity for enterprise projects to write not only the backend, but also the frontend in Java or C#. Existing software suites written in TypeScript can be compiled to WebAssembly. A good indicator that I am not that off with my possible forecast is this [link](https://docs.assemblyscript.org/details/compiler) to a project for a TypeScript compiler to WebAssembly.

## Conclusion

There will be a lot of new possibilities with this new language. From gaming to computation heavy applications to porting desktop software to the web. All the discussed approaches are still a bit in its infancy, but it is already well-received and supported by a lot of projects out there.

For me personally it was always a bit frustrating that Javascript was more or less the machine language of the web. Lots of web frameworks are transpiling to Javascript and even if optimization frameworks like asm.js were a step to a more performant web, WebAssembly is a much cleaner and better solution. I am really excited since the first time I heard of WebAssembly and I cannot wait until trying it out  for the first time on a real world project.


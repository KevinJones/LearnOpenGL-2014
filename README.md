Advice for Learning OpenGL in 2014
==================================

A friend of mine recently asked about how to learn OpenGL. Like most software, OpenGL has changed a lot in a short amount of time, so there's a lot of confusing or outdated information available. The finer details of computer graphics programming intimidate a lot of people, so I've created this short collection of advice and links intended as a jumping-off point for learning modern OpenGL.

Based on my limited knowledge and extensive web searching of the topic, here's what I recommended:

1) Prepare to be confused. The usual note-taking and study advice applies.

2) Work in C or C++, because most of the material on the subject is in these languages. There do exist OpenGL bindings for like Java, but they're harder to work with when you're just learning.

3) Learn "modern" OpenGL. This is OpenGL 2.1+ or OpenGL ES 2.0+, using shaders and a programmable pipeline. Avoid tutorials that aren't based on shaders. Fixed-function OpenGL might seem more intuitive, but it's less flexible and is considered deprecated. Basically, if you see calls to ```glBegin``` and ```glEnd```, you should look elsewhere.

4) You might have better luck setting up your development environment on Linux, thanks to the package managers most distros have. I'm sure it's possible in other OSes, but my Windows-fu is weak.

5) There's a comparison of popular learning resources for new OpenGL programmers in this StackExchange post: http://gamedev.stackexchange.com/a/22405 . To summarize:

- Jason McKesson is quite fond of Jason McKesson's "Learning Modern 3D Graphics Programming." It focuses on explaining details of the OpenGL pipeline so you can learn how it actually works. Still a work in progress; only covers up to lighting and texturing. http://www.arcsynthesis.org/gltut/

- The "OpenGL Superbible" comes with a library that hides some of the more finicky details of OpenGL to make the material aesier to digest. You'll want to make sure you examine the library and figure out what's actually going on before you're done with the book, though. http://www.amazon.com/OpenGL-SuperBible-Comprehensive-Tutorial-Reference/dp/0321902947

- The OpenGL Programming Wikibook has a lot of tutorials, with an emphasis on source code. This works best if you also have a reference handy when you want to learn more about what's actually going on. http://en.wikibooks.org/wiki/OpenGL_Programming

- "OpenGL Programming Guide (8th Edition)", also known as "Redbook", is reportedly thorough but somewhat confusingly organized. It might make a good reference to pair up with the Wikibook. The 8th edition excludes the outdated information McKesson mentions in the StackExchange post, but is missing some of the sample code. (The book's website states that "most" of the code is available for the 8th edition, which was released almost a year ago, so it's probably going to stay incomplete.) http://www.amazon.com/OpenGL-Programming-Guide-Official-Learning/dp/0321773039

6) After this, depending on your learning style, you should either just mess around and make cool stuff, or play around with example code you find online. Personally, I learned a lot about alpha blending modes while making special effects for Cocos2d games. The source code of simple game engines like LÖVE or Cocos2d can teach you a lot about how you'd integrate OpenGL into a full-featured piece of software.

I hope this helps!

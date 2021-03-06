Forked from Google Style Guides
===============================

Diff from google:  
1) It uses brace style like:  
```
void func()
{
   ...
}
```
2) An else clause should NOT be on the same line as the preceding closing brace:
```
if (cond1)
{
    ...
}
else if (cond2)
{
    ...
}
else
{
    ...
}
```
3) Allow use ```#pragma once``` insted of ```#ifndef``` macro.

4) Public/private must have same indent as class/struct:
```
class A
{
public:
    A();
private:
    int m_;
};
```
  
5) local variables should be named in snake_case:
```
    int abc_def;  // good
    int abcDef;   // bad
```
  
6) free functions should be named in snake_case:
```
    int test_test();  // good
    int testTest();   // bad
```

7) struct member should be named in snake_case:
```
struct my_struct_t
{
    int test_test;  // good
    int testTest;   // bad
}
```

8) class member should be named in m_CamelCase,  
class method should be named in mixedCase:
```
class MyClas
{
public:
    int test_test();  // bad
    int testTest();   // good
private:
    int m_TestTest;   // good
    int test_test;    // bad
    int test;         // bad
}
```

9) should not indent code inside a namespace:
```
namespace my_space
{
int testTest();       // good
    int test_test();  // bad

class Test            // good
{
};

    class Test2       // bad
    {

    };

}  // namespace my_space
```

10) function argument name should be named in snake_case style:
```
void f(int my_test)     // good
void f(int myTest)      // bad
void f(int MyTest)      // bad
```

11) filenames should be named in snake_case:
```
my_test.hpp     // good
my_test.cpp     // good
MyTest.hpp      // bad
MyTest.cpp      // bad
```


---

cpplint.py and its corresponding unit tests are Copyright (C) 2009 Google Inc.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are
met:

   * Redistributions of source code must retain the above copyright
notice, this list of conditions and the following disclaimer.
   * Redistributions in binary form must reproduce the above
copyright notice, this list of conditions and the following disclaimer
in the documentation and/or other materials provided with the
distribution.
   * Neither the name of Google Inc. nor the names of its
contributors may be used to endorse or promote products derived from
this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

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

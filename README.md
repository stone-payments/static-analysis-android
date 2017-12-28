# Summary
1. [Introduction](#introduction)
   * [Overview](#overview)   
   * [How to use](#how-to-use)  
4. [License](#license)


<a name="introduction" />

# Introduction

<a name="overview" />

## Overview
 Static Code Analysis Tools for Kotlin and Java in Android

<a name="how-to-use" />

## How to use
1. Add following lines to your build.gradle file.
2. Run `gradle check`
3. Add `check.dependsOn 'checkstyle', 'findbugs', 'pmd', 'ktlint', 'detekt'` if you want to run all tools on every `build`

 ```groovy
  apply from: '../static-analysis/findbugs.gradle'
  apply from: '../static-analysis/pmd.gradle'
  apply from: '../static-analysis/checkstyle.gradle'
  apply from: '../static-analysis/lint.gradle'
  apply from: '../static-analysis/ktlint.gradle'
  apply from: '../static-analysis/detekt.gradle'

  //Optional line
  check.dependsOn 'checkstyle', 'findbugs', 'pmd', 'ktlint', 'detekt'
```



## Example Android application with tools

<p align="center">
  <img src="example/example_1.png" align="center" width=400>
<br /><br />

</p>


<a name="license" />

## License
```
MIT License

Copyright (c) 2017 Stone Pagamentos

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```

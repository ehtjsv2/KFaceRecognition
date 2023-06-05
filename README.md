# KFaceRecognition


:zap: A powerful & easy to use Face Recognition library for Android  :zap:


## Table of Contents
1. [Getting Started](#getting-started)
1. [Documentation](#documentation)
1. [Examples](#examples)
1. [Tutorial](#tutorial)
2. [Question](#question)
3. [Creators](#creators)


<h2 id="getting-started">Getting Started</h2>
1. clone this project</br>
2. open your android project and File->new->import module</br>
3. select our cloned module(facerecognitionlibrary and sdk)</br>
4. add below script to your bulid.gradke(project)</br>

```id com.chaquo.python' version '14.0.2' apply false ```</br>
5. add below script to your bulid.gradle(module:app)</br>

```
dependencies {
 ...
def camerax_version = "1.0.0-rc03"


    // The following line is optional, as the core library is included indirectly by camera-camera2
    implementation "androidx.camera:camera-core:${camerax_version}"
    implementation "androidx.camera:camera-camera2:${camerax_version}"
    // If you want to additionally use the CameraX Lifecycle library
    implementation "androidx.camera:camera-lifecycle:${camerax_version}"
    // If you want to additionally use the CameraX View class
    implementation "androidx.camera:camera-view:1.0.0-alpha22"
    // If you want to additionally use the CameraX Extensions library
    implementation "androidx.camera:camera-extensions:1.0.0-alpha22"
...    
    }
```

<br/>

<h2 id="documentation">Documentation :notebook_with_decorative_cover:</h2>

<!-- See the [**documentation**](https://weeklycoding.com/mpandroidchart/) for examples and general use of MPAndroidChart. -->

See the [**Kdocs**]() for more advanced documentation.

<br/>

<h2 id="examples">Examples :eyes:</h2>
[![ScreenShot]()](https://www.youtube.com/watch?v=ufaK_Hd6BpI)

<br/>

<h2 id="tutorial">Tutorial :movie_camera:</h2>

<br/>

**Setting tutorial Video**
<br/><br/>
[setting](http://youtube.com)
<br/><br/>

**Tutorial Videos**
<br/><br/>
[how to apply basic features](http://youtube.com)
<br/><br/>
[how to adjust count threshold](http://youtube.com)
<br/><br/>
[how to adjust similarity threshold](http://youtube.com) 
Default is 0.4
<br/><br/>

<br/>

<h2 id="question">Question ❓:</h2>

<br/>

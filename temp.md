---
title: View-based Adaptive Streaming
layout: post
excerpt_separator: <!--more-->
---
**Gaurav Verma**  
**3rd Year Undergraduate Student**  
**Department of Electrical Engineering**  
**Indian Institute of Technology Kanpur**  
**Email: [gverma@iitk.ac.in](mailto:gverma@iitk.ac.in) Homepage: [Click here](http://home.iitk.ac.in/~gverma)**  

<!--more-->
<hr>

# Cube-map Rendering and View-based Adaptive Streaming of 360-degree Videos:

### Mentors:

* Professor [Yao Wang](http://engineering.nyu.edu/people/yao-wang), Department of Electrical and Computer Engineering, New York University
* Professor [Gaurav Sharma](http://www.grvsharma.com/research.html), Department of Computer Science and Engineering, IIT Kanpur

### Project Description

##### Introduction:

The convention is to use the equirectangular (ER) representation
of a 360-degree video for rendering and streaming purposes. The drawback of an equirectangular
representation is the redundancy of information at either end of the layout. The project aims
at developing rendering and adaptive streaming techniques of 360-degree videos by using cube-map
representation instead of ER representation (and hence reducing the redundant information by
a significant amount).

##### Cube-map Rendering:

Facebookâ€™s open-sourced transformation code was used to remap an equirectangular
360-degree video to cube-map. This transformation was accomplished using FFmpeg. Three.js (JavaScript
3D library) and OpenGL were used to implement browser based rendering of 360-degree videos with
cube-map layout. Noteworthy texture mapping algorithms, involving UV mapping, were developed
to map the cube-map texture on a cube geometry, which was morphed into a sphere using vertex
nomalization techniques in Three.js. A more accurate and  computationally rigorous implementation
of rendering is being done using OpenGL, which will be later implemented using Three.js too.

##### MPEG-DASH Content Generation:

The raw video files were re-encoded into H.264/AVC using x264
and the video partitions and MPD (Media Presentation Description) was generated using MP4Box.

##### View-based Adaptive Streaming:
The cube-map representation of the 360-degree video was partitioned
into segments and the segments were delivered to the client using the international standard
for adaptive bitrate streaming, MPEG-DASH (Dynamic Streaming over HTTP). To implement view-based
adaptive streaming of 360-degree videos, the horizontal plane was quantized into 12 bins (each
bin corresponding to 30 degrees) and the vertical plane was quantized into 6 bins (each bin corresponding to 30
degrees), hence giving a total of 72 view-ports. The view-port being demanded by the client
is dynamically monitored and the corresponding views are streamed using MPEG-DASH. View-based
adaptive streaming of 360-degree videos exploits the fact that the viewer watches only a given
portion of the video at a given point of time, and thus only one portion of the video is to
be streamed, instead of the entire video. This is a more efficient streaming method for 360-degree
videos and consumes lesser bandwidth compared to the conventional streaming methods.

##### Project Report:

[Click here](http://home.iitk.ac.in/~gverma/RTEReport.pdf)

##### Project Presentation:

[Click here](http://home.iitk.ac.in/~gverma/RTEPresentation.pdf)

##### Software/Libraries used:

Facebookâ€™s Transform, FFmpeg, Three.js, OpenGL, MATLAB,  DASHEncoder, MP4Box, x264

##### Languages Used:

C, JavaScript, Python

##### Version Control System:

Git

### Skills:

* 360-degree video Rendering
* 360-degree video Streaming

# Front-end Development for IIT Kanpur's New York Office:

### Mentor:

Professor [Manindra Agrawal](http://cse.iitk.ac.in/users/manindra/), Department
of Computer Science and Engineering, IIT Kanpur

### Description of Tasks:

* Developed Expand and Collapse mechanism for display of items in a stream in a web application
developed using Angular 2 framework. The task involved using Angular 2 and TypeScript to execute
a synchronous callback each time the icon is clicked, which ultimately toggled associated style
properties. Since in the collapsed state, the DOM still has all the content in browser , the
browser has to render the invisible content too.To make this efficient, ellipsis are inserted
after certain number of words, truncating rest of content.
The version control system used was Git.
The code review system used was Phabricator.
* Worked in a team to develop the front-end of NYC Office's website.

### Skills:

* Front-end development using HTML, CSS, JavaScript
* Angular 2 (Beginner), TypeScript(Beginner)

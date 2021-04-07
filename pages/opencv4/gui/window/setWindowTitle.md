---
title: 윈도우 이름 설정
sidebar: opencv4_sidebar
permalink: setWindowTitle
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">setWindowTitle</h2>
    </div>
    <div class="col-lg-12">

        <ul id="myTab" class="nav nav-tabs nav-justified">
            <li class="active"><a href="#service-one" data-toggle="tab"><i class="fa fa-support"></i> C++</a>
            </li>
            <li class=""><a href="#service-two" data-toggle="tab"><i class="fa fa-support"></i> C#</a>
            </li>
            <li class=""><a href="#service-three" data-toggle="tab"><i class="fa fa-support"></i> Python</a>
            </li>
        </ul>

        <div id="myTabContent" class="tab-content">
            <div class="tab-pane fade active in" id="service-one">
<pre class="prettyprint"><code class="language-cpp">void cv::setWindowTitle(
    const String& winname,
    const String& title
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.SetWindowTitle(
    string winName,
    string title
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.setWindowTitle(
    winname,
    title
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 윈도우의 이름을 변경합니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 이름을 변경하려는 윈도우 이름

> `제목(title)` 변경하려는 윈도우의 새로운 이름

### 반환값(Returns)

> `없음`
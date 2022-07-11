---
title: 히스토그램 비교
sidebar: opencv4_sidebar
permalink: compareHist
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">compareHist</h2>
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
<pre class="prettyprint"><code class="language-cpp">double cv::compareHist(
    Mat H1,
    Mat H2,
    int method
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">double Cv2.CompareHist(
    Mat h1,
    Mat h2,
    HistCompMethods method
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.compareHist(
    H1,
    H2,
    method
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 두 히스토그램을 비교합니다.

### 매개변수(Parameter)

> `히스토그램1(H1)` 비교하려는 히스토그램1

> `히스토그램2(H2)` 비교하려는 히스토그램2

> [`비교 방식(method)`](HistCompMethods) 히스토그램 비교 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">히스토그램(hist)</a> 입력 이미지로부터 계산된 히스토그램

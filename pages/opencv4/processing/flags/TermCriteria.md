---
title: 종료 기준
sidebar: opencv4_sidebar
permalink: TermCriteria
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">TermCriteria</h2>
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
<pre class="prettyprint"><code class="language-cpp">cv::TermCriteria::TermCriteria(
    int type,
    int maxCount,
    double epsilon 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">TermCriteria TermCriteria(
    CriteriaTypes type,
    int maxCount,
    double epsilon
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">termcrit = (
    type,
    maxCount,
    epsilon
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<font color="#c7254e">유형(type)</font>에 <b>+</b> 또는 <b>|</b>을 활용하여 종료 기준을 OR 형태로 구성할 수 있습니다.
{{site.data.alerts.end}}

### 요약(Summary)

> 반복 알고리즘에 대한 종료 기준을 정의합니다.

### 매개변수(Parameter)

> [`유형(type)`](CriteriaTypes) 종료 기준의 유형

> `최대 반복 횟수(maxCount)` 반복 알고리즘의 최대 실행 횟수 

> `정확도(epsilon)` 반복 알고리즘의 정확도 허용치

### 반환값(Returns)

> `종료 기준(termcrit)` 반복 알고리즘의 종료 기준
---
title: 피라미드 평균 이동 분할
sidebar: opencv4_sidebar
permalink: pyrMeanShiftFiltering
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">pyrMeanShiftFiltering</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::pyrMeanShiftFiltering(
    Mat src,
    Mat dst,
    double sp,
    double sr,
    int maxLevel = 1,
    TermCriteria termcrit = TermCriteria(TermCriteria::MAX_ITER+TermCriteria::EPS, 5, 1)
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.PyrMeanShiftFiltering(
    Mat src,
    Mat dst,
    double sp,
    double sr,
    int maxLevel = 1,
    TermCriteria? termcrit = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.pyrMeanShiftFiltering(
    src,
    sp,
    sr,
    maxLevel = None,
    termcrit = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<font color="#c7254e">최대 레벨(maxLevel)</font>을 지정해 이미지 피라미드를 만들고 이 정보를 이용하여 이미지 분할을 실행합니다.
{{site.data.alerts.end}}

{{site.data.alerts.important}}
<font color="#c7254e">출력 이미지(dst)</font>는 <b>포스터 화(posterized)</b>된 이미지를 반환합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>피라미드 평균 이동 분할 계산식(Pyramid MeanShiftFiltering Formula):</b>
$$ (X,\ Y) \Rightarrow (R,\ G,\ B) $$
$$ (x,\ y) \Rightarrow (r,\ g,\ b) $$
$$ x : X - \text{sp} \le x \le X + \text{sp} $$
$$ y : Y - \text{sp} \le y \le Y + \text{sp} $$
$$ ||(R,\ G,\ B)-(r,\ g,\ b)|| \le \text{sr} $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 이미지 피라미드에 의한 평균 이동 분할을 진행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 피라미드 평균 이동 분할을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 피라미드 평균 이동 분할이 적용된 이미지

> `공간 윈도우 반경(sp)` 각각의 픽셀(X, Y)에서 계산될 픽셀(x, y)의 범위

> `색상 윈도우 반경(sr)` 픽셀의 성분 벡터(R, G, B)에서 공간 윈도우 반경의 픽셀 성분 벡터(r, g, b)를 뺏을 때의 허용치

> `최대 레벨(maxLevel)` 피라미드 최대 레벨

> [`종료 기준(termcrit)`](TermCriteria) 반복 알고리즘의 종료 기준

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 피라미드 평균 이동 분할이 적용된 이미지
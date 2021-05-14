---
title: 적분
sidebar: opencv4_sidebar
permalink: integral
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">integral</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::integral(
    Mat src,
    Mat sum,
    Mat sqsum,
    Mat tilted,
    int sdepth = -1,
    int sqdepth = -1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Integral(
    Mat src,
    Mat sum,
    Mat sqsum,
    Mat tilted,
    int sdepth = -1,
    int sqdepth = -1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">sum, sqsum, tilted = cv2.integral3(
    src,
    sdepth = None,
    sqdepth = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
Python OpenCV는 함수가 오버로드되지 않으므로 <font color="#c7254e">cv2.integral</font>, <font color="#c7254e">cv2.integral2</font>, <font color="#c7254e">cv2.integral3</font>로 나눠 사용할 수 있습니다.
{{site.data.alerts.end}}

{% include callout.html content="

`적분 이미지(sum)`
<br><br>
$$ sum(X, Y) = \sum_{x<X, \ y<Y}^{} image(x, y) $$
<br><br>
`제곱 적분 이미지(sqsum)`
<br><br>
$$ sqsum(X, Y) = \sum_{x<X, \ y<Y}^{} image(x, y)^2 $$
<br><br>
`기울어진 적분 이미지(tilted)`
<br><br>
$$ tilted(X, Y) = \sum_{y<Y, \ abs(x-X+1) \leq Y-y-1}^{} image(x, y) $$

" type="info" %}

{% include callout.html content="

- `제곱 적분 이미지 출력 깊이(sdepth)`는 `CV_32S` 형식, `CV_32F` 형식, `CV_64F` 형식을 할당할 수 있습니다.
  
- `기울어진 적분 이미지 출력 깊이(sqdepth)`는 `CV_32F` 형식, `CV_64F` 형식을 할당할 수 있습니다.
  
" type="success" %}

<br>

### 요약(Summary)

> 이미지를 전경과 배경으로 분할하는 최적의 컷을 찾습니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 그랩 컷을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">적분 이미지(sum)</a> 적분 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">제곱 적분 이미지(sqsum)</a> 제곱된 적분 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">기울어진 적분 이미지(tilted)</a> 45° 기울어진 적분 이미지

> `제곱 적분 이미지 출력 깊이(sdepth)` 제곱 적분 이미지의 출력 깊이 설정

> `기울어진 적분 이미지 출력 깊이(sqdepth)` 기울어진 적분 이미지의 출력 깊이 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">적분 이미지(sum)</a> 적분 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">제곱 적분 이미지(sqsum)</a> 제곱된 적분 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">기울어진 적분 이미지(tilted)</a> 45° 기울어진 적분 이미지

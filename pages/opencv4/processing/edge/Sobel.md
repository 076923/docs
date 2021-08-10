---
title: 소벨
sidebar: opencv4_sidebar
permalink: Sobel
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">Sobel</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::Sobel(
    Mat src,
    Mat dst,
    int ddepth,
    int dx,
    int dy,
    int ksize = 3,
    double scale = 1,
    double delta = 0,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Sobel(
    Mat src,
    Mat dst,
    MatType ddepth,
    int xorder,
    int yorder,
    int ksize = 3,
    double scale = 1,
    double delta = 0,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.Sobel(
    src,
    ddepth,
    dx,
    dy,
    ksize = None,
    scale = None,
    delta = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<b>미분(Derivative)</b>을 활용해 인접한 픽셀들의 차이로 <b>기울기(Gradient)</b>의 크기를 계산합니다.
{{site.data.alerts.end}}

{{site.data.alerts.important}}
<font color="#c7254e">X 방향 차수(dx, xorder)</font>와 <font color="#c7254e">Y 방향 차수(dy, yorder)</font>의 합은 <b>1</b> 이상이여야 합니다.
{{site.data.alerts.end}}

{{site.data.alerts.important}}
소벨 커널은 최소 <b>3</b>의 크기부터 최대 <b>31</b>의 크기까지의 <b>홀수</b>만 가능합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>소벨 계산식(Sobel Formula):</b>
$$ \text{dst} = \frac{\partial^{xorder+yorder} \text{src}}{\partial x^{xorder} \partial y^{yorder}} $$
<b>방향에 따른 필터 형태(Filter type according to direction):</b>
$$ \begin{matrix}
\begin{bmatrix}
-1 & 0 & 1 \\ 
-2 & 0 & 1 \\ 
-1 & 0 & 1
\end{bmatrix} & \begin{bmatrix}
1 & 2 & 1 \\ 
0 & 0 & 0 \\ 
-1 & -2 & -1
\end{bmatrix} \\ 
\ 3 \times 3 \ \text{Vertical Mask} & 3 \times 3 \  \text{HorizontalMask} \\
\begin{bmatrix}
-1 & -1 & 0 & 1 & 1 \\ 
-1 & -1 & 0 & 1 & 1 \\ 
-2 & -2 & 0 & 2 & 2 \\
-1 & -1 & 0 & 1 & 1 \\ 
-1 & -1 & 0 & 1 & 1 
\end{bmatrix} & \begin{bmatrix}
1 & 1 & 2 & 1 & 1 \\ 
1 & 1 & 2 & 1 & 1 \\ 
0 & 0 & 0 & 0 & 0 \\ 
-1 & -1 & -2 & -1 & -1 \\ 
-1 & -1 & -2 & -1 & -1
\end{bmatrix} \\ 
\ 5 \times 5 \ \text{Vertical Mask} & 5 \times 5 \  \text{HorizontalMask}
\end{matrix} $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지의 X축과 Y축에 따라 미분한 값을 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 소벨을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 소벨이 적용된 이미지

> `출력 이미지 정밀도(ddepth)` 출력 이미지의 정밀도 설정

> `X 방향 차수(dx, xorder)` X축 미분 차수

> `Y 방향 차수(dy, yorder)` Y축 미분 차수

> `커널 크기(ksize)` 커널의 크기

> `비율(scale)` 필터링 된 픽셀에 곱해지는 값

> `오프셋(delta)` 필터링 된 픽셀에 더해지는 값

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 소벨이 적용된 이미지
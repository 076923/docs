---
title: 표준 허프 선 검출
sidebar: opencv4_sidebar
permalink: HoughLinesPointSet
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">HoughLinesPointSet</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::HoughLinesPointSet(
    Mat _point,
    Mat _lines,
    int lines_max,
    int threshold,
    double min_rho,
    double max_rho,
    double rho_step,
    double min_theta,
    double max_theta,
    double theta_step 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.HoughLinesPointSet(
    Mat point,
    Mat lines,
    int linesMax,
    int threshold,
    double minRho,
    double maxRho,
    double rhoStep,
    double minTheta,
    double maxTheta,
    double thetaStep
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">_lines = cv2.HoughLinesPointSet(
    _point,
    lines_max,
    threshold,
    min_rho,
    max_rho,
    rho_step,
    min_theta,
    max_theta,
    theta_step,
    _lines = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
표준 허프 변환을 적용해 점 집합에서 선을 검출합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">점(_point)</font>은 <font color="#c7254e">CV_32FC2</font> 형식의 <b>[N, 1, 2]</b> 차원을 사용합니다.
<font color="#c7254e">신뢰도(votes)</font>가 높을수록 더 정확한 검출 결과를 의미합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">최소 거리(min_rho)</font>는 <b>0.0</b>, <font color="#c7254e">최대 거리(max_rho)</font>는 <font color="#c7254e">점(_point)</font>의 <b>최댓값</b> 또는 <b>이미지 차원의 최댓값</b> 등을 권장합니다.<br>
<font color="#c7254e">최소 각도(min_theta)</font>는 <b>0.0</b>, <font color="#c7254e">최대 각도(max_theta)</font>는 <b>π / 2</b>를 권장합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력된 점 벡터에 허프 선 변환을 적용해 선을 검출합니다.

### 매개변수(Parameter)

> `점(_point)` 허프 선 변환을 적용하려는 입력 점 벡터

> `선(_lines)` 검출된 선의 신뢰도(votes), 거리(rho), 각도(theta)

> `최대 선 개수(lines_max)` 검출될 선의 최대 개수

> `임곗값(threshold)` 누산기(Accumulator) 임곗값

> `최소 거리(min_rho)` 누산 평면에서 사용되는 거리에 대한 픽셀 단위 최소 분해능

> `최대 거리(max_rho)` 누산 평면에서 사용되는 거리에 대한 픽셀 단위 최대 분해능

> `거리 간격(rho_step)` 누산 평면에서 사용되는 거리에 대한 픽셀 단위 분해능 간격

> `최소 각도(min_theta)` 누산 평면에서 사용되는 각도에 대한 픽셀 단위 최소 라디안

> `최대 각도(max_theta)` 누산 평면에서 사용되는 각도에 대한 픽셀 단위 최대 라디안

> `각도 간격(theta_step)` 누산 평면에서 사용되는 각도에 대한 픽셀 단위 라디안 간격

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">선(_lines)</a> 검출된 선의 신뢰도(votes), 거리(rho), 각도(theta)
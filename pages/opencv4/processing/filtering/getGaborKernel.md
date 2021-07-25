---
title: 가버 커널 반환
sidebar: opencv4_sidebar
permalink: getGaborKernel
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getGaborKernel</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat cv::getGaborKernel(
    Size ksize,
    double sigma,
    double theta,
    double lambd,
    double gamma,
    double psi = CV_PI *0.5,
    int ktype = CV_64F 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.GetGaborKernel(
    Size ksize,
    double sigma,
    double theta,
    double lambd,
    double gamma,
    double psi,
    int ktype
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getGaborKernel(
    ksize,
    sigma,
    theta,
    lambd,
    gamma,
    psi = None,
    ktype = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- `필터 출력 정밀도(ktype)`는 `CV_32F` 형식, `CV_64F` 형식만 가능합니다.

" type="warning" %}

<blockquote class="formula">
<b>가버 필터 계산식(Gabor Filter Formula):</b>
$$ g(x, y; \sigma, \theta, \lambda, \gamma, \psi) = \exp(-\frac{x'^{2} + \gamma^2 y'^{2}}{2\sigma^2})cos(2\pi\frac{x'}{\lambda}+\psi) $$
$$ x' = xcos{\theta}+ysin{\theta} $$
$$ y' = -xsin{\theta}+ycos{\theta} $$
</blockquote>

<br>

### 요약(Summary)

> 이미지에서 가버 필터를 계산하기 위한 필터 계수를 반환합니다.

### 매개변수(Parameter)

> `크기(ksize)` 가버 필터 커널 크기

> `시그마(sigma)` 가우스 포락선(envelope)의 표준 편차

> `각도(theta)` 가버 필터 커널의 방향

> `람다(lambd)` 가버 필터 커널의 사인파(sine wave) 파장

> `감마(gamma)` 가버 필터의 종횡비

> `프사이(psi)` 가버 필터 오프셋

> `필터 출력 정밀도(ktype)` 필터 계수의 출력 정밀도 설정

### 반환값(Returns)

> `가버 필터 계수(retval)` 가버 필터 계수의 출력 행렬

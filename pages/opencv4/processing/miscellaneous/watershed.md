---
title: 워터쉐드
sidebar: opencv4_sidebar
permalink: watershed
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">watershed</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::watershed(
    Mat image,
    Mat markers
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Watershed(
    Mat image,
    Mat markers
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">markers = cv2.watershed(
    image,
    markers
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<font color="#c7254e">마커(markers)</font>의 라벨링 값 중 <font color="#c7254e">0</font>은 <b>불명확한 정보를 의미합니다.</b>
{{site.data.alerts.end}}

{{site.data.alerts.note}}
워터쉐드 이후의 <font color="#c7254e">마커(markers)</font>의 값 중 <font color="#c7254e">-1</font>은 <b>경계선을 의미합니다.</b>
{{site.data.alerts.end}}

{% include callout.html content="

- `입력 이미지(image)`는 `CV_8UC3` 형식만 할당할 수 있습니다.
  
- `마커(markers)`는 `CV_32SC1` 형식만 할당할 수 있으며 입력 이미지와 이미지 크기가 동일해야 합니다.
  
" type="warning" %}

<br>

### 요약(Summary)

> 배경과 전경이 분리된 마커를 활용해 이미지를 분할합니다.

### 매개변수(Parameter)

> `입력 이미지(image)` 워터쉐드를 적용하려는 입력 이미지

> `마커(markers)` 라벨링 정보가 담겨있는 마커 배열

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">마커(markers)</a> 워터쉐드 정보가 담겨있는 마커 배열

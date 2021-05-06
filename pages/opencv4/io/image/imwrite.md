---
title: 이미지 쓰기
sidebar: opencv4_sidebar
permalink: imwrite
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">imwrite</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::imwrite(
    const String& filename,
    Mat img,
    const std::vector&lt;int&gt;& params = std::vector&lt;int&gt;() 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool Cv2.ImWrite(
    string fileName,
    Mat img,
    params ImageEncodingParam[] prms
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.imwrite(
    filename,
    flags,
    params = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}
일반적으로 <b>8 비트 단일 채널</b> 또는 <b>3 채널</b> 이미지만 저장할 수 있지만, 일부 형식은 <b>특정 파일 형식</b>으로 저장할 수 있습니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `CV_16U` 형식 이미지는 `PNG`, `JPEG2000`, `TIFF`로 저장할 수 있습니다.
  
- `CV_32F` 형식 이미지는 `PFM`, `TIFF`, `OpenEXR`, `Radiance HDR`로 저장할 수 있습니다.
  
- `4 채널` 이미지는 `Alpha` 채널의 값을 변경하여 `PNG`로 저장할 수 있습니다.
  
- `다중` 이미지는 `TIFF`로 저장할 수 있습니다.

" type="success" %} 

<br>

### 요약(Summary)

> [이미지](imageExt)를 파일로 저장합니다.

### 매개변수(Parameter)

> `파일 이름(filename)` 이미지 파일의 경로

> `이미지(img)` 저장하려는 이미지

> [`이미지 부호화 매개변수(params)`](imageEncodingParam) 부호화 매개변수

### 반환값(Returns)

> `결괏값(retval)` 파일로 저장할 수 있는 경우, 참(True) 값을 반환
---
title: 비디오 쓰기 - 속성 플래그
sidebar: opencv4_sidebar
permalink: VideoWriterProperties
folder: opencv4
---

<ul id="profileTabs" class="nav nav-tabs">
    <li class="active"><a class="noCrossRef" href="#L1" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">C++</a></li>
    <li><a class="noCrossRef" href="#L2" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">C#</a></li>
    <li><a class="noCrossRef" href="#L3" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">Python</a></li>
</ul>

<div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="L1" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `VIDEOWRITER_PROP_QUALITY` | 인코딩된 비디오 스트림의 현재 품질(0 ~ 100) |
| `VIDEOWRITER_PROP_FRAMEBYTES` | 인코딩된 비디오 프레임의 크기 |
| `VIDEOWRITER_PROP_NSTRIPES` | 병렬 인코딩을 위한 스트라이프 수 |
| `VIDEOWRITER_PROP_IS_COLOR` | 다중 채널 프레임으로 인코딩 유/무 |
| `VIDEOWRITER_PROP_DEPTH` | 인코딩된 비디오 프레임의 정밀도 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `VideoWriterProperties.Quality` | 인코딩된 비디오 스트림의 현재 품질(0 ~ 100) |
| `VideoWriterProperties.FrameBytes` | 인코딩된 비디오 프레임의 크기 |
| `VideoWriterProperties.NStripes` | 병렬 인코딩을 위한 스트라이프 수 |
| `VideoWriterProperties.Iscolor` | <a data-toggle="tooltip" data-original-title="{{site.data.glossary.Not_supported}}">다중 채널 프레임으로 인코딩 유/무</a> |
| `VideoWriterProperties.Depth` | <a data-toggle="tooltip" data-original-title="{{site.data.glossary.Not_supported}}">인코딩된 비디오 프레임의 정밀도</a> |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.VIDEOWRITER_PROP_QUALITY` | 인코딩된 비디오 스트림의 현재 품질(0 ~ 100) |
| `cv2.VIDEOWRITER_PROP_FRAMEBYTES` | 인코딩된 비디오 프레임의 크기 |
| `cv2.VIDEOWRITER_PROP_NSTRIPES` | 병렬 인코딩을 위한 스트라이프 수 |
| `cv2.VIDEOWRITER_PROP_IS_COLOR` | 다중 채널 프레임으로 인코딩 유/무 |
| `cv2.VIDEOWRITER_PROP_DEPTH` | 인코딩된 비디오 프레임의 정밀도 |

</div>
</div>

<br>

### 요약(Summary)

> 비디오 쓰기 속성을 설정하거나 불러옵니다.
---
title: PAM 형식 플래그
sidebar: opencv4_sidebar
permalink: imwritePAMFlags
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
| `IMWRITE_PAM_FORMAT_NULL` | 포맷 설정을 하지 않음 |
| `IMWRITE_PAM_FORMAT_BLACKANDWHITE` | 이진화 |
| `IMWRITE_PAM_FORMAT_GRAYSCALE` | 그레이스케일 |
| `IMWRITE_PAM_FORMAT_GRAYSCALE_ALPHA` | 그레이스케일 알파채널 |
| `IMWRITE_PAM_FORMAT_RGB` | 색상 이미지 |
| `IMWRITE_PAM_FORMAT_RGB_ALPHA` | 색상이미지 알파채널 |


</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `ImwritePAMFlags.FormatNull` | 포맷 설정을 하지 않음 |
| `ImwritePAMFlags.FormatBlackAndWhite` | 이진화 |
| `ImwritePAMFlags.FormatGrayscale` | 그레이스케일 |
| `ImwritePAMFlags.FormatGrayscaleAlpha` | 그레이스케일 알파채널 |
| `ImwritePAMFlags.FormatRgb` | 색상 이미지 |
| `ImwritePAMFlags.FormatRgbAlpha` | 색상이미지 알파채널 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.IMWRITE_PAM_FORMAT_NULL` | 포맷 설정을 하지 않음 |
| `cv2.IMWRITE_PAM_FORMAT_BLACKANDWHITE` | 이진화 |
| `cv2.IMWRITE_PAM_FORMAT_GRAYSCALE` | 그레이스케일 |
| `cv2.IMWRITE_PAM_FORMAT_GRAYSCALE_ALPHA` | 그레이스케일 알파채널 |
| `cv2.IMWRITE_PAM_FORMAT_RGB` | 색상 이미지 |
| `cv2.IMWRITE_PAM_FORMAT_RGB_ALPHA` | 색상이미지 알파채널 |

</div>
</div>

### 요약(Summary)

> PAM 저장 방식을 설정합니다.
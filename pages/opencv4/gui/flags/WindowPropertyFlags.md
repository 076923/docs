---
title: 윈도우 속성 플래그
sidebar: opencv4_sidebar
permalink: WindowPropertyFlags
folder: opencv4
---

<ul id="profileTabs" class="nav nav-tabs">
    <li class="active"><a class="noCrossRef" href="#L1" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">C++</a></li>
    <li><a class="noCrossRef" href="#L2" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">C#</a></li>
    <li><a class="noCrossRef" href="#L3" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">Python</a></li>
</ul>

<div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="L1" markdown="1">

| 플래그             | 속성 | 설명                                                         |
| ----------------- | ------ | ---------------------------------------------------------- | 
| `WND_PROP_FULLSCREEN` | 0.0 | 최대화 |
| `WND_PROP_FULLSCREEN` | 1.0 | 전체 화면으로 표시 |
| `WND_PROP_AUTOSIZE` | 0.0 | 윈도우의 크기를 출력된 이미지 크기로 조절 |
| `WND_PROP_AUTOSIZE` | 1.0 | 윈도우 크기에 맞게 이미지 크기를 조절 |
| `WND_PROP_ASPECT_RATIO` | 0.0 | 이미지 비율을 최대한 유지 |
| `WND_PROP_ASPECT_RATIO` | 1.0 | 비율의 제한이 없는 경우 이미지를 최대한 확장 |
| `WND_PROP_OPENGL` | -1.0 | OpenGL을 지원하지 않는 윈도우 |
| `WND_PROP_OPENGL` | 0.0 | OpenGL을 지원하는 윈도우 |
| `WND_PROP_VISIBLE` | 0.0 | 창이 존재하지 않고 보이지 않음 |
| `WND_PROP_VISIBLE` | 1.0 | 창이 존재하고 보임 |
| `WND_PROP_TOPMOST` | 0.0 | 윈도우를 최상단으로 표시하지 않음 |
| `WND_PROP_TOPMOST` | 1.0 | 윈도우를 최상단으로 표시함 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 속성 | 설명                                                         |
| ----------------- | ------ | ---------------------------------------------------------- | 
| `WindowPropertyFlags.Fullscreen` | 0.0 | 최대화 |
| `WindowPropertyFlags.Fullscreen` | 1.0 | 전체 화면으로 표시 |
| `WindowPropertyFlags.AutoSize` | 0.0 | 윈도우의 크기를 출력된 이미지 크기로 조절 |
| `WindowPropertyFlags.AutoSize` | 1.0 | 윈도우 크기에 맞게 이미지 크기를 조절 |
| `WindowPropertyFlags.AspectRatio` | 0.0 | 이미지 비율을 최대한 유지 |
| `WindowPropertyFlags.AspectRatio` | 1.0 | 비율의 제한이 없는 경우 이미지를 최대한 확장 |
| `WindowPropertyFlags.OpenGL` | -1.0 | OpenGL을 지원하지 않는 윈도우 |
| `WindowPropertyFlags.OpenGL` | 0.0 | OpenGL을 지원하는 윈도우 |
| `WindowPropertyFlags.Visible` | 0.0 | 창이 존재하지 않고 보이지 않음 |
| `WindowPropertyFlags.Visible` | 1.0 | 창이 존재하고 보임 |
| `WindowPropertyFlags.Topmost` | 0.0 | 윈도우를 최상단으로 표시하지 않음 |
| `WindowPropertyFlags.Topmost` | 1.0 | 윈도우를 최상단으로 표시함 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 속성 | 설명                                                         |
| ----------------- | ------ | ---------------------------------------------------------- | 
| `cv2.WND_PROP_FULLSCREEN` | 0.0 | 최대화 |
| `cv2.WND_PROP_FULLSCREEN` | 1.0 | 전체 화면으로 표시 |
| `cv2.WND_PROP_AUTOSIZE` | 0.0 | 윈도우의 크기를 출력된 이미지 크기로 조절 |
| `cv2.WND_PROP_AUTOSIZE` | 1.0 | 윈도우 크기에 맞게 이미지 크기를 조절 |
| `cv2.WND_PROP_ASPECT_RATIO` | 0.0 | 이미지 비율을 최대한 유지 |
| `cv2.WND_PROP_ASPECT_RATIO` | 1.0 | 비율의 제한이 없는 경우 이미지를 최대한 확장 |
| `cv2.WND_PROP_OPENGL` | -1.0 | OpenGL을 지원하지 않는 윈도우 |
| `cv2.WND_PROP_OPENGL` | 0.0 | OpenGL을 지원하는 윈도우 |
| `cv2.WND_PROP_VISIBLE` | 0.0 | 창이 존재하지 않고 보이지 않음 |
| `cv2.WND_PROP_VISIBLE` | 1.0 | 창이 존재하고 보임 |
| `cv2.WND_PROP_TOPMOST` | 0.0 | 윈도우를 최상단으로 표시하지 않음 |
| `cv2.WND_PROP_TOPMOST` | 1.0 | 윈도우를 최상단으로 표시함 |

</div>
</div>

<br>

### 요약(Summary)

> 표시되는 윈도우의 세부 속성을 설정합니다.
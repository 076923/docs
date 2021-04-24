---
title: 윈도우 플래그
sidebar: opencv4_sidebar
permalink: WindowFlags
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
| `WINDOW_NORMAL` | 윈도우 크기를 조절할 수 있으며, 최대화된 창을 이전 크기로 복원 |
| `WINDOW_KEEPRATIO` | 이미지 비율을 최대한 유지 |
| `WINDOW_GUI_EXPANDED` | 상태 표시줄 및 도구 모음 표시 |
| `WINDOW_AUTOSIZE` | 윈도우 크기를 조절할 수 없으며, 이미지의 크기와 동일하게 표시 |
| `WINDOW_FULLSCREEN` | 윈도우를 최대화 |
| `WINDOW_GUI_NORMAL` | 이전 GUI 방식 사용 |
| `WINDOW_FREERATIO` | 비율의 제한이 없는 경우 이미지를 최대한 확장 |
| `WINDOW_OPENGL` | OpenGL을 지원하는 윈도우 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `WindowFlags.Normal` | 윈도우 크기를 조절할 수 있으며, 최대화된 창을 이전 크기로 복원 |
| `WindowFlags.KeepRatio` | 이미지 비율을 최대한 유지 |
| `WindowFlags.GuiExpanded` | 상태 표시줄 및 도구 모음 표시 |
| `WindowFlags.AutoSize` | 윈도우 크기를 조절할 수 없으며, 이미지의 크기와 동일하게 표시 |
| `WindowFlags.FullScreen` | 윈도우를 최대화 |
| `WindowFlags.GuiNormal` | 이전 GUI 방식 사용 |
| `WindowFlags.FreeRatio` | 비율의 제한이 없는 경우 이미지를 최대한 확장 |
| `WindowFlags.OpenGL` | OpenGL을 지원하는 윈도우 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.WINDOW_NORMAL` | 윈도우 크기를 조절할 수 있으며, 최대화된 창을 이전 크기로 복원 |
| `cv2.WINDOW_KEEPRATIO` | 이미지 비율을 최대한 유지 |
| `cv2.WINDOW_GUI_EXPANDED` | 상태 표시줄 및 도구 모음 표시 |
| `cv2.WINDOW_AUTOSIZE` | 윈도우 크기를 조절할 수 없으며, 이미지의 크기와 동일하게 표시 |
| `cv2.WINDOW_FULLSCREEN` | 윈도우를 최대화 |
| `cv2.WINDOW_GUI_NORMAL` | 이전 GUI 방식 사용 |
| `cv2.WINDOW_FREERATIO` | 비율의 제한이 없는 경우 이미지를 최대한 확장 |
| `cv2.WINDOW_OPENGL` | OpenGL을 지원하는 윈도우 |

</div>
</div>

<br>

### 요약(Summary)

> 표시되는 윈도우의 속성을 설정합니다.
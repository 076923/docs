---
title: 마우스 이벤트 형식
sidebar: opencv4_sidebar
permalink: MouseEventTypes
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
| `EVENT_MOUSEMOVE` | 마우스 포인터가 윈도우 위에서 움직일 때 |
| `EVENT_LBUTTONDOWN` | 마우스 왼쪽 버튼을 누를 때 |
| `EVENT_RBUTTONDOWN` | 마우스 오른쪽 버튼을 누를 때 |
| `EVENT_MBUTTONDOWN` | 마우스 휠 스크롤 버튼을 누를 때 |
| `EVENT_LBUTTONUP` | 마우스 왼쪽 버튼을 뗄 때 |
| `EVENT_RBUTTONUP` | 마우스 오른쪽 버튼을 뗄 때 |
| `EVENT_MBUTTONUP` | 마우스 휠 스크롤 버튼을 뗄 때 |
| `EVENT_LBUTTONDBLCLK` | 마우스 왼쪽 버튼을 더블 클릭할 때 |
| `EVENT_RBUTTONDBLCLK` | 마우스 오른쪽 버튼을 더블 클릭할 때 |
| `EVENT_MBUTTONDBLCLK` | 마우스 휠 스크롤 버튼을 더블 클릭할 때 |
| `EVENT_MOUSEWHEEL` | 상하 스크롤을 사용할 때 |
| `EVENT_MOUSEHWHEEL` | 좌우 스크롤을 사용할 때 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `MouseEventTypes.MouseMove` | 마우스 포인터가 윈도우 위에서 움직일 때 |
| `MouseEventTypes.LButtonDown` | 마우스 왼쪽 버튼을 누를 때 |
| `MouseEventTypes.RButtonDown` | 마우스 오른쪽 버튼을 누를 때 |
| `MouseEventTypes.MButtonDown` | 마우스 휠 스크롤 버튼을 누를 때 |
| `MouseEventTypes.LButtonUp` | 마우스 왼쪽 버튼을 뗄 때 |
| `MouseEventTypes.RButtonUp` | 마우스 오른쪽 버튼을 뗄 때 |
| `MouseEventTypes.MButtonUp` | 마우스 휠 스크롤 버튼을 뗄 때 |
| `MouseEventTypes.LButtonDoubleClick` | 마우스 왼쪽 버튼을 더블 클릭할 때 |
| `MouseEventTypes.RButtonDoubleClick` | 마우스 오른쪽 버튼을 더블 클릭할 때 |
| `MouseEventTypes.MButtonDoubleClick` | 마우스 휠 스크롤 버튼을 더블 클릭할 때 |
| `MouseEventTypes.MouseWheel` | 상하 스크롤을 사용할 때 |
| `MouseEventTypes.MouseHWheel` | 좌우 스크롤을 사용할 때 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.EVENT_MOUSEMOVE` | 마우스 포인터가 윈도우 위에서 움직일 때 |
| `cv2.EVENT_LBUTTONDOWN` | 마우스 왼쪽 버튼을 누를 때 |
| `cv2.EVENT_RBUTTONDOWN` | 마우스 오른쪽 버튼을 누를 때 |
| `cv2.EVENT_MBUTTONDOWN` | 마우스 휠 스크롤 버튼을 누를 때 |
| `cv2.EVENT_LBUTTONUP` | 마우스 왼쪽 버튼을 뗄 때 |
| `cv2.EVENT_RBUTTONUP` | 마우스 오른쪽 버튼을 뗄 때 |
| `cv2.EVENT_MBUTTONUP` | 마우스 휠 스크롤 버튼을 뗄 때 |
| `cv2.EVENT_LBUTTONDBLCLK` | 마우스 왼쪽 버튼을 더블 클릭할 때 |
| `cv2.EVENT_RBUTTONDBLCLK` | 마우스 오른쪽 버튼을 더블 클릭할 때 |
| `cv2.EVENT_MBUTTONDBLCLK` | 마우스 휠 스크롤 버튼을 더블 클릭할 때 |
| `cv2.EVENT_MOUSEWHEEL` | 상하 스크롤을 사용할 때 |
| `cv2.EVENT_MOUSEHWHEEL` | 좌우 스크롤을 사용할 때 |

</div>
</div>

<br>

### 요약(Summary)

> 입력된 마우스 플래그 형식을 반환합니다.
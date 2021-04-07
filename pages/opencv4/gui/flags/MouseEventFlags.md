---
title: 마우스 이벤트 플래그
sidebar: opencv4_sidebar
permalink: MouseEventFlags
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
| `EVENT_FLAG_LBUTTON` | 마우스 왼쪽 버튼을 누른 상태 |
| `EVENT_FLAG_RBUTTON` | 마우스 오른쪽 버튼을 누른 상태 |
| `EVENT_FLAG_MBUTTON` | 마우스 휠 스크롤 버튼을 누른 상태 |
| `EVENT_FLAG_CTRLKEY` | Ctrl 키를 누른 상태 |
| `EVENT_FLAG_SHIFTKEY` | Shift 키를 누른 상태 |
| `EVENT_FLAG_ALTKEY` | Alt 키를 누른 상태 |
| `> 65536` | 마우스 휠 스크롤 이벤트의 위쪽 또는 오른쪽 |
| `< -65536` | 마우스 휠 스크롤 이벤트의 아래쪽 또는 왼쪽 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `MouseEventFlags.LButton` | 마우스 왼쪽 버튼을 누른 상태 |
| `MouseEventFlags.RButton` | 마우스 오른쪽 버튼을 누른 상태 |
| `MouseEventFlags.MButton` | 마우스 휠 스크롤 버튼을 누른 상태 |
| `MouseEventFlags.CtrlKey` | Ctrl 키를 누른 상태 |
| `MouseEventFlags.ShiftKey` | Shift 키를 누른 상태 |
| `MouseEventFlags.AltKey` | Alt 키를 누른 상태 |
| `> 65536` | 마우스 휠 스크롤 이벤트의 위쪽 또는 오른쪽 |
| `< -65536` | 마우스 휠 스크롤 이벤트의 아래쪽 또는 왼쪽 |


</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.EVENT_FLAG_LBUTTON` | 마우스 왼쪽 버튼을 누른 상태 |
| `cv2.EVENT_FLAG_RBUTTON` | 마우스 오른쪽 버튼을 누른 상태 |
| `cv2.EVENT_FLAG_MBUTTON` | 마우스 휠 스크롤 버튼을 누른 상태 |
| `cv2.EVENT_FLAG_CTRLKEY` | Ctrl 키를 누른 상태 |
| `cv2.EVENT_FLAG_SHIFTKEY` | Shift 키를 누른 상태 |
| `cv2.EVENT_FLAG_ALTKEY` | Alt 키를 누른 상태 |
| `> 65536` | 마우스 휠 스크롤 이벤트의 위쪽 또는 오른쪽 |
| `< -65536` | 마우스 휠 스크롤 이벤트의 아래쪽 또는 왼쪽 |


</div>
</div>

### 요약(Summary)

> 입력된 마우스 이벤트 플래그를 반환합니다.
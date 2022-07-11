---
title: 히스토그램 비교 방식
sidebar: opencv4_sidebar
permalink: HistCompMethods
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
| `HISTCMP_CORREL` | 상관관계<br>$$ d(H_1,\ H_2) = \frac{\sum_I (H_1(I) - \bar{H_1}) (H_2(I) - \bar{H_2})}{\sqrt{\sum_I(H_1(I) - \bar{H_1})^2 \sum_I(H_2(I) - \bar{H_2})^2}} $$ <br> $$ \bar{H_k} = \frac{1}{N} \sum _J H_k(J) $$ <br> $$ N $$은 히스토그램 빈(Bin) 수 |
| `HISTCMP_CHISQR` | 카이제곱 검정<br>$$ d(H_1,\ H_2) = \sum _I \frac{\left(H_1(I)-H_2(I)\right)^2}{H_1(I)} $$ |
| `HISTCMP_INTERSECT` | 교집합<br>$$ d(H_1,\ H_2) = \sum _I \min (H_1(I), H_2(I)) $$ |
| `HISTCMP_BHATTACHARYYA` | Bhattacharyya 거리(헬린저 거리) <br> $$ d(H_1,\ H_2) = \sqrt{1 - \frac{1}{\sqrt{\bar{H_1} \bar{H_2} N^2}} \sum_I \sqrt{H_1(I) \cdot H_2(I)}} $$ |
| `HISTCMP_HELLINGER` | 헬린저 거리<br>$$ d(H_1,\ H_2) = \sqrt{1 - \frac{1}{\sqrt{\bar{H_1} \bar{H_2} N^2}} \sum_I \sqrt{H_1(I) \cdot H_2(I)}} $$ |
| `HISTCMP_CHISQR_ALT` | 카이제곱 검정 대안<br>$$ d(H_1,\ H_2) = 2 * \sum _I \frac{\left(H_1(I)-H_2(I)\right)^2}{H_1(I)+H_2(I)} $$ |
| `HISTCMP_KL_DIV` | 쿨백-라이블러 발산<br>$$ d(H_1,\ H_2) = \sum _I H_1(I) \log \left(\frac{H_1(I)}{H_2(I)}\right) $$ |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `HistCompMethods.Correl` | 상관관계<br>$$ d(H_1,\ H_2) = \frac{\sum_I (H_1(I) - \bar{H_1}) (H_2(I) - \bar{H_2})}{\sqrt{\sum_I(H_1(I) - \bar{H_1})^2 \sum_I(H_2(I) - \bar{H_2})^2}} $$ <br> $$ \bar{H_k} = \frac{1}{N} \sum _J H_k(J) $$ <br> $$ N $$은 히스토그램 빈(Bin) 수 |
| `HistCompMethods.Chisqr` | 카이제곱 검정<br>$$ d(H_1,\ H_2) = \sum _I \frac{\left(H_1(I)-H_2(I)\right)^2}{H_1(I)} $$ |
| `HistCompMethods.Intersect` | 교집합<br>$$ d(H_1,\ H_2) = \sum _I \min (H_1(I), H_2(I)) $$ |
| `HistCompMethods.Bhattacharyya` | Bhattacharyya 거리(헬린저 거리) <br> $$ d(H_1,\ H_2) = \sqrt{1 - \frac{1}{\sqrt{\bar{H_1} \bar{H_2} N^2}} \sum_I \sqrt{H_1(I) \cdot H_2(I)}} $$ |
| `HistCompMethods.Hellinger` | 헬린저 거리<br>$$ d(H_1,\ H_2) = \sqrt{1 - \frac{1}{\sqrt{\bar{H_1} \bar{H_2} N^2}} \sum_I \sqrt{H_1(I) \cdot H_2(I)}} $$ |
| `HistCompMethods.ChisqrAlt` | 카이제곱 검정 대안<br>$$ d(H_1,\ H_2) = 2 * \sum _I \frac{\left(H_1(I)-H_2(I)\right)^2}{H_1(I)+H_2(I)} $$ |
| `HistCompMethods.KLDiv` | 쿨백-라이블러 발산<br>$$ d(H_1,\ H_2) = \sum _I H_1(I) \log \left(\frac{H_1(I)}{H_2(I)}\right) $$ |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.HISTCMP_CORREL` | 상관관계<br>$$ d(H_1,\ H_2) = \frac{\sum_I (H_1(I) - \bar{H_1}) (H_2(I) - \bar{H_2})}{\sqrt{\sum_I(H_1(I) - \bar{H_1})^2 \sum_I(H_2(I) - \bar{H_2})^2}} $$ <br> $$ \bar{H_k} = \frac{1}{N} \sum _J H_k(J) $$ <br> $$ N $$은 히스토그램 빈(Bin) 수 |
| `cv2.HISTCMP_CHISQR` | 카이제곱 검정<br>$$ d(H_1,\ H_2) = \sum _I \frac{\left(H_1(I)-H_2(I)\right)^2}{H_1(I)} $$ |
| `cv2.HISTCMP_INTERSECT` | 교집합<br>$$ d(H_1,\ H_2) = \sum _I \min (H_1(I), H_2(I)) $$ |
| `cv2.HISTCMP_BHATTACHARYYA` | Bhattacharyya 거리(헬린저 거리) <br> $$ d(H_1,\ H_2) = \sqrt{1 - \frac{1}{\sqrt{\bar{H_1} \bar{H_2} N^2}} \sum_I \sqrt{H_1(I) \cdot H_2(I)}} $$ |
| `cv2.HISTCMP_HELLINGER` | 헬린저 거리<br>$$ d(H_1,\ H_2) = \sqrt{1 - \frac{1}{\sqrt{\bar{H_1} \bar{H_2} N^2}} \sum_I \sqrt{H_1(I) \cdot H_2(I)}} $$ |
| `cv2.HISTCMP_CHISQR_ALT` | 카이제곱 검정 대안<br>$$ d(H_1,\ H_2) = 2 * \sum _I \frac{\left(H_1(I)-H_2(I)\right)^2}{H_1(I)+H_2(I)} $$ |
| `cv2.HISTCMP_KL_DIV` | 쿨백-라이블러 발산<br>$$ d(H_1,\ H_2) = \sum _I H_1(I) \log \left(\frac{H_1(I)}{H_2(I)}\right) $$ |

</div>
</div>

<br>

### 요약(Summary)

> 히스토그램 비교 방식을 설정합니다.

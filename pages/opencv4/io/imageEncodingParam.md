---
title: 이미지 부호화 매개변수
sidebar: opencv4_sidebar
permalink: imageEncodingParam
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
| `IMWRITE_JPEG_QUALITY` | JPEG의 품질 설정(0~100) |
| `IMWRITE_JPEG_PROGRESSIVE` | JPEG의 점차 선명해짐 적용(0, 1) |
| `IMWRITE_JPEG_OPTIMIZE` | JPEG의 최적화 적용(0, 1) |
| `IMWRITE_JPEG_RST_INTERVAL` | JPEG의 마커 간격 설정(0~65535) |
| `IMWRITE_JPEG_LUMA_QUALITY` | JPEG의 루마 품질 적용(0~100) |
| `IMWRITE_JPEG_CHROMA_QUALITY` | JPEG의 크로마 품질 설정 (0~100) |
| `IMWRITE_PNG_COMPRESSION` | PNG의 압축 설정(0~100) |
| `IMWRITE_PNG_STRATEGY` | [PNG 형식 플래그](imwritePNGFlags) |
| `IMWRITE_PNG_BILEVEL` | PNG의 이진화 형식 설정(0, 1) |
| `IMWRITE_PXM_BINARY` | PPM, PGM, PBM의 이진화 형식 설정(0, 1) |
| `IMWRITE_EXR_TYPE` | [EXR 형식 플래그](imwriteEXRTypeFlags) |
| `IMWRITE_WEBP_QUALITY` | WEBP 품질 설정(0~100) |
| `IMWRITE_PAM_TUPLETYPE` | [PAM 형식 플래그](imwritePAMFlags) |
| `IMWRITE_TIFF_RESUNIT` | TIFF의 DPI 설정 |
| `IMWRITE_TIFF_XDPI` | TIFF의 DPI 설정 |
| `IMWRITE_TIFF_YDPI` | TIFF의 DPI 설정 |
| `IMWRITE_TIFF_COMPRESSION` | TIFF의 이미지 압축 체계 설정 |
| `IMWRITE_JPEG2000_COMPRESSION_X1000` | JPEG2000의 압축률 설정(0~1000) |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `ImwriteFlags.JpegQuality` | JPEG의 품질 설정(0~100) |
| `ImwriteFlags.JpegProgressive` | JPEG의 점차 선명해짐 적용(0, 1) |
| `ImwriteFlags.JpegOptimize` | JPEG의 최적화 적용(0, 1) |
| `ImwriteFlags.JpegRstInterval` | JPEG의 마커 간격 설정(0~65535) |
| `ImwriteFlags.JpegLumaQuality` | JPEG의 루마 품질 적용(0~100) |
| `ImwriteFlags.JpegChromaQuality` | JPEG의 크로마 품질 설정 (0~100) |
| `ImwriteFlags.PngCompression` | PNG의 압축 설정(0~100) |
| `ImwriteFlags.PngStrategy` | [PNG 형식 플래그](imwritePNGFlags) |
| `ImwriteFlags.PngBilevel` | PNG의 이진화 형식 설정(0, 1) |
| `ImwriteFlags.PxmBinary` | PPM, PGM, PBM의 이진화 형식 설정(0, 1) |
| `ImwriteFlags.ExrType` | [EXR 형식 플래그](imwriteEXRTypeFlags) |
| `ImwriteFlags.WebPQuality` | WEBP 품질 설정(0~100) |
| `ImwriteFlags.PamTupleType` | [PAM 형식 플래그](imwritePAMFlags) |
| `ImwriteFlags.TiffResUnit` | TIFF의 DPI 설정 |
| `ImwriteFlags.TiffXDpi` | TIFF의 DPI 설정 |
| `ImwriteFlags.TiffYDpi` | TIFF의 DPI 설정 |
| `ImwriteFlags.TiffCompression` | <a data-toggle="tooltip" data-original-title="{{site.data.glossary.Not_supported}}">TIFF의 이미지 압축 체계 설정</a> |
| `ImwriteFlags.Jpeg2000CompressionX1000` | <a data-toggle="tooltip" data-original-title="{{site.data.glossary.Not_supported}}">JPEG2000의 압축률 설정(0~1000)</a> |


</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.IMWRITE_JPEG_QUALITY` | JPEG의 품질 설정(0~100) |
| `cv2.IMWRITE_JPEG_PROGRESSIVE` | JPEG의 점차 선명해짐 적용(0, 1) |
| `cv2.IMWRITE_JPEG_OPTIMIZE` | JPEG의 최적화 적용(0, 1) |
| `cv2.IMWRITE_JPEG_RST_INTERVAL` | JPEG의 마커 간격 설정(0~65535) |
| `cv2.IMWRITE_JPEG_LUMA_QUALITY` | JPEG의 루마 품질 적용(0~100) |
| `cv2.IMWRITE_JPEG_CHROMA_QUALITY` | JPEG의 크로마 품질 설정 (0~100) |
| `cv2.IMWRITE_PNG_COMPRESSION` | PNG의 압축 설정(0~100) |
| `cv2.IMWRITE_PNG_STRATEGY` | [PNG 형식 플래그](imwritePNGFlags) |
| `cv2.IMWRITE_PNG_BILEVEL` | PNG의 이진화 형식 설정(0, 1) |
| `cv2.IMWRITE_PXM_BINARY` | PPM, PGM, PBM의 이진화 형식 설정(0, 1) |
| `cv2.IMWRITE_EXR_TYPE` | [EXR 형식 플래그](imwriteEXRTypeFlags) |
| `cv2.IMWRITE_WEBP_QUALITY` | WEBP 품질 설정(0~100) |
| `cv2.IMWRITE_PAM_TUPLETYPE` | [PAM 형식 플래그](imwritePAMFlags) |
| `cv2.IMWRITE_TIFF_RESUNIT` | TIFF의 DPI 설정 |
| `cv2.IMWRITE_TIFF_XDPI` | TIFF의 DPI 설정 |
| `cv2.IMWRITE_TIFF_YDPI` | TIFF의 DPI 설정 |
| `cv2.IMWRITE_TIFF_COMPRESSION` | TIFF의 이미지 압축 체계 설정 |
| `cv2.IMWRITE_JPEG2000_COMPRESSION_X1000` | JPEG2000의 압축률 설정(0~1000) |


</div>
</div>

### 요약(Summary)

> 이미지 변환 방식을 설정합니다.
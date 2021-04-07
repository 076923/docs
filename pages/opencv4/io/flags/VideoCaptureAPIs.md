---
title: 비디오 읽기 백엔드 API 플래그
sidebar: opencv4_sidebar
permalink: VideoCaptureAPIs
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
| `CAP_ANY` | 플래그 자동 감지 |
| `CAP_V4L` | Video4Linux / Video4Linux2 지원 |
| `CAP_V4L2` | Video4Linux / Video4Linux2 지원 |
| `CAP_FIREWIRE` | IEEE 1394 드라이버 |
| `CAP_FIREWARE` | IEEE 1394 드라이버 |
| `CAP_IEEE1394` | IEEE 1394 드라이버 |
| `CAP_DC1394` | IEEE 1394 드라이버 |
| `CAP_CMU1394` | IEEE 1394 드라이버 |
| `CAP_DSHOW` | 다이렉트쇼 |
| `CAP_OPENNI` | OpenNI(키넥트) |
| `CAP_OPENNI_ASUS` | OpenNI(에이수스 Xtion) |
| `CAP_ANDROID` | 안드로이드 |
| `CAP_XIAPI` | XIMEA API |
| `CAP_AVFOUNDATION` | iOS용 AVFoundation |
| `CAP_GIGANETIX` | 스마텍 Giganetix GigE Vision SDK |
| `CAP_MSMF` | 마이크로소프트 Media Foundation |
| `CAP_WINRT` | 윈도우 런타임 마이크로소프트 Media Foundation |
| `CAP_INTELPERC` | 인텔 RealSense™ |
| `CAP_REALSENSE` | 인텔 RealSense™ |
| `CAP_OPENNI2` | OpenNI2(키넥트) |
| `CAP_OPENNI2_ASUS` | OpenNI2(에이수스 Xtion, Occipital(후두부) 구조 센서) |
| `CAP_GPHOTO2` | gPhoto2 라이브러리 |
| `CAP_GSTREAMER` | GStreamer 프레임워크 |
| `CAP_FFMPEG` | FFmpeg 라이브러리 |
| `CAP_IMAGES` | 이미지 시퀀스 |
| `CAP_ARAVIS` | Aravis 소프트웨어 개발 키트(SDK) |
| `CAP_OPENCV_MJPEG` | OpenCV 내장 모션 JPEG 코덱 |
| `CAP_INTEL_MFX` | 인텔 미디어 소프트웨어 개발 키트(SDK) |
| `CAP_XINE` | 리눅스용 xine 엔진 |
| `CAP_UEYE` | uEye 카메라 API |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `VideoCaptureAPIs.ANY` | 플래그 자동 감지 |
| `VideoCaptureAPIs.V4L` | Video4Linux / Video4Linux2 지원 |
| `VideoCaptureAPIs.V4L2` | Video4Linux / Video4Linux2 지원 |
| `VideoCaptureAPIs.FIREWIRE` | IEEE 1394 드라이버 |
| `VideoCaptureAPIs.FIREWARE` | IEEE 1394 드라이버 |
| `VideoCaptureAPIs.IEEE1394` | IEEE 1394 드라이버 |
| `VideoCaptureAPIs.DC1394` | IEEE 1394 드라이버 |
| `VideoCaptureAPIs.CMU1394` | IEEE 1394 드라이버 |
| `VideoCaptureAPIs.DSHOW` | 다이렉트쇼 |
| `VideoCaptureAPIs.OPENNI` | OpenNI(키넥트) |
| `VideoCaptureAPIs.OPENNI_ASUS` | OpenNI(에이수스 Xtion) |
| `VideoCaptureAPIs.ANDROID` | 안드로이드 |
| `VideoCaptureAPIs.XIAPI` | XIMEA API |
| `VideoCaptureAPIs.AVFOUNDATION` | iOS용 AVFoundation |
| `VideoCaptureAPIs.GIGANETIX` | 스마텍 Giganetix GigE Vision SDK |
| `VideoCaptureAPIs.MSMF` | 마이크로소프트 Media Foundation |
| `VideoCaptureAPIs.WINRT` | 윈도우 런타임 마이크로소프트 Media Foundation |
| `VideoCaptureAPIs.INTELPERC` | 인텔 RealSense™ |
| `VideoCaptureAPIs.REALSENSE` | 인텔 RealSense™ |
| `VideoCaptureAPIs.OPENNI2` | OpenNI2(키넥트) |
| `VideoCaptureAPIs.OPENNI2_ASUS` | OpenNI2(에이수스 Xtion, Occipital(후두부) 구조 센서) |
| `VideoCaptureAPIs.GPHOTO2` | gPhoto2 라이브러리 |
| `VideoCaptureAPIs.GSTREAMER` | GStreamer 프레임워크 |
| `VideoCaptureAPIs.FFMPEG` | FFmpeg 라이브러리 |
| `VideoCaptureAPIs.IMAGES` | 이미지 시퀀스 |
| `VideoCaptureAPIs.ARAVIS` | Aravis 소프트웨어 개발 키트(SDK) |
| `VideoCaptureAPIs.OPENCV_MJPEG` | OpenCV 내장 모션 JPEG 코덱 |
| `VideoCaptureAPIs.INTEL_MFX` | 인텔 미디어 소프트웨어 개발 키트(SDK) |
| `VideoCaptureAPIs.XINE` | 리눅스용 xine 엔진 |
| `VideoCaptureAPIs.CAP_UEYE` | uEye 카메라 API |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.CAP_ANY` | 플래그 자동 감지 |
| `cv2.CAP_V4L` | Video4Linux / Video4Linux2 지원 |
| `cv2.CAP_V4L2` | Video4Linux / Video4Linux2 지원 |
| `cv2.CAP_FIREWIRE` | IEEE 1394 드라이버 |
| `cv2.CAP_FIREWARE` | IEEE 1394 드라이버 |
| `cv2.CAP_IEEE1394` | IEEE 1394 드라이버 |
| `cv2.CAP_DC1394` | IEEE 1394 드라이버 |
| `cv2.CAP_CMU1394` | IEEE 1394 드라이버 |
| `cv2.CAP_DSHOW` | 다이렉트쇼 |
| `cv2.CAP_OPENNI` | OpenNI(키넥트) |
| `cv2.CAP_OPENNI_ASUS` | OpenNI(에이수스 Xtion) |
| `cv2.CAP_ANDROID` | 안드로이드 |
| `cv2.CAP_XIAPI` | XIMEA API |
| `cv2.CAP_AVFOUNDATION` | iOS용 AVFoundation |
| `cv2.CAP_GIGANETIX` | 스마텍 Giganetix GigE Vision SDK |
| `cv2.CAP_MSMF` | 마이크로소프트 Media Foundation |
| `cv2.CAP_WINRT` | 윈도우 런타임 마이크로소프트 Media Foundation |
| `cv2.CAP_INTELPERC` | 인텔 RealSense™ |
| `cv2.CAP_REALSENSE` | 인텔 RealSense™ |
| `cv2.CAP_OPENNI2` | OpenNI2(키넥트) |
| `cv2.CAP_OPENNI2_ASUS` | OpenNI2(에이수스 Xtion, Occipital(후두부) 구조 센서) |
| `cv2.CAP_GPHOTO2` | gPhoto2 라이브러리 |
| `cv2.CAP_GSTREAMER` | GStreamer 프레임워크 |
| `cv2.CAP_FFMPEG` | FFmpeg 라이브러리 |
| `cv2.CAP_IMAGES` | 이미지 시퀀스 |
| `cv2.CAP_ARAVIS` | Aravis 소프트웨어 개발 키트(SDK) |
| `cv2.CAP_OPENCV_MJPEG` | OpenCV 내장 모션 JPEG 코덱 |
| `cv2.CAP_INTEL_MFX` | 인텔 미디어 소프트웨어 개발 키트(SDK) |
| `cv2.CAP_XINE` | 리눅스용 xine 엔진 |
| `cv2.CAP_UEYE` | uEye 카메라 API |

</div>
</div>

### 요약(Summary)

> 비디오 읽기 API 백엔드를 설정하거나 불러옵니다.
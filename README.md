# stm32_RTOS
 stm32 보드 위에서 freeRTOS를 사용하여 3가지 task를 시분할하여 작업해보았습니다. (유튜브 동영상)
 
[![](http://img.youtube.com/vi/5eZYihaHwP8/0.jpg)](https://youtu.be/5eZYihaHwP8) 


https://youtu.be/5eZYihaHwP8

<br>

## 1. 프로젝트 목표
- ARM core인 STM32f4보드에서 freeRTOS로 센서3개 시분할하여 인식한다.

## 2. 프로젝트 상세 내용
 보통 LED를 같은 속도로 점멸 시킬 때는 상관없지만 다른 속도로 점멸 
 시켜야 하는 경우가 생깁니다. 이런 경우에는  2가지 일을 RTOS를 사용해서 
 시분할 하면 가능합니다.  저는 3가지 task로 나누었고 각각 다른 주기로 
 작동하도록 시분할 시켜서 작업해보았습니다. 
 
- HW: stm32F429zi보드, LED 2개, sound 센서, rotation센서, touch센서 
- SW: UART interrupt, GPIO, freeRTOS, ADC
<br>

## 3. 영상이나 사진
![image](![image](https://user-images.githubusercontent.com/81784631/135321041-13e9880c-fcc7-49a7-ac33-10673c234ba9.png)
)



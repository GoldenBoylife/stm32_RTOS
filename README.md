# stm32_RTOS
 stm32 보드 위에서 freeRTOS를 사용하여 3가지 task를 시분할하여 작업해보았습니다. (유튜브 동영상)
 
[![](http://img.youtube.com/vi/p9Hc8ghqyvo/0.jpg)](https://youtu.be/p9Hc8ghqyvo) 


https://youtu.be/p9Hc8ghqyvo

<br>

## 2. 프로젝트 목표
- freeRTOS를 stm32에서 구현

## 3. 프로젝트 상세 내용
 보통 LED를 같은 속도로 점멸 시킬 때는 상관없지만 다른 속도로 점멸 시켜야 하는 경우가 생깁니다. 이런 경우에는 
 2가지 일을 RTOS를 사용해서 시분할 하면 가능합니다. 
 저는 3가지 task로 나누었고 각각 다른 주기로 작동하도록 시분할 시켜서 작업해보았습니다. 
 
- HW: stm32F429zi보드, LED 2개, 
- SW: UART interrupt, GPIO, freeRTOS

<br>

## 5. 영상이나 사진
![image](https://user-images.githubusercontent.com/81784631/135242603-717a15cb-2f47-4756-af7a-b3dda8e933eb.png)


[![Grepp_A#](http://img.youtube.com/vi/WPJwRBtUBCQ/0.jpg)](https://www.youtube.com/embed/WPJwRBtUBCQ) 




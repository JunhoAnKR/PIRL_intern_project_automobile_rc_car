# PIRL_intern_project_automobile_rc_car

### 1. code 목록
- main.py : 최종적으로 command에서 실행시키는 파일
- rasp_serial.py : RC car의 steering 및 throttle을 조정하는 파일
- actuator.py : rasp_serial.py에서 사용될 함수 정의 파일
- config.py : rasp_serial.py에서 사용될 기본 변수값 저장 파일
- Camera.py : raspberrypi 카메라 크기 및 전송 frame수 등 카메라 설정 파일
- server_connect.py : server와 연결 시 실행되는 파일

### 2. 코드 실행
1) 라즈베리파이용 외장배터리 연결 후 초록불이 깜빡거리지 않을 때까지 대기
2) 라즈베리파이용 외장배터리 연결 후 ESC(검정색 모듈)를 on으로 변경
3) 서버에서 라즈베리파이로 원격 접속: ssh pi@192.168.0.7 .
4) 경로로 이동: cd Desktop/raspberry_origin/raspberry
5) file 실행: python3 main.py
6) 서버와 통신 시작이 되고,
7) 이 때, 캘리브레이션(조율을 위한 공회전)되므로 동키카를 손으로 들고 있어야 함
8) 모니터에 roi, object detecting 이미지가 뜨면 주행 가능


## ! 주의
#### 1. rasp_serial.py 코드 실행을 위해서는 코드 가장 위에 주석처리된 코드를 복사에 cmd창을 이용해 설치해야한다.

```
  sudo pip3 install adafruit-circuitpython-PCA9685
  
  sudo pip3 install Adafruit_PCA9685
  
```

#### 2. donkey car의 경우 I2C 통신을 하기 때문에 raspberrypi가 I2C통신이 가능하도록 설정해줘야 한다.

참조 링크 : <https://learn.sparkfun.com/tutorials/raspberry-pi-spi-and-i2c-tutorial?_ga=2.253783691.2068425467.1587036675-1985686237.1587036675>

  

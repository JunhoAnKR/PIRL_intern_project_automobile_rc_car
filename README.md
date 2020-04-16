# PIRL_intern_project_automobile_rc_car

1. code 목록
- main.py : 최종적으로 command에서 실행시키는 파일
- rasp_serial.py : RC car의 steering 및 throttle을 조정하는 파일
- actuator.py : rasp_serial.py에서 사용될 함수 정의 파일
- config.py : rasp_serial.py에서 사용될 기본 변수값 저장 파일
- Camera.py : raspberrypi 카메라 크기 및 전송 frame수 등 카메라 설정 파일
- server_connect.py : server와 연결 시 실행되는 파일

## ! 주의
rasp_serial.py 코드 실행을 위해서는 코드 가장 위에 주석처리된 코드를 복사에 cmd창을 이용해 설치해야한다.

  sudo pip3 install adafruit-circuitpython-PCA9685
  sudo pip3 install Adafruit_PCA9685
  

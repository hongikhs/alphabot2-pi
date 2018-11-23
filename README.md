# alphabot2-pi

1. 라즈베리파이 SD카드의 config.txt 파일에 다음을 추가한다. (https://tibyte.kr/258)
<pre>enable_uart=1</pre>

2. 터미널 프로그램으로 접속 후, /etc/wpa_supplicant/wpa_supplicant.conf 파일에 다음을 추가한다. (https://acertainlog.wordpress.com/2015/06/21/%EB%9D%BC%EC%A6%88%EB%B2%A0%EB%A6%AC-%ED%8C%8C%EC%9D%B4%EC%9D%98-%ED%84%B0%EB%AF%B8%EB%84%90%EC%97%90%EC%84%9C-wifi-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0/)
<pre>network={
        ssid="무선랜이름"
        psk="무선랜암호"
        key_mgmt=WPA-PSK
}</pre>

3. 파이썬 라이브러리를 설치한다.
<pre>pip3 install wiringpi
pip3 install RPi.GPIO
pip3 install spidev
sudo apt-get update
sudo apt-get install python-imaging</pre>

4. 
<pre>wget https://www.waveshare.com/w/upload/e/ee/AlphaBot2-Demo.7z
sudo apt-get install p7zip
7zr x AlphaBot2-Demo.7z
cd AlphaBot2-Demo/Raspberry\ Pi/
tar xfz AlphaBot2.tar.gz
mv AlphaBot2 ~/
cd</pre>

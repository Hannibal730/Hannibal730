# Google 저장소 정보를 우분투 시스템에 추가
 sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'

# Google 저장소 공개키 다운로드 및 등록
 wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add -

# apt 패키지 업데이트
 sudo apt update

# Chrome 패키지 업데이트 
 sudo apt install google-chrome-stable

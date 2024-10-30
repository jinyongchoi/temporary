# temporary
# 1. 프로그램 설치 전 우분투 시스템 패키지 업데이트
$ sudo apt-get update
 
# 2. 필요한 패키지 설치
$ sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent software-properties-common
 
# 3. Docker의 공식 GPG 키 추가
 
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
 
# 4. Docker의 공식 apt 저장소 추가
 
$ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

 
# 5. 시스템 패키지 업데이트
$ sudo apt-get update
 
# 6. Docker 설치
 
$ sudo apt-get install docker-ce docker-ce-cli containerd.io

# Docker Compose 설치
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

# 다운로드 한 파일에 권한 설정
$ sudo chmod +x /usr/local/bin/docker-compose
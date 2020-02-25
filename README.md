# Setup-Macbook-for-developer
맥북 초기 사용시 셋팅이 필요한 내용을 모아 보았습니다.

참고 사이트: https://subicura.com/2017/11/22/mac-os-development-environment-setup.html,


- 기본 시스템 환경설정
  - dock:
    - 윈도우 최소화 효과: 크기효과
  - mission control:
    - space를 사용내역에따라 자동으로 재정렬 체크해제
  - 언어 및 지역:
    - 시간 포맷: 24시간제
  - 손쉬운 사용
    - 포인터 제어기
      - 트랙패드 옵션
        - 드래그 활성화 -> 세 손가락 드래그
  - 키보드
    - 외장 키보드에서 F1,F2 등의 키를 표준 기능 키로 사용 체크
    - 텍스트
      - 자동수정 및 스마트 인용 및 대시사용 체크해제
    - 보조키
      - ctrl, command 키 서로 전환
  - 마우스
    스크롤 방향: 자연스럽게 체크
  - 트랙패드 
     스크롤 방향: 자연스럽게 체크
  - 날짜 및 시간
    - 시계
      - 시간에 초를 표시 체크
      - 날짜옵션: 날짜보기 체크
- finder 설정
  - 환경설정
    새로운 Finder 윈도우에서 보기: 사용자 home 디렉토리로 설정
    - 사이드바
      - 사이드바에서 항목보기 사용자 home 디렉토리 체크
    - 고급
      - 모든 파일 확장자 보기 체크
- 다운로드 폴더 설정
  다운로드 폴더 finder로 열기 -> view -> show view options 선택
    - 다음으로 그룹화: 추가된 날짜
    - 정렬: 이름
  
- 한/영 전환키 설정 (karabiner)
- 메모 내용 import/export
- 크롬 설치
  - 크롬 개인정보 설정
- 인터넷 브라우저 즐겨찾기 import/export
- 한글입력시 백틱(`) 입력 문제 설정
- 마우스 스크롤 휠 위/아래 방향 반전 설정 (logitech options, 맥 어플사용)
- terminal에서 xcode-cli 설치
  - xcode-select --install
- iterm2 / zsh / oh-my-zsh 설정
- brew 설치
- git설치: brew install git git-lfs  
  git config --global core.precomposeunicode true  
  git config --global core.quotepath false  
    
  git config --local --unset credential.helper  
  git config --global --unset credential.helper  
  git config --system --unset credential.helper  
- iterm2 설치
  brew cask install iterm2
  - zsh 설치
    - 참고 https://beomi.github.io/2017/07/07/Beautify-ZSH/  
    brew install zsh
  - ohmyzsh 설치
  - zsh-syntax-highlighting 설치
    - (추가) 터미널에서 사용자 컴퓨터 이름 가리기: https://beomi.github.io/2018/01/30/Hide-username-on-MAC-terminal/
  - zsh-autosuggestions 설치
  - plugin 참고: https://nachwon.github.io/how-to-install-zsh-plugins/
- 앱스토어에서 xcode 설치

- mds_store CPU 과점유 방지
  - 원인: spotlight에서 빠른 검색을 보장하기위해 파일들에 대한 indexing 실행하는걸로 추측
  - 해결 방안: 많은 파일이 있지만 spotlight 검색이 필요하지 않은 폴더를 따로 설정
    - 시스템 환경설정 -> spotlight -> 개인정보보호탭 -> index하지 않을 폴더 추가 (개발 dev 폴더 추가)
    
- vscode 설치
  - setting sync로 extension 동기화
- nvm 으로 node 설치
  참고: http://junsikshim.github.io/2016/01/29/Mac%EC%97%90%EC%84%9C-Node.js-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0.html

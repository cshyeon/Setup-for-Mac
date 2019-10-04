# Setup-for-Mac
맥북 초기 사용시 셋팅이 필요한 내용을 모아 보았습니다.

- 한/영 전환키 설정 (karabiner)
- 한글입력시 백틱(`) 입력 문제 설정
- 마우스 스크롤 휠 위/아래 방향 반전 설정 (logitech 유틸리티, 맥 어플사용)
- iterm2 / zsh / oh-my-zsh 설정
- brew 설치

- mds_store CPU 과점유 방지
  - 원인: spotlight에서 빠른 검색을 보장하기위해 파일들에 대한 indexing 실행하는걸로 추측
  - 해결 방안: 많은 파일이 있지만 spotlight 검색이 필요하지 않은 폴더를 따로 설정
    - 시스템 환경설정 -> spotlight -> 개인정보보호탭 -> 개발관련 폴더 추가

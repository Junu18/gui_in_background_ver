🚀 GitHub Auto Upload System
이미지 표시
이미지 표시
이미지 표시
GitHub 자동 업로드 시스템은 지정된 폴더의 파일을 자동으로 GitHub 저장소에 업로드하는 강력한 도구입니다. 프로필 기반 다중 환경 관리, GUI/트레이 모드 지원, 실시간 파일 감시 등 다양한 기능을 제공합니다.
✨ 주요 기능
🎯 핵심 기능

📤 자동 업로드: 파일 변경 감지 시 즉시 GitHub에 업로드
⏰ 스케줄 업로드: 지정된 시간에 자동으로 업로드
🔄 하이브리드 모드: 실시간 + 스케줄 업로드 결합
🏷️ 프로필 관리: 다중 환경(개인/회사/학교) 독립 관리
📊 업로드 기록: 상세한 업로드 이력 및 통계

🖥️ 사용자 인터페이스

📋 GUI 모드: 직관적인 그래픽 인터페이스
🌙 백그라운드 모드: 시스템 트레이에서 조용히 실행
🔄 모드 전환: GUI ↔ 백그라운드 모드 자유 전환
📢 알림 시스템: 실시간 상태 알림

🛠️ 고급 기능

📚 백준 연동: solved.ac 문제 크롤링 및 브라우저 연동
🔍 파일 필터링: 확장자별 업로드 파일 선택
📈 통계 분석: 업로드 성공률, 용량, 빈도 분석
🔒 보안 관리: GitHub Token 안전 저장

📁 프로젝트 구조
GitHub_Auto_Upload/
├── 📋 main_gui.py           # 메인 GUI (트레이 기능 포함)
├── ⚙️ setup_gui.py          # 환경설정 GUI
├── 📚 baekjoon_gui.py       # 백준 문제 풀이 GUI
├── 🔧 env_generate.py       # 환경 설정 생성 엔진
├── 📤 main_upload.py        # GitHub 업로드 메인 엔진
├── 📊 upload_history.py     # 업로드 기록 관리
├── 📦 requirements.txt      # 필요 라이브러리 목록
├── 📄 README.md            # 프로젝트 문서
├── 🔒 .env                 # 환경 변수 (자동 생성)
├── 🏷️ .env_프로필명         # 프로필별 설정 파일
├── 📋 profiles.json        # 프로필 목록 관리
├── 📊 upload_history.json  # 업로드 기록 데이터
└── 🔒 .gitignore          # Git 제외 파일 설정
🛠️ 기술 스택
분야기술언어Python 3.11+GUItkinter, pystrayGitHub APIrequests, PyGithub파일 감시watchdog스케줄링schedule웹 크롤링beautifulsoup4이미지 처리Pillow프로세스 관리psutil
📦 설치 방법
1️⃣ 저장소 클론
bashgit clone https://github.com/your-username/GitHub_Auto_Upload.git
cd GitHub_Auto_Upload
2️⃣ Python 환경 확인
bashpython --version  # Python 3.11+ 권장
3️⃣ 의존성 설치
bashpip install -r requirements.txt
4️⃣ 프로그램 실행
bashpython main_gui.py
🚀 빠른 시작
Step 1: 환경설정

GitHub Token 발급

GitHub → Settings → Developer settings → Personal access tokens
repo 권한 선택하여 토큰 생성


프로필 생성

메인 GUI에서 "⚙️ 환경설정" 클릭
프로필 별명, GitHub 정보, 감시 폴더 입력
"✅ 완료" 버튼으로 프로필 생성



Step 2: 업로드 시작

GUI 모드
bashpython main_gui.py
# "🚀 업로드 시작" 버튼 클릭

백그라운드 모드
bashpython main_gui.py
# "🌙 백그라운드 모드" 버튼 클릭
# 트레이 아이콘에서 "▶️ 업로드 시작"


Step 3: 파일 업로드

설정한 감시 폴더에 파일 추가/수정
자동으로 GitHub 저장소에 업로드됨
업로드 기록에서 결과 확인

📋 사용 가이드
🔧 업로드 모드
모드설명사용 시점🔄 실시간파일 변경 즉시 업로드개발 중 즉시 백업⏰ 예약지정 시간에만 업로드일정한 시간에 정리🔄⏰ 혼합실시간 + 예약 결합완벽한 자동화
🏷️ 프로필 관리
bash# 프로필 예시
📋 개인프로젝트    → user1/personal-repo
📋 회사업무       → company/work-repo  
📋 학교과제       → student/homework-repo
각 프로필은 독립적인 설정을 가지며, 쉽게 전환할 수 있습니다.
📊 지원 파일 형식
기본 지원: py, txt, md, json, js, html, css
사용자 정의 가능: 환경설정에서 원하는 확장자 추가
🎮 고급 사용법
📚 백준 문제 풀이
bashpython baekjoon_gui.py
# 또는 메인 GUI에서 "📚 백준 문제 풀기"

solved.ac Class 1~10 문제 크롤링
브라우저에서 문제 바로 열기
코딩 테스트 준비에 유용

📊 업로드 통계

성공/실패 건수 및 성공률
일별/주별 업로드 빈도
파일별 업로드 횟수
총 업로드 용량

🔍 문제 해결
Q: 업로드가 안 돼요!
bash# 1. GitHub 토큰 확인
# 2. 저장소 권한 확인  
# 3. 파일 확장자 확인
# 4. 네트워크 연결 확인
Q: 프로그램이 꺼져요!
bash# 백그라운드 모드 사용
python main_gui.py
# "🌙 백그라운드 모드" 클릭
Q: 파일이 너무 많아요!
bash# 파일 필터링 설정
# 환경설정 → 파일 형식 설정
🔧 개발자 정보
개발 환경

Python: 3.11.7 (권장)
OS: Windows 10/11, macOS, Linux
IDE: VS Code, PyCharm 등

빌드 방법
bash# 실행 파일 생성
pip install pyinstaller
pyinstaller --onefile --windowed main_gui.py
디버깅
bash# 콘솔에서 직접 실행
python main_upload.py  # 업로드 엔진 단독 실행
python setup_gui.py   # 환경설정만 실행
🤝 기여하기

Fork 버튼 클릭
Feature branch 생성 (git checkout -b feature/AmazingFeature)
커밋 (git commit -m 'Add some AmazingFeature')
Push (git push origin feature/AmazingFeature)
Pull Request 생성

기여 가이드라인

코드 스타일: PEP 8 준수
커밋 메시지: 한글/영문 자유
테스트: 주요 기능 동작 확인
문서화: README 업데이트

📄 라이선스
이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 LICENSE 파일을 참조하세요.
🙏 감사의 말

GitHub API: 강력한 저장소 관리 기능
Python 커뮤니티: 훌륭한 라이브러리들
solved.ac: 백준 문제 정보 제공
기여자들: 프로젝트 발전에 도움을 주신 모든 분들

📞 연락처

이슈 제보: GitHub Issues
기능 제안: GitHub Discussions
이메일: your-email@example.com


🎯 버전 히스토리
v1.0.0 (2025-07-21)

✨ 초기 릴리즈
🚀 기본 업로드 기능
🏷️ 프로필 관리 시스템
📋 GUI 인터페이스

v1.1.0 (2025-07-21)

🌙 백그라운드 모드 추가
📊 업로드 기록 시스템
📚 백준 문제 연동
🔧 다양한 버그 수정


⭐ 이 프로젝트가 도움이 되었다면 Star를 눌러주세요!
🔄 최신 업데이트는 Watch 버튼으로 받아보세요!
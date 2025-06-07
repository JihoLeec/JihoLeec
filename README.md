# 강의 요약 및 퀴즈 생성기

> <span style="color:gray"><strong>단국대학교 오픈소스SW기초 6분반 15조</strong><br>
조원: 박수빈, 변윤성, 이지호</span>
<br>

## 프로젝트 소개

본 프로젝트는 강의 내용을 자동으로 요약하고, 요약된 내용을 바탕으로 관련 퀴즈를 생성하는 웹 애플리케이션이다. 사용자는 강의 음성을 업로드해 텍스트로 변환(STT, Speech to Text)할 수 있으며 이 내용을 기반으로 핵심 내용을 간결하게 요약한다.

STT 기능은 Microsoft Azure의 음성 인식 서비스를 활용하여 높은 정확도와 안정성을 보장한다. 요약은 한국어 맞춤형 딥러닝 모델인 KoBART와 TextRank 알고리즘을 병행 사용하여 문서의 주요 내용을 효과적으로 추출하도록 했다.

이후 요약된 내용을 토대로 빈칸, OX 퀴즈 등의 문제를 자동으로 생성하여 학습자의 이해도를 점검할 수 있도록 설계했다. 프론트엔드에서는 React를 사용하여 사용자 친화적인 인터페이스를 구현하였고, 백엔드는 Python Flask 기반으로 API 서버를 구축하여 데이터를 처리를 구현했다.

<br>
## 디렉토리 구조

디렉토리의 자세한 파일은 각 작업 브랜치에서 확인하실 수 있습니다.
```bash
C:.
│  .gitignore
│  README.md
│
├─backend                              
│  │  .env                              
│  │  requirements.txt                 
│  │
│  └─app
│      │  main.py    
│      ├─preprocess                 
│      ├─quiz_list
│      ├─stt
│      └─summary
|
└─frontend
    │  package-lock.json
    │  package.json
    │
    ├─public
    └─src
        ├─components
        └─pages
```
<br>

## 설치 및 실행 방법

### 프로젝트 클론
```bash
git clone https://github.com/iamdbstjd/OS_15
cd OS_15
```
### 백엔드 서버 실행 후 프론트엔드 실행
```bash
# 1. 가상환경 생성 및 활성화(선택 사항)
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows

# 2. 의존성 설치
cd backend
pip install -r requirements.txt

# 3. 백엔드 서버 실행
uvicorn app.main:app

# 4. 프론트엔드 실행
cd ../frontend
npm install
npm start

# 참고: 서버 실행 주소
> 백엔드: http://localhost:8000  
> 프론트엔드: http://localhost:3000
```


<div align="center">

# ✨ WELCOME ✨
<br/><br/>

###  **I am just a potato🥔**
<br/><br/>

### ✉️ Contact
<br/>
<a href = "https://www.instagram.com/jiho__lee_/"><img src="https://img.shields.io/badge/jiho____lee__-F3F5F5?style=social&logo=instagram&logoColor=000000"/></a>
<br/>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/jiholee.py@gmail.com-F3F5F5?style=social&logo=Gmail&logoColor=000000"/></a>
<br/><br/><br/>

### ✏️ Tech Stack
<br/>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=000000"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/JAVA-B32629?style=for-the-badge&logo=OpenJDK&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=F3F5F5"/></a>
<!--<br/>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=Oracle&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=HTML5&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=F3F5F5"/></a>-->
<br/><br/>

### ✏️ BOJ Profile
<br/>

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=dlwlgh0111)](https://solved.ac/dlwlgh0111/)
<a href = "https://solved.ac/profile/dlwlgh0111"><img src="http://mazandi.herokuapp.com/api?handle=dlwlgh0111&theme=(dark)"/>
<br/><br/>

### 📃 Github Stats
<br/>

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=JihoLeec&show_icons=true&theme=dark)

---
</div>

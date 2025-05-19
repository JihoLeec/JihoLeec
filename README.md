# 강의 요약 및 퀴즈 생성기

> <span style="color:gray"><strong>단국대학교 오픈소스SW기초 6분반 15조</strong><br>
조원: 박수빈, 변윤성, 이지호</span>

<br><br>

## 이곳은 "backend" branch입니다.

<br><br>

## 디렉토리 구조
<pre>
OS_15
│  .gitignore
│  README.md
│
└─backend
    │  .env
    │  requirements.txt
    │
    └─app
        │  main.py
        │  __init__.py
        │
        ├─stt
        │      azure_stt.py
        │
        └─summary
                bart_summary.py
</pre>
<br><br>

## 서버 실행 방법

1. 프로젝트 clone
```bash 
git clone https://github.com/iamdbstjd/OS_15
cd OS_15/backend/app
```
2. .env 환경 변수 설정
```bash
# .env에 저희 카톡에 있는 KEY를 추가하셔야 합니다. (""로 안 감싸도 됨)
AZURE_SPEECH_KEY="저희 카톡에 있는 KEY"
```
3. 서버 실행
```bash
uvicorn main:app --reload
```
서버 실행 후 브라우저에서 http://127.0.0.1:8000/docs를 입력하면 API 스펙과 파일 업로드 테스트를 UI로 직접 할 수 있습니다.

파일 업로드 후 응답 데이터(JSON)를 바로 확인할 수 있습니다.

<br><br>

##  현재 구현된 기능

- [✅] 음성 파일 업로드 기능
- [✅] Azure STT 연동 및 텍스트 변환
- [✅] 텍스트 요약 (BART 모델)
- [❌] 퀴즈 자동 생성 (미완)

## 진행 상황 공유
- 음성 파일 업로드 및 텍스트 요약까지 수행
- 그러나 업로드하면 (PXERR_INVALID_HEADER) 에러가 생기는 버그 있음
- 반환값: JSON(transcription, summary, (예정)quiz)

<div align="center">

# ✨ WELCOME ✨
<br/><br/>

###  **I am just a potato🥔**
<br/><br/><br/>

### ✉️ Contact
<br/>
<a href = "https://www.instagram.com/jiho__lee_/"><img src="https://img.shields.io/badge/jiho____lee__-F3F5F5?style=social&logo=instagram&logoColor=000000"/></a>
<br/>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/jiholee.py@gmail.com-F3F5F5?style=social&logo=Gmail&logoColor=000000"/></a>
<br/><br/><br/>

### ✏️ Learning Tech Stack
<br/>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=000000"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/JAVA-000000?style=for-the-badge&logo=OpenJDK&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=F3F5F5"/></a>
<br/>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=Oracle&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=HTML5&logoColor=F3F5F5"/></a>
<a href = "https://github.com/JihoLeec"><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=F3F5F5"/></a>
<br/><br/><br/>

### ✏️ Learning Algorithm
<br/>

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=dlwlgh0111)](https://solved.ac/dlwlgh0111/)
<a href = "https://solved.ac/profile/dlwlgh0111"><img src="http://mazandi.herokuapp.com/api?handle=dlwlgh0111&theme=(dark)"/>
<br/><br/><br/>

### 📃Learning Github
<br/>

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=JihoLeec&show_icons=true&theme=dark)

---
</div>

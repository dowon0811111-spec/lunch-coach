# 프로젝트 개요
공공데이터 cvs를 표 그래프 지도로 보여주는 streamlit 웹앱. 기획서는 CLAUDE.md참고.

## 파일 구조
- lunch_app.py : 매인 앱 (ui+로직)
- .env :ANTHROPIC_API_KEY 보관
- ai_helper.py : claude api룰 사용하는 ask_ai() 함수 정의
- 급식식단정보.csv : 공공데이터 파일
## 규칙
- 항상 PLAN.md 기획서를 기준으로 구현할것
- API 호출은 반드시 ai_helper.py 에서 ask_ai 함수를 불러 쓴다.
- API key는 .env에서 읽고 코드에 직접 쓰지 않는다
- 급식식단정보 .cvs를 UTF-8로 먼저 ,안 되면 cp949로 읽는다.

# langchain-playground

langchain-playground는 **LangChain을 공부하면서 실습한 기록**을 정리한 공간입니다.  
단순히 예제를 실행하는 것에 그치지 않고, 학습한 개념과 실험 결과를 기록하며 점진적으로 확장해 나가고 있습니다.  

기본 예제부터 RAG, Tools/Agents, 프롬프트 엔지니어링까지 단계적으로 실험할 수 있도록 구성했습니다.  


---

## 📂 프로젝트 구조
langchain-playground/
├─ notebooks/ # Jupyter 노트북 모음
│ ├─ 01_quickstart_lcel.ipynb # LangChain 기본 (LCEL)
│ ├─ 02_prompt_template.ipynb # 프롬프트 템플릿 실습
│ ├─ 03_tools_and_agents.ipynb # 툴 / 에이전트
│ └─ 10_rag_faiss_minimal.ipynb # RAG + FAISS
├─ prompts/ # 프롬프트 템플릿 저장
├─ data/ # 샘플 문서/데이터
├─ requirements.txt
├─ .gitignore
└─ README.md


---

## ⚙️ 환경 세팅
bash
# 1. 가상환경 생성
python -m venv .venv
source .venv/bin/activate   # (Windows: .venv\Scripts\activate)

# 2. 의존성 설치
pip install -r requirements.txt

# 3. Jupyter 커널 등록 (처음 한 번만)
python -m ipykernel install --user --name lc-play --display-name "Python (lc-play)"

# 4. API 키 설정
cp .env.example .env   # .env에 OPENAI_API_KEY=your-key-here 입력

## 학습/기록 방식

실습 노트북: 각 노트북은 LangChain 문법/기능을 따라 하면서 직접 실험한 결과를 기록합니다.

메모/주석: 코드 셀에 학습한 개념, 오류 해결 과정, 아이디어를 주석으로 남깁니다.

점진적 확장: 단순 예제 → 기능 조합 → RAG/에이전트 → 응용 프로젝트로 발전시켜 나갑니다.

## 참고 자료

LangChain Docs: https://python.langchain.com

LangChain OpenAI Integration: https://python.langchain.com/docs/integrations/platforms/openai

OpenAI API Docs: https://platform.openai.com/docs/overview

## License
MIT License

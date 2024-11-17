
# Datadog LLM observability + Langchain 맛보기
아래의 필요 작업 진행 후, 노트북을 위에서부터 하나씩 살펴보며 실행시키면 됩니다.
- notebook-langchain 노트북으로 openai 기본과 langchain 기본 + DD LLM Observability
- 이후에는 https://github.com/DataDog/llm-observability 에서 더 자세히 알아보기

## 필요 작업 1
파이선 가상환경 설정이 필요합니다.
```
python -m venv venv
source venv/bin/activate
```

## 필요 작업 2
이후 파이선 패키지 설치가 필요합니다.
```
pip install -r requirements.txt
```

## 필요 작업 3
Root 디렉토리에 .env 파일 생성하고, 아래와 같이 작성합니다.
```
OPENAI_API_KEY="<OPENAI API 키>"
DD_API_KEY="<Datadog API 키>"
DD_SITE="<SITE명, 예: datadoghq.com>"
DD_LLMOBS_AGENTLESS_ENABLED=1
DD_LLMOBS_ML_APP="<ML서비스명>"
```

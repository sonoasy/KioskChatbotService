
<img src="https://github.com/user-attachments/assets/cc76444d-e588-4834-88c9-05f40c14a8c0.PNG" width="600" height="800"/>




# 프로젝트 개요
 
무인 터치스크린 키오스크 미적응자들을 위한 음성인식 AI 점원 API 서비스 

## 주요 기능

- 음성인식 및 음성합성을 통한 대화
- FAQ 질의응답

## 개발 환경 및 기술
- Google Colab
- 음성인식(Speech-To-Text): Google cloud Speech-To-Text
- 음성합성(Text-To-Speech): Pyttsx3
- 의도 파악 모델: Bi-LSTM,Mutinomial Naive Bayes 
- 개체명 인식 모델: Bi-LSTM+CRF
- 답변 생성 모델: Transformer
- 서버: Flask 
## API 시스템 구조도

![systemarchitecture](https://user-images.githubusercontent.com/61787171/142223280-59ecdffa-c486-4239-a324-4163cce4acb3.PNG)



## 파일 디렉토리 구조

```bash
├── README.md
├── STT,TTS
│   ├── .idea
│   │    ├── inspectionProfiles
│   │    │   └── profiles_settings.xml
│   │    ├── .gitignore
│   │    ├── flaskrestful.iml
│   │    ├── misc.xml
│   │    ├── modules.xml
│   │    └── vcs.xml
│   ├── static
│   │   └── styles
│   │       └── index.css
│   │
│   ├── templates
│   │   ├── frontend.html
│   │   └── index.html
│   ├── app.py
│   ├── stttts.ipynb
│   └── transcribe_streaming_mic.py
├── chatbot
│   ├── answer
│   │   └── answer_chatbot.py
│   ├── intent
│   │   ├─ Mutinomial_tfidf.py
│   │   └── lstmNBsfvoting.py
│   ├─ ner
│   │   └─ ner_chatbot.py
│   └── scenario.py
└── dataset
    ├── ChatBotData_answer.csv
    ├─  Intent_bilstm.csv
    ├─  ChatBotData_ner.csv
    ├── dataset.py
    └── nerexcel.py

``` 

## Kiosk Demo
   
#### [안드로이드 ver.](https://github.com/woongjichoi/chatbotdemo)
#### [윈도우 ver.](https://github.com/sonoasy/Kiosk_window/tree/main)

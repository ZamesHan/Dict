# 말하는 영어사전 (Voice English Dictionary)

음성인식으로 검색하는 오프라인 영한사전입니다. 외부 서버 없이 브라우저 안에서 완전히 동작합니다.

## 기능

- **음성 검색**: 마이크 버튼을 누르고 알파벳을 한 글자씩 스펠링하거나 단어를 통째로 말하면, 잠시 멈출 때 자동으로 검색됩니다 (Web Speech API 사용)
- **오프라인 사전**
  - 정성 큐레이션 60단어: 영어 뜻·예문·어원·한국어 번역 포함
  - 확장 사전(A~Z, 약 9.2만 단어): 한국어 뜻 제공 (`edic` 데이터 기반)
- **발음 듣기**: 브라우저 내장 음성 합성(TTS) 사용
- **복습 모드 2종**: 최근 검색한 20개 단어를 새 탭에서 복습
  - 단어 → 뜻 (단어를 보고 뜻을 떠올리기)
  - 뜻 → 단어 (뜻을 보고 단어를 떠올리기)

## 사용 방법

`voice-english-dictionary.html` 파일을 브라우저(Chrome 권장)로 열기만 하면 됩니다. 별도의 서버나 빌드 과정이 필요 없습니다.

GitHub Pages로 배포하려면 이 파일을 `index.html`로 저장한 뒤 저장소의 Pages 설정을 켜면 됩니다.

## 데이터 출처 및 라이선스 주의사항

- 확장 사전 데이터는 [`liks79/edic`](https://github.com/liks79/edic) 저장소의 데이터를 가공한 것입니다.
- 해당 저장소는 원저작자와 라이선스가 명시되어 있지 않은 커뮤니티 데이터입니다. **개인 학습 용도로만 사용을 권장**하며, 공개 배포 시 이 점을 유의해주세요.
- 음성 인식/합성은 브라우저의 Web Speech API를 사용하며, Chrome에서 가장 안정적으로 동작합니다.

## 기술 스택

- 순수 HTML / CSS / JavaScript (프레임워크 없음, 단일 파일)
- Web Speech API (SpeechRecognition, SpeechSynthesis)
- Google Fonts (Newsreader, JetBrains Mono, Noto Sans KR)

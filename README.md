# TQQQ / UPRO App Data + 한글 Dashboard

Private `tqqq-upro-live` 저장소의 GitHub Actions가 `latest.json`을 자동 갱신합니다.

- `latest.json`: Android/iOS/Web 앱이 읽는 최신 전략/계좌/주문 데이터
- `index.html`: 모바일 대응 한글 웹 대시보드

## 중요: 계좌정보 공개범위

현재 live 설정은 사용자의 요청대로 앱에서 수익률/보유/주문을 볼 수 있도록 `latest.json`에 **계좌 계산결과를 포함**합니다.
따라서 이 저장소를 Public으로 만들면 보유수량, 평단, 손익, 주문안도 공개됩니다.

Telegram bot token, chat id, APP_DATA_TOKEN, 원본 `ACCOUNT_CONFIG_ENV` secret 자체는 이 저장소에 기록하지 않습니다.

## 앱 연결

Public 저장소라면 Raw 주소 형식:

`https://raw.githubusercontent.com/OWNER/tqqq-upro-app-data/main/latest.json`

웹 대시보드는 GitHub Pages를 켜면 `index.html`을 그대로 사용할 수 있습니다.

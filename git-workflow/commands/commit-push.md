---
name: commit-push
description: 변경사항을 분석하여 커밋하고 푸시합니다
arguments:
  - name: jira_ticket
    description: 지라 티켓 번호 (예: PI-1234). 전달 시 브랜치명 대신 이 값을 커밋 메시지에 사용
    required: false
---

개발한 변경사항을 분석하여 Conventional Commits 형식의 한국어 커밋 메시지를 자동 생성하고, 커밋 및 푸시를 수행해줘.

$ARGUMENTS가 있으면 해당 값을 지라 티켓 번호로 사용하여 커밋 메시지에 포함해줘. 브랜치명에서 추출하지 말고 인자로 받은 티켓 번호를 우선 사용해.
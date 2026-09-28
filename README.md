# genspark-skills-ko

젠스파크(Genspark) 크레딧을 아끼고, 긴 대화가 끊겨도 작업을 이어갈 수 있게 해 주는 스킬 4개입니다.

A set of 4 Genspark Skills to save credits and continue your work across chats.

[한국어](#한국어) | [English](#english)

---

## 한국어

### 왜 만들었나요?
젠스파크는 대화가 길어질수록 메시지마다 이전 대화를 다시 읽어서 크레딧이 더 듭니다.
그렇다고 새 대화로 옮기면 지금까지 한 작업을 기억하지 못합니다.
이 스킬들은 **작업 내용을 요약해서 넘기고, 새 대화에서 이어서 작업하는 방식**으로 이 문제를 해결합니다.

### 스킬 목록
| 스킬 | 하는 일 | 언제 쓰나 |
|---|---|---|
| [conversation-handoff](skills/conversation-handoff/SKILL.md) | 목표, 파일 구조, 진행 상황, 오류, 규칙을 8개 항목으로 요약 | 대화가 길어졌을 때 |
| [resume-work](skills/resume-work/SKILL.md) | 요약을 읽고 남은 할 일부터 이어서 작업 | 새 대화를 시작할 때 |
| [fix-error](skills/fix-error/SKILL.md) | 원인 한 줄 + 바뀐 코드만 제시, 두 번 실패하면 멈춤 | 에러가 났을 때 |
| [token-saving-coding](skills/token-saving-coding/SKILL.md) | 짧은 답, 바뀐 코드만, 요청 안 한 기능 금지 | 코딩할 때 |

### 사용 흐름
```
resume-work → token-saving-coding → (에러 나면) fix-error → conversation-handoff → 새 대화
```
1. 새 대화에서 `/res`로 **resume-work**를 부르고, 저장해 둔 요약을 붙여넣습니다.
2. 코딩할 때는 `/tok`로 **token-saving-coding**을 씁니다.
3. 에러가 나면 `/fix`로 **fix-error**를 씁니다.
4. 대화가 길어지면 `/con`으로 **conversation-handoff**를 부르고, 요약을 메모나 AI Drive에 저장합니다.

### 설치 방법
**방법 1: 공유 링크로 추가 (가장 쉬움, 로그인 필요)**
- [conversation-handoff](https://www.genspark.ai/skills/share/D-ka4dzPkTzGWHqZHD92lMIroc_Mgmz7)
- [resume-work](https://www.genspark.ai/skills/share/He8tMmMPbXkA_lYT8C1-PKzrFKR4D5bj)
- [fix-error](https://www.genspark.ai/skills/share/PCme_KeVENSiyUnHWXTqGtNvGz4YG2Yz)
- [token-saving-coding](https://www.genspark.ai/skills/share/_Ni18bsRM7kalbNh4DBu-iUS2sMfoR6F)

**방법 2: 파일로 직접 만들기**
1. `skills/` 폴더에서 원하는 스킬의 `SKILL.md` 내용을 복사합니다.
2. [genspark.ai/skills](https://www.genspark.ai/skills)에서 **+ New Skill** → **Create for myself**를 누릅니다.
3. 복사한 내용을 붙여넣고 "이걸로 스킬 만들어줘"라고 보냅니다.

> 아이폰은 사파리에서 **데스크탑 웹사이트 요청**을 켜면 Skills 메뉴가 보입니다.
> 입력창에서는 영어 앞글자(`/con`, `/res`, `/fix`, `/tok`)로 검색하세요.

### 크레딧 아끼는 팁
- 요청은 한 번에 구체적으로 적기 (다시 생성할 때마다 크레딧이 처음과 똑같이 듭니다)
- 한 대화에서는 한 가지 일만 하기
- 에러는 코드 전체 말고 에러 메시지와 관련된 부분만 보내기
- 작은 수정은 직접 고치기

---

## English

### Why?
In Genspark, long chats cost more credits because every message re-processes the full context.
But starting a new chat loses everything you've done.
These Skills solve this by **summarizing your work and continuing it in a new chat**.

### Skills
| Skill | What it does | When to use |
|---|---|---|
| [conversation-handoff](skills/conversation-handoff/SKILL.md) | Summarizes goal, files, progress, errors, and rules in 8 fixed sections | When the chat gets long |
| [resume-work](skills/resume-work/SKILL.md) | Reads the summary and continues from the next task | When starting a new chat |
| [fix-error](skills/fix-error/SKILL.md) | One-line cause + only changed code, stops after 2 failed attempts | When you hit an error |
| [token-saving-coding](skills/token-saving-coding/SKILL.md) | Short answers, only code changes, no unrequested features | While coding |

### Workflow
```
resume-work → token-saving-coding → (on error) fix-error → conversation-handoff → new chat
```

### Installation
**Option 1: Share links** (Genspark login required): see the links in the Korean section above.

**Option 2: Create from file**
1. Copy the contents of a `SKILL.md` file in the `skills/` folder.
2. Go to [genspark.ai/skills](https://www.genspark.ai/skills) → **+ New Skill** → **Create for myself**.
3. Paste it and ask Genspark to create the Skill.

> The Skill prompts are written in Korean. You can ask Genspark to translate them before creating the Skill.

---

## Author
Made by [Yune](https://github.com/buriburiyj)

If these Skills help you, please leave a ⭐!

# genspark-skills-ko

Practical skills for Genspark and other AI coding assistants, written in Korean with English names and examples where useful.

Genspark 및 AI 코딩 에이전트에서 바로 활용할 수 있는 실용 스킬 모음입니다. 대화 맥락을 이어가고, 오류를 안전하게 수정하고, 코딩 답변을 간결하게 만드는 데 초점을 둡니다.

## Skills

| Skill | What it does |
| --- | --- |
| [`conversation-handoff`](skills/conversation-handoff/SKILL.md) | Creates a structured handoff summary for continuing work in a new chat. |
| [`fix-error`](skills/fix-error/SKILL.md) | Diagnoses errors, suggests minimal changes, and avoids unverified fixes. |
| [`resume-work`](skills/resume-work/SKILL.md) | Resumes a project from a handoff summary and starts with the next open task. |
| [`token-saving-coding`](skills/token-saving-coding/SKILL.md) | Keeps coding replies concise and limited to requested changes. |

## Use a skill

1. Open the skill's `SKILL.md` and check its trigger conditions.
2. Add the skill folder to an agent that supports the Agent Skills format, or paste the instructions into your agent's skill configuration.
3. Ask the agent for a task that matches the skill.

Each skill is self-contained in `skills/<skill-name>/SKILL.md`; no package installation is required.

## Contributing

Keep each skill focused on one job. Update its frontmatter description when its trigger or behavior changes, and include a concise example for behavior that may be ambiguous.

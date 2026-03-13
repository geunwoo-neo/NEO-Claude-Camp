# NEO AI Native Camp (Windows 버전)

> 7일 후, 당신의 업무 방식은 영구적으로 바뀐다.
> 비개발자를 위한 Claude Code 7일 집중 캠프.

---

## 시작 전에 — 이 문서를 읽는 분께

코딩을 몰라도 됩니다. 개발자가 아니어도 됩니다.
이 가이드는 **컴퓨터를 처음 세팅하는 것처럼** 하나씩 따라 하도록 만들어졌습니다.

막히는 부분이 있으면 그냥 Claude에게 물어보세요.

---

## 준비물 체크리스트

캠프를 시작하기 전에 아래 4가지를 설치해야 합니다.
순서대로 하나씩 진행하세요.

- [ ] Node.js 설치
- [ ] Git 설치
- [ ] Python 설치
- [ ] Claude Code 설치

---

## 1단계: Node.js 설치

**Node.js가 뭔가요?**
스킬 설치 명령어를 실행하기 위해 필요한 도구입니다. 한 번만 설치하면 됩니다.

**설치 방법:**

1. 브라우저에서 [https://nodejs.org](https://nodejs.org) 를 엽니다
2. 초록색 버튼 **"LTS"** 를 클릭해서 파일을 내려받습니다
   - LTS = 가장 안정적인 버전이라는 뜻입니다
3. 내려받은 파일(`.msi`)을 더블클릭해서 실행합니다
4. 설치 창이 뜨면 **"Next"를 계속 클릭**해서 기본 설정으로 설치합니다

**설치 확인:**

1. 키보드에서 `Windows 키 + R` 을 누릅니다
2. `powershell` 을 입력하고 Enter
3. 검은 창(PowerShell)이 열리면 아래를 입력하고 Enter:

```
node -v
```

`v20.xx.x` 처럼 숫자가 나오면 성공입니다.

---

## 2단계: Git 설치

**Git이 뭔가요?**
내가 만든 파일과 작업 내역을 버전별로 저장해두는 도구입니다.
"어제 버전으로 되돌리고 싶다"는 상황에 유용합니다.

**설치 방법:**

1. 브라우저에서 [https://git-scm.com](https://git-scm.com) 을 엽니다
2. **"Download for Windows"** 버튼을 클릭합니다
3. 내려받은 파일을 더블클릭해서 실행합니다
4. 설치 창에서 **"Next"를 계속 클릭**해서 기본 설정으로 설치합니다

**설치 확인:**

PowerShell을 열고 아래를 입력하고 Enter:

```
git --version
```

`git version 2.xx.x` 처럼 나오면 성공입니다.

---

## 3단계: Python 설치

**Python이 뭔가요?**
캠프 실습에서 Claude가 데이터를 분석하거나 자동화 작업을 할 때 사용하는 도구입니다.

**설치 방법:**

1. 브라우저에서 [https://www.python.org/downloads](https://www.python.org/downloads) 를 엽니다
2. **"Download Python 3.xx.x"** 버튼을 클릭합니다
3. 내려받은 파일을 더블클릭해서 실행합니다
4. 설치 창 맨 아래에 **"Add Python to PATH"** 라는 체크박스가 있습니다
   - **반드시 체크하고** "Install Now"를 클릭하세요
   - 이걸 안 하면 나중에 Python을 인식 못 합니다

**설치 확인:**

PowerShell을 열고 아래를 입력하고 Enter:

```
python --version
```

`Python 3.xx.x` 처럼 나오면 성공입니다.

---

## 4단계: Claude Code 설치

**Claude Code가 뭔가요?**
이 캠프의 핵심 도구입니다. Claude AI를 내 컴퓨터에서 직접 실행할 수 있게 해줍니다.

**필요한 것:**
- Claude 계정 (Pro, Max, Teams, Enterprise 중 하나)
- 인터넷 연결

**설치 방법:**

모르면 Claude한테 물어보세요. [https://claude.ai](https://claude.ai) 에 접속해서 이렇게 입력하면 됩니다:

```
Claude Code 윈도우에 설치하는 방법 알려줘
```

Claude가 단계별로 안내해줍니다.

<details>
<summary>직접 설치하려면 (참고용)</summary>

**PowerShell에서 실행:**

```powershell
irm https://claude.ai/install.ps1 | iex
```

**명령 프롬프트(CMD)에서 실행:**

```cmd
curl -fsSL https://claude.ai/install.cmd -o install.cmd && install.cmd && del install.cmd
```

</details>

**설치 확인:**

PowerShell을 열고 아래를 입력하고 Enter:

```
claude
```

Claude가 인사말을 보여주면 성공입니다.
로그인 안내가 나오면 그대로 따라 진행하세요.

---

## Step 1: 캠프 스킬 설치

PowerShell을 열고 아래 명령어를 입력하고 Enter:

```
npx skills add ai-native-camp/camp-2 --agent claude-code --yes
```

설치가 완료되면 Claude Code에서 아래 명령어로 Day 1을 시작하세요:

```
/day1-onboarding
```

---

## 커리큘럼

| Day | 명령어 | 배우는 것 |
|-----|--------|-----------|
| 1 | `/day1-onboarding` | 7개 핵심 기능 (Memory, Skill, MCP, Subagent, Agent Teams, Hook, Plugin) |
| 2 | `/day2-mcp-and-context-sync` | MCP 딥다이브 + Context Sync 스킬 구축 |
| 3 | `/day3-clarify` | Clarify 플러그인 활용 + 나만의 스킬 만들기 + Plugin 심화 + 엑셀 데이터 전처리 실습 |
| 4 | `/day4-wrap-and-analyze` | Wrap & Analyze: 세션 분석 스킬 구축 + 콘텐츠 소화 체험 |

---

## 막히면?

> Claude Code 안에서 언제든지 이렇게 물어보세요:
>
> "지금 뭘 해야 해?"
> "이게 무슨 뜻이야?"
> "오류가 났어, 어떻게 해?"

Claude가 바로 도와줍니다.

---

## 캠프가 끝나면

수료가 아니라 시작이다.
Claude Code라는 불을 다루는 신인류 커뮤니티의 일원이 된다.

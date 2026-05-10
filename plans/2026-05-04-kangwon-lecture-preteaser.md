# 세션 전에 읽고 오면 더 재밌어요
**2026. 05. 12 | 배필주 / Kurly, Staff Engineer**

---

개발자가 AI에게 이렇게 말했어요.

*"테스트 통과시켜줘"*

AI는 열심히 했습니다. 테스트를 통과 못 하자 테스트 코드를 삭제했고, 그래도 안 되자 CI에서 해당 항목을 아예 제외해버렸어요. 결과는 CI 녹색, 보고는 "All tests pass".

거짓말한 게 아니에요. AI는 시킨 걸 했을 뿐입니다.

이 얘기로 세션이 시작돼요. 미리 알면 더 재밌어질 것들 몇 가지만 공유할게요.

---

## 강연자가 누구예요

안드로이드 개발 경력 13년차예요. Coupang, NAVER Z(ZEPETO)를 거쳐 현재 Kurly에서 Staff Engineer로 일하고 있어요. GDG Korea Android 오거나이저로도 활동 중이고요.

Jetpack Compose 마이그레이션, 앱 성능 최적화, AI 개발 워크플로우를 주로 다루고 있어요. 발표도 꾸준히 하고 있습니다.

---

## Goodhart's Law — 세션 내내 등장하는 개념

> "측정 기준이 목표가 되는 순간, 더 이상 좋은 측정 기준이 아니다."

뭔가 딱딱하게 들리는데, 사실 우리 주변에 흔한 얘기예요.

선생님이 출석에 점수를 주면 어떻게 되죠? 학생들은 출석만 합니다. 목표는 공부였는데, 측정 기준인 출석만 최적화하는 거예요. AI도 똑같이 작동해요. "테스트 통과시켜줘"가 목표가 되면, 테스트를 지우는 게 오히려 합리적인 선택이 됩니다.

> 📖 쉬운 설명: [What is Goodhart's Law? — Splunk](https://www.splunk.com/en_us/blog/learn/goodharts-law.html)  
> 📖 조금 더 깊게: [Goodhart's Law: Why Everything Eventually Goes Wrong — Medium](https://machine-learning-made-simple.medium.com/goodharts-law-why-everything-eventually-goes-wrong-44e66ca0c6bd)

그럼 AI한테 원하는 걸 얻으려면 어떻게 말해야 할까요?

---

## AI는 텍스트를 어떻게 볼까요

2024년 초까지 ChatGPT(GPT-4 기준)한테 "strawberry에 r이 몇 개야?" 물어보면 틀렸어요. 지금은 고쳐졌지만, 멍청해서가 아니라 구조적인 이유가 있었고 그 구조는 지금도 그대로예요.

우리는 strawberry를 s-t-r-a-w-b-e-r-r-y, 문자 하나하나로 읽는데 AI는 이걸 `[49323]` 같은 정수 덩어리로 봐요. 어떤 문자로 이루어졌는지는 관심이 없는 거죠.

세션 중간에 이 얘기가 나오는데, 알고 들으면 훨씬 빠르게 이해할 수 있어요.

> 📖 strawberry 논란 원문: [Why ChatGPT gets strawberry wrong](https://www.distractify.com/p/chatgpt-how-many-rs-in-strawberry)  
> 🔧 직접 해보기: [OpenAI Tokenizer](https://platform.openai.com/tokenizer) — strawberry 입력해보면 바로 보여요

---

## Andrej Karpathy가 누구예요

Tesla 자율주행 AI팀장 출신, OpenAI 공동창업자예요. 개발자들 사이에선 유튜브 AI 강의로 꽤 유명한 분이에요.

2025년에 이 분이 **"vibe coding"** 이란 말을 만들었어요. 코드를 직접 짜지 않고 AI한테 느낌으로 전달해서 만드는 방식인데, 세션에서 이 분 말이 인용돼요. 미리 알면 맥락이 훨씬 잘 잡힐 거예요.

> 📖 vibe coding 원문 트윗: [Andrej Karpathy on X](https://x.com/karpathy/status/1886192184808149383)  
> 🎥 유튜브 채널: [Andrej Karpathy](https://www.youtube.com/@AndrejKarpathy)

vibe coding, 현업에서 진짜 되는 얘기인가요?

---

## Jetpack Compose, 선언형이 뭐예요

Android 개발 방식이 두 가지가 있어요.

기존 XML 방식은 "버튼을 여기 놓고, 크기는 이만큼, 색은 이렇게" 처럼 어떻게 만들지를 하나하나 명령해요. Compose는 달라요. "이런 버튼이 있으면 좋겠어"처럼 뭘 보여줄지만 선언하면 알아서 그려줘요. 이걸 선언형(Declarative)이라고 해요.

세션에서 이 방식이 AI와 일하는 방식이랑 똑같다는 얘기가 나와요. 직접 써본 적 없어도 괜찮아요. 개념만 알고 오면 그 순간 훨씬 재밌게 들릴 거예요.

> 📖 공식 소개: [Jetpack Compose — Android Developers](https://developer.android.com/compose)

처음 배울 때 AI랑 같이 시작해도 괜찮을까요?

---

**5월 12일, 이 질문 하나 들고 와주세요.**

> AI가 모바일 개발자를 대체할 수 있을까요?

읽다가 궁금한 것 생기면 세션 전에 미리 보내주세요.

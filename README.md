# arc-hack

Build on Arc 해커톤을 위한 **h402** 제출 자료입니다. h402는 결제 자체를 다시
만들지 않습니다. Circle Agent Stack과 x402를 통해 실행되는 에이전트 결제 위에,
어떤 제공자를 왜 선택했고 실제 결과가 어땠는지 증명하는 의사결정·신뢰 레이어를
구축합니다.

## Included

- `index.html` — 영문/국문 전환이 가능한 팀·프로젝트 소개 페이지입니다. Arc에서의
  h402 전략, 팀 역량, 기존 제품 검증과 4주 MVP 범위를 담고 있습니다.
- `deck.html` — Build on Arc 제출용 11페이지 발표 자료의 웹 원본입니다.
- `deck.pdf` — `deck.html`에서 생성하고 렌더링 검수한 제출용 PDF입니다.
- `assets/` — 팀 프로필과 기존 제품 이미지입니다.

## Arc strategy

1. Agent Wallet의 USDC 예산 안에서 가격·품질·지연시간·가용성을 비교해 제공자를
   선택합니다.
2. Circle Nanopayments/x402로 소액 결제를 실행하고, Arc에 선택 근거와 결과 해시가
   담긴 서명 영수증을 남깁니다.
3. 검증된 성과는 ERC-8004 평판으로 축적하고, 장기·고가 작업은 ERC-8183 에스크로
   흐름으로 확장합니다.

## Local preview

```bash
python3 -m http.server 8747
# → http://127.0.0.1:8747/
```

## Deploy on Vercel

1. Vercel → Add New → Project → Import `realproject7/arc-hack`
2. Framework Preset: **Other** · build command 없음 · Root Directory: `/`
3. Deploy. `index.html`은 `/`에서 제공됩니다.

심사자가 로그인 없이 열 수 있도록 Deployment Protection / Vercel Authentication은
꺼 두어야 합니다.

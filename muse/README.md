# Muse招待コード（DKR2BF）

Museの招待コードを実際に使ってもらうための発信。Museのエージェント（マルローネ）が作ったガイドと投稿データを受け取り、Xは常時接続PCの自動投稿で出す（2026-11-02）。

- 戦略：[04_二番煎じ戦略.md](04_二番煎じ戦略.md)（「気になってたけど、まだ始めていない人」向け。煽らない）
- 受け渡し仕様：[X自動投稿_受け渡し仕様.md](X自動投稿_受け渡し仕様.md)
- 投稿データと仕組み：`ai_yorimichi_master` の `automation/publisher/campaigns/muse-invite/`（posts.json は受け取ったまま）
- 結果（計測シートと同じ列）：`ai_yorimichi_master` の `automation/publisher/state/campaign-muse-invite.csv`（読むだけ）

## 編集長の決定（2026-11-02）

- Xの投稿は、部員の連載・4コマとは声が違う（編集長本人の発信）ので、末尾に `#編集長の独り言` を付ける。受け渡し仕様の「ハッシュタグは原則なし」より優先する
- Threadsはマルローネが担当（この仕組みの対象外）

## 止めるとき

`ai_yorimichi_master` の `automation/publisher/campaigns/muse-invite/campaign.json` の `stop` を `true` にし、`stop_reason` を書く。Typefullyに入った予約は自動では消えないので、Typefullyで消す。

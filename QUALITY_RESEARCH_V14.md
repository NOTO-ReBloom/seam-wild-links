# MASTERPIECE DIVE V14 — 品質向上の研究と実装方針

## 参照した考え方

### 1. 物語とレベルデザインを分離しない
GDCの「A Narrative Approach to Level Design」「Level Design in a Day」では、物語を台詞だけで伝えるのではなく、空間、進行、プレイヤーの選択と結び付ける考え方が扱われています。

V14では、物語幕は会話と環境の痕跡を中心に残し、別枠の試練では同じ能力を異なる目的へ転用しました。これにより、世界設定を壊さずに遊びの幅を増やしています。

### 2. 得意・不得意が違う二人を同時に参加させる
『New Super Mario Bros. Wii』の開発者インタビューでは、得意な人と苦手な人が一緒に遊ぶこと、復帰や待ち時間を減らすことが重要な課題として語られています。

V14では、即失敗ではなく救助を維持しながら、試練ごとに役割を明確にしました。

- リレー：担当を交互に切り替える
- 護送：二人の距離そのものが進行条件
- 二重奏：別々の地点で同時操作
- ボス：固定と描画を連続して使う
- 追跡：移動と停止のタイミングを共有する

### 3. 機能数ではなく「遊びとして成立する完成度」を確認する
Supergiant Gamesは、ゲームが全体の体験を表現し、実際に遊ぶ価値がある状態でなければ完成段階とは呼べないという趣旨を説明しています。

V14では、単に試練カードを追加するだけでなく、各試練について専用の進行条件、HUD、失敗、スコア、ランク、保存、描画、効果音、ゴール解放まで実装しました。

## 今回の品質判断基準

- 物語幕と特殊試練で、プレイの心理が明確に異なる
- 二人とも操作する必要がある
- 役割が一方的に固定されず、相手の行動を読む必要がある
- 現在の目的と進捗をHUDだけで確認できる
- 成功、失敗、部分成功が音と画面変化で分かる
- 失敗後に再挑戦の理由が分かる
- 既存の名画背景と能力を使い回すだけでなく、別の遊びへ変換する

## 参照元
- GDC Vault: A Narrative Approach to Level Design
- GDC Vault: Level Design in a Day: Best Practices from the Best in the Business
- Nintendo / Iwata Asks: New Super Mario Bros. Wii Vol. 3
- Supergiant Games: Transistor development update / alpha definition
- Masahiro Sakurai on Creating Games official channel

# Life Value Continuity（人生の価値の継続）

> **人を変えずに、構造を変える。**

Status: 思想 v1.0 / AI 仕様 v0.2–v0.3（概念仕様） · License: [CC BY 4.0](LICENSE)

**English summary** — Life Value Continuity (LVC) is the personal edition of [Value Continuity](https://github.com/value-continuity/value-continuity). Its highest value is *keeping the state in which you can re-choose your own values*, and its design goal is *being able to decide for yourself where to optimize and where not to*. This repository holds two clearly separated layers: the **principles** (what LVC is, independent of any technology) and the **AI specifications** derived backward from those principles (how a personal AI must behave so that it does not override the person). The documents are written in Japanese.

![人生の価値の継続（LVC）の全体像](principles/images/lvc.png)

---

## 二つの層

このリポジトリは、性質の異なる二つのものを分けて置いている。

| 層 | ディレクトリ | 何を扱うか | 状態 |
|---|---|---|---|
| **思想** | [principles/](principles/) | LVC そのもの。価値・目的・手段、本人の主権、原則。AI の有無に依存しない | v1.0 |
| **AI 仕様** | [ai-spec/](ai-spec/) | 思想から逆算した、パーソナル AI が満たすべき仕様。過干渉しない境界と、本人の文脈の扱い | 概念仕様 v0.2–v0.3 |

### 依存の向き

```
Value Continuity（上位原則）
  └─ Life Value Continuity（思想）        … principles/
       └─ LVC の AI 仕様（逆算した仕様）   … ai-spec/
```

- 依存は**一方向**である。AI 仕様は思想を参照するが、思想は AI 仕様を参照しない。
- AI 仕様が変わっても、思想は変わらない。思想と AI 仕様の表現が食い違う場合は、**思想を優先**する。
- AI 仕様は、思想を実現する方法の一つにすぎない。AI を使わずに LVC を実践することもできる。

---

## 文書構成

### 思想（[principles/](principles/)）

| 文書 | 内容 |
|---|---|
| [life-value-continuity.md](principles/life-value-continuity.md) | LVC の定義と原則。**思想の正本** |

### AI 仕様（[ai-spec/](ai-spec/)）

| 文書 | 内容 |
|---|---|
| [common-principles.md](ai-spec/common-principles.md) | 三つの仕様の責務分担、実効権限の「交差」、技術的強制、統合テストケース |
| [ib-intervention-boundary.md](ai-spec/ib-intervention-boundary.md) | IB：介入境界仕様。AI に何をさせるか（介入レベル・起動条件・停止・委譲） |
| [lcs-life-context-store.md](ai-spec/lcs-life-context-store.md) | LCS：ライフコンテキストストア。何を保持し、何を見せるか（層・開示段階・保管） |
| [CCP ライフプロファイル](https://github.com/VCDesign-org/continuity-claim-protocol/blob/main/docs/ja/life-profile.md) | 誰と、どんな条件で接続するか（相手・目的・保持期間）。[CCP（Continuity Claim Protocol）](https://github.com/VCDesign-org/continuity-claim-protocol) を個人の文脈に適用するプロファイルで、CCP リポジトリで管理する |

---

## 読む順番

1. まず [principles/life-value-continuity.md](principles/life-value-continuity.md) で考え方を読む。
2. AI との関わり方に関心があれば、[ai-spec/](ai-spec/) の共通原則 → IB → LCS の順に読む。

---

## 関連

| 層 | 内容 |
|---|---|
| [Value Continuity](https://github.com/value-continuity/value-continuity) | 価値と判断を時間の中でどう扱うかという上位思想 |
| [VCDesign](https://github.com/VCDesign-org/vcdesign) | 業務において、価値・判断・責任を継続させる設計 |
| [CCP](https://github.com/VCDesign-org/continuity-claim-protocol) | AI どうしが境界と責任を宣言して接続を始めるための最小ハンドシェイクプロトコル。AI 仕様の接続条件で参照する |
| Life Value Continuity（本リポジトリ） | 個人において、価値を選び直せる状態を継続させる設計 |

## License

[CC BY 4.0](LICENSE)

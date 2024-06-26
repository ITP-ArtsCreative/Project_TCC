﻿# Ladder

#### **Namespace**: Unity.TinyCharacterController.Modifier
---

## 概要:
`Ladder` コンポーネントは、はしごの設定を表し、`MoveLadderControl` での移動を制御するために使用されます。はしごに登ったり、降りたりする際の挙動を定義し、キャラクターの移動を自然に見せるためのパラメータを提供します。

## 機能と操作:
- **はしごの位置とサイズの定義**: はしごの開始点、終了点、ステップ数を設定します。
- **キャラクターのオフセット**: キャラクターがはしごを使う際の位置オフセットを設定します。
- **はしごへのアクセスポイント**: はしごの上部と下部にアクセスするための開始位置を定義します。

## プロパティ
| 名前 | 説明 |
|------|-------------|
| `_startOffset` | はしごの開始点のオフセット。 |
| `_characterOffset` | キャラクターのオフセット。 |
| `_length` | はしごの高さ。 |
| `_stepCount` | ステップ数。 |
| `_topStartPosition` | はしごの上部にアクセスするための開始位置。 |
| `_bottomStartPosition` | はしごの下部にアクセスするための開始位置。 |

## メソッド
| 名前 | 機能 |
|------|----------|
|  `Vector3` CloseStepPosition( `Vector3 position` )  | 指定された位置に最も近いステップの座標を取得します。 |
|  `Vector3` CloseStepPosition( `float point` )  | 指定された移動距離に最も近いステップの座標を取得します。 |
|  `Vector3` ClosePosition( `Vector3 position` )  | 指定された位置に最も近いはしご上の座標を取得します。 |
|  `float` CloseStepPoint( `float point` )  | 指定された移動距離に最も近いステップの移動距離を取得します。 |
|  `float` ClosePoint( `Vector3 position` )  | 指定された位置に最も近いはしご上の移動距離を取得します。 |

---
## その他の注意事項
- `Ladder` ははしごに関連するキャラクターの動作を定義するために使用されます。キャラクターがはしごを登る際の自然な動きや、はしごの各ステップに合わせた動作を実現するための重要なパラメータを提供します。
- はしごの各ステップの位置や、はしごにアクセスするための上部・下部の開始位置など、詳細な設定を行うことで、ゲーム内でのはしごの使用感を向上させることができます。

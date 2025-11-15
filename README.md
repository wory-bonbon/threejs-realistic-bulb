# 照明シミュレーター 💡

WebベースのインタラクティブなLighting Simulator。Three.jsを使用した3D電球シミュレーション。

![Demo](images/demo.gif)

## デモ

https://wory-bonbon.github.io/lighting-simulator/

## 機能

### 基本機能
- 電球数調整（1-10個）
- 配置パターン（単一/円形/グリッド）
- カラー変更（フルカラーピッカー）
- 照明強度・範囲調整
- 品質モード切替（高品質/軽量）

### エフェクト機能
- **プリセット**：温かい電球色/クールな白/ムーディー/パーティー
- **点滅機能**：一定/ランダム/パルス（速度調整可能）
- **ミラーボール効果**：60光点、360度全方向照射

### バリエーション
- **index.html**：フルフィーチャー版（推奨）
- **webxr-bulb.html**：Meta Quest対応WebXR版
- **shader-bulb.html**：シェーダー電球単体

## 使い方

1. HTMLファイルをブラウザで開く
2. 右側のコントロールパネルで調整
3. プリセットボタンで素早く雰囲気変更

## 技術仕様

- **Three.js r128**：3Dレンダリング
- **Tailwind CSS**：UI（CDN）
- **UnrealBloomPass**：ポストプロセッシング
- **カスタムGLSLシェーダー**：リアルなガラス表現

## パフォーマンス

- 60fps維持（電球10個＋ミラーボール60光点）
- デバイス最適化対応
- Quest向け軽量モード自動切替

## 動作環境

- モダンブラウザ（Chrome/Edge/Firefox推奨）
- WebGL対応デバイス
- Meta Quest 2/3（webxr-bulb.htmlのみ）

## ライセンス

MIT License

## 開発者

Wory Bonbon - [@wory-bonbon](https://github.com/wory-bonbon)
```

#### 2-3. `LICENSE` 作成

MITライセンス全文（Cursorで新規ファイル作成 → `LICENSE`）：
```
MIT License

Copyright (c) 2025 Wory Bonbon

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
# THE UME DIGEST（UMEポートフォリオページ）

UME（Naoki Umegatani、AI Urbex Artist）のポートフォリオページ「THE UME DIGEST」のソースバックアップ。
本体はClaude Artifactとして公開・運用中で、このフォルダは**ソースのローカル/GitHubバックアップ**。

作成日: 2026-11-03

---

## 1. 本番の場所

- **公開URL（本番）**: https://claude.ai/artifact/JmQGexMSdtqhyryQRSn2NH
- 編集は毎回 Claude Code（Artifactツール）経由で上記URLへ直接publishして行う。このフォルダの`index.html`は**publish後に手動でバックアップコピーしたもの**であり、このフォルダを編集してもライブページには反映されない。
- 比較・検証用のサンプルページ（別Artifact）: https://claude.ai/artifact/Qez16bUGWt91CEBxERhdYY （デザイン案の比較検討用、本番ではない）

## 2. 見落とし注意：画像は単体では表示されない

`index.html`内の画像は全て `/_blob/<id>` 形式のパスで、Claude Artifactのアセットストレージを指す内部URL。
**このフォルダの`index.html`をブラウザで直接開いても画像は表示されない**（Artifact環境外では解決しないパスのため）。
あくまでHTML/CSS/JS側のソースコードを保全するためのバックアップであり、単体で動くスタンドアロン版ではない。

## 3. 更新フロー

1. Claude Artifact（本番URL）側でEdit→publishして実際のページを更新
2. publish後、最新のソースをこのフォルダの`index.html`に上書きコピー（バックアップ目的）
3. 変更内容が大きい場合はgitコミット

## 4. 構成

```
035_P_ume-digest/
└── index.html   # THE UME DIGEST 本番Artifactのソースバックアップ（画像は/_blob/参照のため単体表示不可）
```

## 5. 関連

- サンプル/比較用Artifact: https://claude.ai/artifact/Qez16bUGWt91CEBxERhdYY
- 展示実績の出典: `021_beyond-decay-exhibition`、`027_pop-alive-exhibition`、`project_beyond_decay.md`
- グッズ・物販の既存ショップ: `031_ume-studio-ec-setup`（UME STUDIO／BASE）

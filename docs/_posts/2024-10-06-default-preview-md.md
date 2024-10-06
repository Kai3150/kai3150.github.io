---
layout: post
title:  "【VScode】 .mdファイルをデフォルトでpreview表示する方法"
date:   2024-10-06 06:26:07 +0000
categories: vscode
---

[こちら][参照]の記事でも紹介されているように私がマークダウンをVScodeで開く時，99.999%はReadOnlyです．

そこでVScodeでデフォルトでmdファイルをプレビューモードで開く設定について紹介します．


設定は簡単 `workbench.editorAssociations`の項目を以下のように設定するだけ以上！

<img width="576" alt="image" src="https://github.com/user-attachments/assets/5bd48671-fd0f-4b37-9ed6-8ddcf70e0ce4">



一応setting.jsonでも設定ができるらしいです．
```json:setting.json
{
    // your other settings ...
    "workbench.editorAssociations": [
        {
            "*.md": "vscode.markdown.preview.editor"
        }
    ],
}
```




参照： https://stackoverflow.com/questions/60155443/vscode-preview-markdown-by-default

[参照]:https://stackoverflow.com/questions/60155443/vscode-preview-markdown-by-default

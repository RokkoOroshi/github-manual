# Git チートシート

## 基本的な流れ
```
clone → switch -c → 編集 → add → commit → push → Pull Request
```

---

## コマンド一覧

### セットアップ
| コマンド | 説明 |
|---|---|
| `git clone [URL]` | リモートリポジトリをローカルにコピー |
| `cd [リポジトリ名]` | クローンしたフォルダに移動 |

### ブランチ
| コマンド | 説明 |
|---|---|
| `git branch` | ブランチ一覧を表示 |
| `git switch [ブランチ名]` | ブランチを切り替え |
| `git switch -c [ブランチ名]` | ブランチを作成して切り替え |

### 変更の記録
| コマンド | 説明 |
|---|---|
| `git status` | 変更状態を確認 |
| `git add [ファイル名]` | 特定のファイルをステージング |
| `git add .` | すべての変更をステージング |
| `git commit -m "メッセージ"` | 変更を記録 |

### リモートとのやり取り
| コマンド | 説明 |
|---|---|
| `git push -u origin [ブランチ名]` | 初回push |
| `git push` | 2回目以降のpush |
| `git pull` | リモートの変更をローカルに取得 |

### 確認
| コマンド | 説明 |
|---|---|
| `git log --oneline` | コミット履歴を簡潔に表示 |
| `git diff` | 未ステージの変更内容を表示 |

---

## よくある作業の流れ

### 新しい作業を始めるとき
```
git switch main          # mainに戻る
git pull                 # 最新状態に更新
git switch -c [作業名]   # 作業ブランチを作成
```

### 変更をpushするとき
```
git status               # 変更ファイルを確認
git add .
git commit -m "メッセージ"
git push -u origin [ブランチ名]   # 初回
git push                           # 2回目以降
```

---

## リポジトリ一覧

### Wimm
| リポジトリ | URL |
|---|---|
| 本体 | https://github.com/yuki-asagoe/Wimm |
| Machine Example `オブジェクト実装の具体例` | https://github.com/yuki-asagoe/Wimm_Machine_Example |

### ロボット
| リポジトリ | URL |
|---|---|
| アルゴ | https://github.com/yuki-asagoe/Robot-Algo |
| コーカサス | https://github.com/yuki-asagoe/Robot-Caucasus |
| スカウト | https://github.com/yuki-asagoe/Robot-Scout |
| アレイニー | https://github.com/yuki-asagoe/Robot-Araneae |
| ラーテル | https://github.com/KakeruDaian/Robot-Ratel |

---

## organization リポジトリのURL
部のorganizationアカウント: https://github.com/RokkoOroshi

リポジトリのURLは以下の形式になる。
```
https://github.com/RokkoOroshi/[リポジトリ名]
```

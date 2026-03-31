# @fandhe-ai/shared-config-vitest

Vitest（ユニットテスト）の共有設定。

## エクスポート

| パス | 説明 |
|------|------|
| `@fandhe-ai/shared-config-vitest/base` | happy-dom 環境、V8 カバレッジ、blob レポーターの共有設定 |

## 使用方法

`vitest.config.ts` で `sharedConfig` を import して使用する:

```ts
import { sharedConfig } from "@fandhe-ai/shared-config-vitest/base";
import { defineConfig, mergeConfig } from "vitest/config";

export default mergeConfig(sharedConfig, defineConfig({}));
```

## 開発

### セットアップ

```bash
pnpm install
```

### コミット規約

[Conventional Commits](https://www.conventionalcommits.org/ja/) を採用。
[commitlint](https://commitlint.js.org/) + [lefthook](https://github.com/evilmartians/lefthook) により自動検証。

```
<type>: <description>

# 例
feat: 新しいルールを追加
fix: 設定の不具合を修正
chore: 依存関係を更新
```

## ライセンス

Copyright © Fandhe Inc.

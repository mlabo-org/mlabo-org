# mlabo-org Profile Repository Constitution

このファイルは `mlabo-org/mlabo-org` profile repository 配下における Codex と Claude Code が共用する局所 `AGENTS.md` であり、このprojectの正本、編集、公開条件を定義する SSOT である。
本書は助言集ではなく、project identity、source boundary、GitHub integration、検証条件を拘束する運用契約として扱う。
上位の `AGENTS.md`、システム指示、開発者指示、ユーザーの明示要求と競合する場合は、作業中のホストエージェント（Codex または Claude Code）の優先順位規則に従う。Claude Code はこのファイルを同じフォルダの `CLAUDE.md` から `@AGENTS.md` で読み込む。

## Purpose And Source Boundary

- このrepositoryはGitHub account `mlabo-org` のpublic profile metadataそのものを所有する独立projectである。
- このlocal directoryを編集用working tree、`https://github.com/mlabo-org/mlabo-org.git`を同一Git履歴の`origin`、GitHub `main`を共有履歴の基準とする。
- 一般projectの公開copy、release staging、plugin/skill source、runtime dataをこのrepositoryへ混ぜない。
- `PROJECT_IDENTITY_ISOLATION`を継承し、他repositoryのsource、commit、branch、tag、issue、pull requestを取り込まない。

## Editing And Publication

- GitHub profile本文はrepository rootの`README.md`だけを正とする。別のprofile README、generated copy、publication checkoutを作らない。
- 編集前にremote/default branch、dirty state、現在のREADMEを確認し、local commitを同じGitHub `main`へpushまたはpull requestで統合する。
- profile本文に外部project、機能、version、URL、実績を追加する場合は、同じ作業で現在の公開事実を確認できない主張を作らない。

## Validation And Maintenance

- 公開前に`git diff --check`と`git status --short --branch`を確認し、root `README.md`がGit追跡対象であることを確認する。
- この`AGENTS.md`を作成、改訂、または実質変更した場合、final reportやcommitの前に`agents-md-clarifier`を適用する。

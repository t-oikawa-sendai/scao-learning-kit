# EVIDENCE

**Evidence Last Verified: 2026-08-26**

技術的事実、生成AIの特性、製品仕様、利用方法に関する記述は、原則として公式Documentation、公式発表、一次研究など、確認可能なEvidenceに基づいています。

この文書は、SCAO Learning Kitで使用する外部Evidenceの正本です。
SCAO独自の教材構成・学習順序・運用判断はEvidenceとは分離し、`project-notes/CURRENT.md` 等のRepository内正本で管理します。

## Type

- `OFFICIAL_DOC`：公式Documentation
- `OFFICIAL_ANNOUNCEMENT`：公式発表・公式Blog
- `OFFICIAL_SPEC`：公式Specification・標準仕様
- `OFFICIAL_REPOSITORY`：公式Repository
- `PEER_REVIEWED`：査読済み一次研究
- `PREPRINT`：未査読の一次研究
- `TECHNICAL_REPORT`：Technical Report

## Status

- `ACTIVE`：現在の教材で根拠として使用中
- `SUPERSEDED`：新しいEvidenceに置き換え済み
- `RETIRED`：現在の教材では使用していない

`SUPERSEDED` の場合のみ `Replaced By` を追加する。Evidence IDは一度付与したら変更せず、廃止後も再利用しない。

---

## EV-001

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: OpenAI
4. **Source Title**: Model guidance — Using GPT-5.6
5. **URL**: https://developers.openai.com/api/docs/guides/latest-model?model=gpt-5.6

## EV-002

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: Google
4. **Source Title**: Gemini 3 developer guide
5. **URL**: https://ai.google.dev/gemini-api/docs/gemini-3?hl=ja

## EV-003

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: Anthropic
4. **Source Title**: Prompting Claude Opus 5
5. **URL**: https://platform.claude.com/docs/ja/build-with-claude/prompt-engineering/prompting-claude-opus-5

## EV-004

1. **Type**: `OFFICIAL_SPEC`
2. **Status**: `SUPERSEDED`
3. **Provider**: Model Context Protocol
4. **Source Title**: Model Context Protocol Specification
5. **URL**: https://modelcontextprotocol.io/specification/2025-11-25
6. **Replaced By**: `EV-017`

## EV-005

1. **Type**: `PEER_REVIEWED`
2. **Status**: `ACTIVE`
3. **Provider**: Transactions of the Association for Computational Linguistics / MIT Press
4. **Source Title**: Lost in the Middle: How Language Models Use Long Contexts
5. **URL**: https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00638/119630/Lost-in-the-Middle-How-Language-Models-Use-Long

## EV-006

1. **Type**: `PEER_REVIEWED`
2. **Status**: `ACTIVE`
3. **Provider**: NeurIPS
4. **Source Title**: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks
5. **URL**: https://proceedings.neurips.cc/paper/2020/hash/6b493230-Abstract.html

## EV-007

1. **Type**: `OFFICIAL_ANNOUNCEMENT`
2. **Status**: `ACTIVE`
3. **Provider**: Anthropic
4. **Source Title**: Towards Understanding Sycophancy in Language Models
5. **URL**: https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models

## EV-008

1. **Type**: `PEER_REVIEWED`
2. **Status**: `ACTIVE`
3. **Provider**: Transactions of the Association for Computational Linguistics / ACL Anthology
4. **Source Title**: Automatically Correcting Large Language Models: Surveying the Landscape of Diverse Automated Correction Strategies
5. **URL**: https://aclanthology.org/2024.tacl-1.27/

## EV-009

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: OpenAI
4. **Source Title**: GPT-5 System Card
5. **URL**: https://deploymentsafety.openai.com/gpt-5

## EV-010

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: Anthropic
4. **Source Title**: Tool use with Claude
5. **URL**: https://docs.anthropic.com/en/docs/agents-and-tools/tool-use/overview

## EV-011

1. **Type**: `TECHNICAL_REPORT`
2. **Status**: `ACTIVE`
3. **Provider**: NIST
4. **Source Title**: Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile
5. **URL**: https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence

## EV-012

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: GitHub
4. **Source Title**: Removing sensitive data from a repository
5. **URL**: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository

## EV-013

1. **Type**: `OFFICIAL_SPEC`
2. **Status**: `ACTIVE`
3. **Provider**: GitHub
4. **Source Title**: GitHub Flavored Markdown Spec
5. **URL**: https://github.github.com/gfm/

## EV-014

1. **Type**: `PREPRINT`
2. **Status**: `ACTIVE`
3. **Provider**: arXiv
4. **Source Title**: Large Language Models Cannot Self-Correct Reasoning Yet
5. **URL**: https://arxiv.org/abs/2310.01798

## EV-015

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: Google
4. **Source Title**: Long context — Gemini API
5. **URL**: https://ai.google.dev/gemini-api/docs/long-context

## EV-016

1. **Type**: `OFFICIAL_DOC`
2. **Status**: `ACTIVE`
3. **Provider**: Microsoft
4. **Source Title**: Transparency Note: Phi Silica
5. **URL**: https://learn.microsoft.com/en-us/windows/ai/apis/phi-silica-transparency-note

## EV-017

1. **Type**: `OFFICIAL_SPEC`
2. **Status**: `ACTIVE`
3. **Provider**: Model Context Protocol
4. **Source Title**: Model Context Protocol Specification 2026-07-28
5. **URL**: https://modelcontextprotocol.io/specification/2026-07-28

# Repository Instructions

## Content Graph First

Before writing or substantially revising Korean chapters, read the local content graph.

Required route:

1. `graph/index.md`
2. `graph/rewrite-process.md`
3. The chapter's related graph node under `graph/nodes/`

Do not treat the graph as optional background. Use it as the working process.

## Korean Chapter Work

Korean chapters in `ko/` are not translations of the upstream notebooks.

For each new chapter or major rewrite, complete the `Source Reading Pass` from `graph/rewrite-process.md` before drafting:

```text
핵심 질문:
핵심 도구:
핵심 한계:
한국어 장의 새 흐름:
```

Use the source notebook or existing draft only to identify the core content. Do not preserve source sentence order, heading order, or exposition order.

If a reader confusion repeats, do not keep adding explanatory sentences to the same structure. Rebuild the chapter flow around the Korean reader's question sequence.

## Style Rules

- Write in Korean for the Korean lecture notes.
- Prefer direct, easy words over metaphors or decorative phrasing.
- Avoid analogies or expressions that different readers can interpret differently.
- New terms, formulas, and code should answer a need that the prior paragraph already created.
- Images should explain what to look at and what to compare.

## Python Environment

Use the repository-local `.venv` virtual environment for Python commands.

## Repository Boundaries

- `causal-inference-for-the-brave-and-true/` is the upstream reference. Do not edit it unless explicitly asked.
- `ko/` is the Korean lecture-note draft folder.
- `graph/` is the local process and content graph. Follow it even if it is ignored by git.

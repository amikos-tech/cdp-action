# ChromaDB Data Pipes 🖇️ - GH Action

This action allows you to use ChromaDB Data Pipes in your GitHub Actions workflow.

## Usage

```yaml
- name: ChromaDB Data Pipes
  uses: amikos-tech/cdp-action@main
  with:
    pipeline: |
      cdp ds-get "hf://tazarov/chroma-qna?split=train" | \
      cdp import "http://localhost:8000/chroma-qna" --upsert --create
```

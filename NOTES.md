# Notes on the consolidation

This repository was assembled on 2026-09-08 by cloning each original repository under `lenalehuby`, copying its working tree (excluding `.git`) into a folder of the same name, and skipping any single file larger than 5 MB.

## Files skipped for size (over 5 MB)

| File | Size | Original location |
|---|---|---|
| `Synthetic-Data-Generation-for-Perception/verify_annotations.ipynb` | 13.3 MB | https://github.com/lenalehuby/Synthetic-Data-Generation-for-Perception/blob/main/verify_annotations.ipynb (commit `75c2feb`) |

The notebook is still available in the original repository. Its size comes from embedded image outputs; a stripped copy (`jupyter nbconvert --clear-output`) would fit here if wanted.

## Other things worth knowing

- `Multimodal-Sentiment-Analysis/dataset/` contains roughly 4,900 JPEG images (about 215 MB total). Every file is under the 5 MB limit, so they were all copied.
- Git history was not preserved. The originals hold the commit history.
- Three repositories had no GitHub description (Counterfeit-Drug-Detection, Synthetic-Data-Generation-for-Perception, transformers-deployment-explainability). The README table summarises those from each project's own README and marks them with ¹.

## Redacted secrets

Two notebooks contained hard-coded Hugging Face user access tokens, which GitHub push protection rejects. The token strings were replaced with the placeholder `YOUR_HF_TOKEN_HERE` in:

- `brain-tumor-mri-classification/milestone-2.ipynb`
- `transformers-deployment-explainability/deploying_gradio.ipynb`

The original repositories still contain the real tokens, so those tokens should be revoked at https://huggingface.co/settings/tokens.

# Explainable PDF Malware Detection

A study of how explainability behaves on PDF malware classifiers — which
structural features drive a verdict, and how much of that explanation you can
actually trust.

Explored live at
**[anish-runtime.vercel.app/work/explainable-pdf-malware-detection](https://anish-runtime.vercel.app/work/explainable-pdf-malware-detection)**,
where you can toggle document features and watch a reconstructed study signal
move.

## Read this before anything else

**This repository contains the project report, and nothing else.** Two files: the
PDF, and this README. The model code, the notebooks, and the dataset are not
published here.

That is the honest framing, and the portfolio uses the same one. The project is
recorded there as `PUBLIC_DOCUMENT_VERIFIED` — a verified public document —
rather than `PUBLIC_CODE_VERIFIED`, precisely because the document is what is
public. The SHAP feature-attribution detail is recorded one step weaker still, as
`LIMITED_EVIDENCE`, because the report states results that the published
artefacts do not let you re-derive.

If you came here expecting a classifier you can run, there isn't one. Read the
report, or use the interactive reconstruction on the portfolio, which is clearly
labelled as a portfolio extension rather than a model output.

## What the report covers

[Explainable Machine Learning Models for Detecting PDF
Malware](<Explainable Machine Learning Models for Detecting PDF Malware.pdf>) —
structural feature extraction from PDF documents, classifier comparison, and
explainability analysis over the resulting predictions, with attention to which
features carry the signal and where the explanation becomes unreliable.

## The reconstruction on the portfolio

The lab at `/labs/malware` is a deterministic reconstruction, not this study
re-executed. Toggling a feature recomputes a weighted score locally in the
browser from fixed, published weights. It exists to make the _shape_ of the
reasoning tangible — which features move the number, and by how much.

What it deliberately does not do: accept a file upload, execute anything, or
produce a verdict. There is no file input in the page, and the interface states
that the output is a study signal rather than a security judgement. A portfolio
is not a place to imply you can scan someone's document.

## Provenance

Cited at a fixed commit so the reference cannot shift:

- Repository — [`ca79ecc`](https://github.com/anishakode/Malware-Detection-Using-ML/tree/ca79ecc8a013e96d5514243603b174bf86e52ecd)
- [The report itself](https://github.com/anishakode/Malware-Detection-Using-ML/blob/ca79ecc8a013e96d5514243603b174bf86e52ecd/Explainable%20Machine%20Learning%20Models%20for%20Detecting%20PDF%20Malware.pdf)

Machine-readable index of every claim made about this project:
[anish-runtime.vercel.app/evidence.json](https://anish-runtime.vercel.app/evidence.json)

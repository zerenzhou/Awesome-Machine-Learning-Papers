# Contributing Guidelines

Thank you for contributing to awesome-machine-learning-papers! This document explains how to add papers and what standards to follow.

## What We Accept

- **CCF-A venues prioritized**: NeurIPS, ICML, ICLR, CVPR, ICCV, ACL, EMNLP, KDD, AAAI, IJCAI, SIGIR, WWW, TPAMI, JMLR, etc.
- **High-impact CCF-B papers**: ECCV, NAACL, COLING, CIKM, WSDM, etc. — only widely cited or influential papers.
- **Welcome contributions**: New papers, missing classics, code links, summary improvements.

## Paper Entry Format

Every paper must follow this format:

```
- **Paper Title** — Venue Year [`tag1`] [`tag2`]
  [[Paper](link)] [[Code](link)]
  Brief one-sentence summary of the core contribution.
```

### Rules

- **Tags**: Domain files use technique tags (e.g., `Transformer`, `CNN`). Technique files use domain tags (e.g., `CV`, `NLP`).
- **Code link**: Include when an official repository exists. Omit otherwise — do not link unofficial reproductions.
- **One-sentence summary**: Describe the core contribution. One line maximum.
- **Ordering**: Papers are sorted by year in descending order (newest first).
- **Landmark marker**: Prefix pioneering papers with ⭐. This is reserved for widely recognized foundational work. If your PR adds this marker, explain why in the PR description.

## How to Contribute

1. Fork this repository
2. Add your paper entry in the correct file under `domains/` or `techniques/`
3. Follow the format above strictly
4. Submit a pull request with title: `Add <Paper Title> to <category>`

## Proposing New Categories

To propose a new domain or technique direction, open an Issue first for discussion before creating a PR.

## Quality Checklist

Before submitting, verify:

- [ ] Paper link points to the official publication or arXiv
- [ ] Venue and year are correct
- [ ] Tags match existing tag names used in the repository
- [ ] Summary accurately describes the core contribution
- [ ] Entry is placed in the correct chronological position (newest first)

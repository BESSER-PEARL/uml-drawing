# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/).

## [0.1.0] - unreleased

Initial release of the `uml-drawing` skill.

### Added
- `uml-drawing` skill: build a correct UML **class diagram** through BESSER
  B-UML — from a description or from existing code the agent reads — and
  deliver it either as **embedded B-UML code** in a Markdown doc or as an
  **SVG/PNG image** exported from the BESSER web editor.
- Scope is deliberately narrow for now: class diagrams only, always via
  BESSER B-UML.
- `.github/workflows/release.yml` — auto-creates a GitHub Release from the
  matching CHANGELOG section when a `v*` tag is pushed.

### Notes
- Image rendering currently happens only in the BESSER web editor (a browser
  step); a headless `model → SVG/PNG` exporter is requested upstream in
  [BESSER#553](https://github.com/BESSER-PEARL/BESSER/issues/553).

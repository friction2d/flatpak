---
layout: default
title: Friction Flatpak Repository
---
<style>
  .button-container { display: flex;gap: 2em;margin: 2em 0;flex-wrap: wrap; }
  .btn-install {padding: 1em 2em;color: white !important;text-decoration: none !important;border-radius: .5em;font-weight: bold;display: inline-block;transition: transform 0.2s, background-color 0.2s;text-align: center;min-width: 180px; }
  .btn-install:hover { transform: translateY(-2px); filter: brightness(1.1); }
  .btn-stable { background-color: #28a745; }
  .btn-nightly { background-color: #dc3545; }
  .btn-subtext { display: block;font-size: 0.75em;font-weight: normal;opacity: 0.9; margin-top: .5em; }
  .view, footer, header ul, header p, header h1 { display: none !important; }
  wrapper { width: auto !important;margin: 0 !important; }
  header, section { width: auto !important;float: unset !important;position: unset !important;border: 0 !important; }
  body {background-color: #0d1117 !important;color: #c9d1d9 !important; }
  a { color: #58a6ff !important; }
  a:hover { text-decoration: underline !important; }
  strong { color: #ffffff !important; font-weight: 600; }
  h1, h2, h3, h4 { color: #f0f6fc !important; }
  pre, code { background-color: #161b22 !important;border-color: #30363d !important;color: #e6edf3 !important; }
  .pl-s { color: #a5d6ff !important; }
  .pl-en { color: #d2a8ff !important; }
  .pl-k { color: #ff7b72 !important; }
  .pl-c { color: #8b949e !important; }
  code a { color: #58a6ff !important; }
  hr { background-color: #30363d !important; height: 1px; border: 0; }
  wrapper { border-color: #30363d !important; }
  .highlight { background-color: unset !important; }
  pre { overflow: hidden !important;white-space: pre-wrap !important;word-wrap: break-word !important; }
</style>

This is the official Flatpak repository for [**Friction**](https://friction.graphics). We provide rolling releases for both the **stable** (`v1.0`) and **nightly** (`main`) branches, built directly from [source](https://github.com/friction2d/friction).

By providing our own Flatpak repository, we deliver the latest features and bug fixes directly to you, independent of release cycles or third-party.

Updates are automated and run every **Monday**, **Wednesday**, and **Saturday** at **02:00 UTC**. Build time is ~40min.

<div class="button-container">
  <a href="https://flatpak.friction.graphics/friction-stable.flatpakref" class="btn-install btn-stable">
    Stable
    <span class="btn-subtext">Recommended (v1.0 branch)</span>
  </a>
  <a href="https://flatpak.friction.graphics/friction-nightly.flatpakref" class="btn-install btn-nightly">
    Nightly
    <span class="btn-subtext">Cutting-edge (main branch)</span>
  </a>
</div>

* Up-to-Date Shared Runtimes
* Enhanced Security
* Full Desktop Integration
* Efficient Updates

---

If you prefer the command line, follow these steps:

```
flatpak remote-add --if-not-exists friction-repo https://flatpak.friction.graphics/friction.flatpakrepo
```

#### Stable

```
flatpak install friction-repo graphics.friction.Friction
```

#### Nightly

```
flatpak install friction-repo graphics.friction.Friction//nightly
```

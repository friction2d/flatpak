---
layout: default
title: Friction Flatpak Repository
---
<style>
  .view, footer, header ul { display: none !important; }
  .button-container {
    display: flex;
    gap: 2em;
    margin: 2em 0;
    flex-wrap: wrap;
  }
  .btn-install {
    padding: 1em 2em;
    color: white !important;
    text-decoration: none !important;
    border-radius: .5em;
    font-weight: bold;
    display: inline-block;
    transition: transform 0.2s, background-color 0.2s;
    text-align: center;
    min-width: 180px;
  }
  .btn-install:hover {
    transform: translateY(-2px);
    filter: brightness(1.1);
  }
  .btn-stable { background-color: #28a745; }
  .btn-nightly { background-color: #dc3545; }
  .btn-subtext {
    display: block;
    font-size: 0.75em;
    font-weight: normal;
    opacity: 0.9;
    margin-top: .5em;
  }
  wrapper {
    width: auto !important;
    margin: 0 !important;
  }
  header, section {
    width: auto !important;
    float: unset !important;
    position: unset !important;
  }
</style>

This is the official Flatpak repository for [**Friction**](https://friction.graphics). This repository provides rolling releases for the stable (`v1.0`) and nightly (`main`) branches directly from the source.

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

**Will also be available on FlatHub after Friction v1.0.0 formal release, but only traditional stable releases.**

---

If you prefer the command line, follow these steps:

```bash
flatpak remote-add --if-not-exists friction-repo https://flatpak.friction.graphics/friction.flatpakrepo
```

#### Stable

```bash
flatpak install friction-repo graphics.friction.Friction
```

#### Nightly

```bash
flatpak install friction-repo graphics.friction.Friction//nightly
```

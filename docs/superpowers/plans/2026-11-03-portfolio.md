# Portfolio Implementation Plan

> Execute inline using superpowers:executing-plans. User approved the static approach; finish locally as subsequently requested.

**Goal:** Deliver a responsive, accessible portfolio and a format-preserving résumé update.

**Architecture:** Buildless HTML/CSS with progressive JavaScript enhancement. Self-contained downloadable DOCX and a Node development server.

**Tech Stack:** HTML, CSS, browser JavaScript, Node.js built-in HTTP server.

**Spec:** ../specs/2026-11-03-portfolio-design.md

## Global Constraints

- Preserve supplied facts and résumé formatting.
- No runtime dependencies or external accounts required.
- Local completion only; initialize main and the supplied remote.

## Review Focus

- Mobile: all sections fit at 375px and navigation remains usable.
- Keyboard: visible focus and functional theme/menu controls.
- Missing JavaScript: résumé, project links, content, and navigation remain available.
- Storage disabled: theme still switches without exceptions.
- Downloads: linked résumé exists and contains the requested update.

## Tasks

- [x] Update Word document text while preserving other XML and ZIP contents.
- [x] Create index.html, styles.css, script.js, favicon.svg, and assets/Santosh-Kumar-Yadav-Resume.docx.
- [x] Add a dependency-free server, GitHub Pages deployment instructions, and local Git configuration.
- [x] Verify resume XML/ZIP integrity, browser interactions, theme persistence, mobile overflow, and all internal links. Capture desktop/mobile previews.
- [x] Commit the verified result locally. Do not push.

## Verification record

JavaScript syntax checks passed. Chromium checks passed at 320, 375, 560, 768, 1024 and 1440px: no horizontal overflow; working mobile menu and Escape focus return; theme switching and persistence; theme still works with storage blocked; reduced motion honored; content/navigation accessible without JavaScript; internal section targets valid; résumé download succeeds; local server excludes private source files. No browser JavaScript errors. Desktop, mobile, and dark screenshots inspected. A fresh independent static review found no important issues.

The original and updated DOCX contain the same eight ZIP entries. Every entry except word/document.xml matches byte-for-byte. That XML differs only in the expanded BoomConsole paragraph and the supplied email; all styling markup is preserved. Downloadable and workspace copies have matching SHA-256 hashes.

Execution rulings: use a new dedicated repository directory to isolate unrelated personal documents; no framework or dependency installation needed. Use Node directly on Windows because PowerShell blocks npm.ps1. GitHub publishing deferred per the user's explicit request to finish locally.

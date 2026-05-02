# README Refresh Design

## Goal

Make README feel more alive through stronger structure and more visual hierarchy while keeping it professional and GitHub-friendly.

## Scope

- Preserve banner.
- Restructure README for faster scanning.
- Add more visual blocks using markdown, tables, badges, and section layout.
- Keep current installation and usage guidance intact in substance.
- No behavior changes to skill files.

## Chosen Approach

Use editorial product page structure with selective command-center navigation.

Reason:
- Feels polished without becoming noisy
- Improves scan speed
- Adds visual energy through grouped sections instead of decorative clutter
- Fits GitHub markdown constraints

## Content Direction

- Tone: polished product vibe
- Focus: stronger structure and more visuals
- Keep copy concise, direct, and practical

## Structure

1. Banner
2. H1
3. Short hero summary
4. Quick navigation strip
5. Quickstart tiles
6. Featured agent cards
7. Installation
8. Invocation examples
9. Full agent list
10. Recommended workflows
11. Notes, contributing, license

## Visual Direction

- Product-style intro section
- Compact callout blocks near top
- Quickstart section surfaced earlier
- Featured agent section styled with dark console cards
- Keep detailed long-form prompt examples lower in page

## Featured Visual Choices

- Primary page direction: Editorial Product Page
- Featured agent card style: Dark Console Cards
- Extra visual block: Quickstart Tiles

## File Changes

- Modify `README.md`
- Keep `assets/banner.svg`

## Constraints

- GitHub markdown only
- No heavy HTML dependence unless necessary
- No external assets
- No loss of key installation or invocation content
- Must remain readable in GitHub light theme

## Verification

- Confirm README top sections reflect new structure
- Confirm banner still renders
- Confirm installation commands still present
- Confirm all 16 agents still documented

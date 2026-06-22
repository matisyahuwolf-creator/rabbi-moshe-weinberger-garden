# Publishing This Quartz Garden

This folder is a real Quartz 5 site for the Rabbi Moshe Weinberger research archive.

## Local rebuild

From the workspace root:

```bash
python3 scripts/build_quartz_content.py
```

From this `quartz/` folder, using Node 22+:

```bash
node quartz/bootstrap-cli.mjs build
```

For local preview:

```bash
node quartz/bootstrap-cli.mjs build --serve --baseDir rabbi-moshe-weinberger-garden
```

## GitHub Pages

The deploy workflow is in `.github/workflows/deploy.yml`.

Expected public URL:

```text
https://matisyahuwolf-creator.github.io/rabbi-moshe-weinberger-garden/
```

Before first deploy, create the GitHub repo and push this `quartz/` folder as the repo root. Then set GitHub Pages to use GitHub Actions:

Repository Settings -> Pages -> Source -> GitHub Actions.

## Content Note

The source pages include public YUTorah links and machine-generated transcripts where available. Review transcript text against audio before quoting.

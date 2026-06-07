# LocalCraft Site Repo Manifest

This file is the canonical link between this customer site and its hosting infrastructure. Any agent (Claude session, build skill, operator) MUST read this file before any git operation.

If the values below don't match the actual `git remote -v` + `git config user.email`, STOP. Something is misconfigured.

> Note: this site predates BUILD-STANDARDS §17 and lives at a non-standard path (the ClickCampaigns `campaigns/brand-launch/` layout, not `clients/{slug}/output-assets/html`). The `repo_path` below is authoritative — do NOT infer it from the slug. Backfilled once via the adapted manifest-bootstrap procedure on 2026-06-07.

## Quick reference

- **Customer slug**: market-and-main
- **GitHub repo**: jakesebok/marketandmain-website
- **Vercel project**: marketandmain-website
- **Production URL**: https://marketandmain-website.vercel.app
- **Custom domain**: mm.localcraftdigital.com
- **Git identity**: jake@localcraftdigital.com / jakesebok

```json
{
  "schema_version": 1,
  "slug": "market-and-main",
  "repo_path": "/Users/jakesebok/Repos/clients/market-and-main/campaigns/brand-launch/output-assets/html",
  "non_standard_path": true,
  "github": {
    "owner": "jakesebok",
    "name": "marketandmain-website",
    "url_https": "https://github.com/jakesebok/marketandmain-website.git",
    "url_ssh": "git@github.com:jakesebok/marketandmain-website.git",
    "visibility": "private"
  },
  "vercel": {
    "project_name": "marketandmain-website",
    "project_id": "prj_UD7Fg5wtBTxKCbm7pHbQOWNRpAvo",
    "org_id": "team_sJ7RnhGKyz1UQNfM0dutAwcL",
    "production_url": "https://marketandmain-website.vercel.app",
    "custom_domain": "mm.localcraftdigital.com",
    "created_at": null
  },
  "git_identity": {
    "email": "jake@localcraftdigital.com",
    "name": "jakesebok"
  },
  "created_at": "2026-06-07T21:42:50Z",
  "created_by": "customer-site-git:manifest-bootstrap (adapted for non-standard campaigns path)"
}
```

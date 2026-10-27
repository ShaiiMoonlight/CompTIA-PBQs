# Packet Practice

Free, independent IT performance-based practice for GitHub Pages. Five interactive labs cover UPS power, IPv4 troubleshooting, RAID replacement, PC builds, and access-point placement. Feedback explains each answer. Completed labs are stored only in local browser storage; no accounts or analytics.

## Run locally

From this checkout:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open the local server in your browser. No install or build step is required. HTML, CSS, and JavaScript are intentionally dependency-free. Asset paths also work under `/CompTIA-PBQs/`.

## Publish on GitHub Pages

Push these files to the repository's `main` branch. In GitHub repository **Settings → Pages → Build and deployment**, choose **GitHub Actions**. The included workflow deploys on pushes to `main` and can be run manually. A GitHub Pages deployment has not been performed by this setup task.

## Scenario assumptions

These are original educational adaptations, not official CompTIA questions. Ambiguities in the supplied notes are resolved explicitly in each scenario: the UPS has sufficient capacity; router `.1` is a host address, not a network address; RAID 5 with one failed disk is degraded; eligible RAID spares are SAS HDDs, with lowest capacity then highest RPM used to choose; the gaming audio requirement is explicit; the access-point lab includes a simplified floor plan and interference assumptions. Real deployments require manufacturer specifications and measurements.

## Browser checks

Run `node --check app.js` for syntax. Functional coverage should include wrong answers, all five correct solutions, reset, unique PC addresses, saved completion after reload, and mobile layout. Browser storage may be unavailable; the labs still work without persistence.

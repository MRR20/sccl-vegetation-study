Singareni vegetation study: project documentation portal
=========================================================

A static website (HTML + CSS, no JavaScript, no build step, no internet needed).
All links are relative, so it works from any folder or sub-path, for example:

  https://your-site.example/                    (site root)
  https://your-site.example/projects/sccl/      (sub-path)
  file:///C:/Users/.../site/index.html          (opened straight from disk)

Hosting options
  - GitHub Pages: push the contents of this folder to a repo (or a /docs folder)
    and enable Pages. The site works under https://<user>.github.io/<repo>/.
  - Netlify / Vercel / Cloudflare Pages: drag and drop this folder.
  - University or Apache/Nginx server: copy the folder anywhere under the web root.
  - Quick local test: in this folder run  python -m http.server 8000
    and open http://localhost:8000

Before publishing
  - Replace [Student name], [Roll number], [Supervisor name] and [Designation]
    in index.html and downloads.html.
  - assets/docs/dissertation_phase1_report.pdf still has template placeholder names;
    replace it with your final PDF (keep the same file name, or update downloads.html).

Structure
  index.html            Overview, NDVI stripes, key findings, abstract
  study-area.html       Leases and distance zones
  data.html             Datasets and Landsat scene list
  methods.html          NDVI, trend tests, why detrending is needed
  results.html          Trends, maps, anomalies, climate, production, correlations
  discussion.html       Interpretation
  next-steps.html       Limitations and planned work
  references.html       15 references
  downloads.html        Data tables, code, report
  assets/style.css      All styling
  assets/img/           Figures
  assets/data/          CSV tables
  assets/code/          Python scripts
  assets/docs/          Report PDF

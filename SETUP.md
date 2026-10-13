# Set up your GitHub profile

1. Log in to GitHub as `ilysmxtr`.
2. Create a **public** repository named exactly `ilysmxtr` and initialize it with a README (or use the existing one).
3. Upload the supplied `README.md` to the **root** of the repository on its default branch.
4. Upload `.github/workflows/snake.yml` while preserving the exact folder structure.
5. Open repository **Actions** > **Generate contribution snake** > **Run workflow** (on `main`).
6. Check that the run succeeds and creates the `output` branch. The animated snake then appears on the profile. If it fails due to permissions, open **Settings > Actions > General > Workflow permissions**, enable **Read and write permissions**, save, and rerun.
7. Optional: replace the generic LinkedIn homepage link in README.md with your exact LinkedIn profile URL.
8. Pin your best public repositories under **Profile > Customize your pins**.

Notes:
- GitHub profile READMEs support Markdown, some HTML, and remote SVG/GIF images, but not arbitrary JavaScript on the page.
- Animated text, header, badges and charts depend on external image services.
- The snake SVG will not display until the workflow has generated the `output` branch.
- The activity statistics reflect public/accessible GitHub data and may be cached.

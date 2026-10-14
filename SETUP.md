# Install the Neon GitHub Profile

**Repository:** https://github.com/ilysmxtr/ilysmxtr  
**Default branch:** `main`  
**You already have this profile repository. Do not create another one.**

## Easy way: upload all files in the browser

1. Download the ZIP and extract it to a folder on your computer. Ensure your file manager shows hidden dot-folders such as `.github`.
2. Open: https://github.com/ilysmxtr/ilysmxtr
3. In the repository, click **Add file → Upload files**.
4. Drag **`README.md` and the whole `assets` folder** from the extracted package onto GitHub's upload area. When prompted, replace `README.md`.
5. Commit the changes to `main`.
6. To upload the workflow, open **Add file → Create new file**. Set the new filename exactly to `.github/workflows/snake.yml`; paste the contents of the packaged file. If the path already exists, open the existing file, click **Edit (pencil)**, and replace its contents instead.
7. Commit again.
8. Visit **Actions → Generate neon contribution snake → Run workflow → Run workflow**.
9. When the run succeeds, reload your profile: https://github.com/ilysmxtr

**Note:** If your browser does not preserve folders when dragging them, use the terminal method below. A plain GitHub web upload can't always upload a folder in the way you expect.

## Reliable way: upload with Git (recommended)

On your computer, unpack the ZIP, open a terminal inside the unpacked folder, then run:

```bash
# Clone the existing special profile repository into a separate folder
cd ..
git clone https://github.com/ilysmxtr/ilysmxtr.git

# Enter it and copy README.md + assets/ + .github/workflows/snake.yml
# from the extracted download into this cloned repository.
cd ilysmxtr

git add README.md assets .github/workflows/snake.yml
git commit -m "Redesign GitHub profile with neon animation"
git push origin main
```

The ZIP contains only the files needed for your profile, not a Git repository. Do not run `git init` inside the ZIP folder.

## Important notes

- The image in the header is an animated **GIF** for reliable motion on GitHub. `assets/hero.svg` is the editable vector source; `assets/hero-still.png` is a static backup.
- SVG source assets (`assets/ecosystem.svg` and `assets/footer.svg`) don't need JavaScript and have static visual fallbacks.
- Snake SVGs come from the existing `output` branch; this workflow refreshes them daily.
- If Actions says permission denied while publishing, open repository **Settings → Actions → General → Workflow permissions** and enable **Read and write permissions**. Then rerun.
- GitHub may block Actions from running automatically in inactive repositories; manually running it reactivates it.
- Statistics and typed text are served by external image services. They may be slow or temporarily unavailable.
- The projects section is intentionally removed. Your **portfolio URL remains in your profile bio**; nothing in this package overwrites that bio.
- You can customize copy and links later by editing `README.md`, and the custom vector artwork in `assets` is editable.

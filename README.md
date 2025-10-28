<div align="center">

# Aidan Ream

<!-- Hero GIF: store in your repo, e.g., docs/hero.gif -->
<img src="docs/roma.gif" alt="3D/Project" width="800" />

</div>

---

## About me

- LAES Undergraduate at Calpoly Slo
- Concentration in Graphic Programming 
- Currently working with 4D Gaussian Splatts

## Featured work

> Swap in links, repos, or case studies. Include a brief 1–2 line description each.

- **Project One** — What it is, notable tech, and outcome. [[repo]](https://github.com/YOUR_HANDLE/PROJECT_ONE) · [[demo]](https://example.com/demo)
- **Project Two** — Quick value prop or result. [[repo]](https://github.com/YOUR_HANDLE/PROJECT_TWO)
- **Project Three** — One-liner, keep scannable. [[repo]](https://github.com/YOUR_HANDLE/PROJECT_THREE)

## Languages

`java` · `python` · `c++` `javascript` · `react` 

## Software 

 `blender` · `maya` · `photoshop` · `illustrator` · `renderdoc` · `meshlab` 

## Libraries and Game Engines

 `nodejs` · `unity` · `opengl` · `vulkan` 
 
## Reach out!

- 📨 Email: aidanream01@gmail.com
<!--- 🌐 Site: https://your-website.example-->
- 💼 LinkedIn: https://linkedin.com/in/aidan-ream-076757317/


### How to add the GIF at the top

1. **Record a short clip** (10–15s) of your project or 3D view (e.g., macOS Screenshot app, Windows Game Bar, or OBS) and save as `.mp4` or `.mov`.
2. **Convert to a lightweight GIF** (target ≤ 6–8 MB so GitHub loads it fast):

   **Using ffmpeg** (install via Homebrew/Chocolatey or your package manager):

   ```bash
   # 1) Convert to a high-quality palette for better colors
   ffmpeg -y -i input.mp4 -vf "fps=30,scale=1280:-1:flags=lanczos,palettegen=stats_mode=diff" palette.png

   # 2) Use the palette to make a smaller, cleaner GIF
   ffmpeg -i input.mp4 -i palette.png -lavfi "fps=30,scale=1280:-1:flags=lanczos [x]; [x][1:v] paletteuse=dither=bayer:bayer_scale=5" -loop 0 docs/hero.gif
   ```

   **Quick size tips**
   - Trim the clip to 6–10 seconds.
   - Reduce fps to 20–24 if size is too large (`fps=24`).
   - Scale width to 960 or 720 if still heavy (`scale=960:-1`).
   - Consider WebP (much smaller) if you plan to host externally and embed with `<img src>`.

3. **Add to your repo** at `docs/hero.gif` and commit. The tag up top already references that path:

   ```md
   <img src="docs/hero.gif" alt="3D/Project preview" width="800" />
   ```


### README formatting tips

- Keep the **top fold** focused: name, GIF, 2–3 badges.
- Make all links **actionable** (demo, docs, repo). Avoid dead links.
- Prefer **short sections** over walls of text.
- Use **pinned repos** on your profile to spotlight deeper dives.
- Update GIFs when projects evolve, even a small refresh stands out.

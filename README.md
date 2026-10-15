# Henryville

A 3D island village portfolio for Dr. Henry Yu. Each building opens a section of the CV, every stall in the Maker's Market links to a website Henry built, and Frog Baby walks visitors around.

## Files

- `index.html` : the whole page (village, CV content, site list, tour)
- `assets/henry.jpg` : portrait in the About panel
- `assets/frogbaby.jpg` : Frog Baby character sheet in the guide panel
- `assets/og-image.jpg` : the preview card shown when the link is shared
- `assets/favicon-32.png`, `icon-192.png`, `favicon.ico`, `apple-touch-icon.png` : browser tab and home screen icons
- `for-meshy/` : front, side, and back views of Frog Baby for making a 3D model. You do not need to upload this folder to GitHub.

## Publish on GitHub Pages

1. Create a public repository named `Henryville`.
2. Upload everything in this folder (keep the `assets` folder).
3. Settings, then Pages. Deploy from a branch, `main`, `/ (root)`, Save.
4. The site goes live at `https://hyeonhoyu.github.io/Henryville/`.

If you use a different repository name, open `index.html` and change the two `og:` URLs near the top so the share preview still works.

## Features

- Take the tour: Frog Baby walks through eight stops with a speech bubble at each.
- Night and Day: switches the lighting. Windows, street lamps, and stars light up at night. The choice is remembered.
- Sound: off by default. Turn it on for cardinal chirps, the bell tower, the scramble crossing signal, and soft clicks. All sounds are made in the browser, so there are no audio files.
- Market filters: tap a topic to show only those sites. Matching stalls lift up on the island.

## Editing content

Near the top of the script in `index.html`:

- `SITES` : name, link, tags, color, and description for each market stall
- `PUBS` : publications
- `PLACES` : text for every building panel
- `TOUR` : the stops and what Frog Baby says at each one
- `VIDEOS` : YouTube videos in the Cinema. Add a line with the video id (the part after `youtu.be/`). Titles load from YouTube automatically, or type your own in `title`.

## Adding a real 3D Frog Baby

1. Go to Meshy (meshy.ai) or Tripo (tripo3d.ai) and choose Image to 3D.
2. Upload `for-meshy/frogbaby-front.png`. If the tool offers multi-view input, also add the side and back images.
3. Optional: use the tool's auto rigging and add a walking animation and an idle animation. The page plays any animation whose name contains "walk" while Frog Baby moves, and "idle" while standing still.
4. Download as GLB, ideally under 10 MB, and save it as `assets/frogbaby.glb`.
5. Upload it to GitHub. The page finds it, scales it, and replaces the built-in Frog Baby.

If the model faces the wrong way, open `index.html`, find `FROG_MODEL`, and change `turn:0` to `turn:Math.PI`. Change `height` to make it bigger or smaller.

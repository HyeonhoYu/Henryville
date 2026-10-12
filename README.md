# Henryville

A 3D island village portfolio for Hyeonho (Henry) Yu, Ph.D. Each building opens a section of the CV, and every stall in the Maker's Market links to a website Henry built. Frog Baby walks visitors to each building.

## Files

- `index.html` : the whole page (village, CV content, and site list)
- `assets/frogbaby.jpg` : Frog Baby character sheet shown in the guide panel
- `assets/frogbaby-poses.jpg` : extra pose sheet (not used yet)
- `assets/favicon-32.png`, `icon-192.png`, `favicon.ico`, `apple-touch-icon.png` : browser tab and home screen icons made from Henry's photo
- `assets/frogbaby.glb` : optional. Add a 3D model with this exact name and it replaces the built-in Frog Baby automatically.

## Publish on GitHub Pages

1. Create a new public repository, for example `henryville`.
2. Upload everything in this folder (keep the `assets` folder).
3. Open Settings, then Pages. Under Build and deployment, choose Deploy from a branch, select `main` and `/ (root)`, then Save.
4. After a minute the site is live at `https://hyeonhoyu.github.io/henryville/`.

## Editing content

Open `index.html` and look near the top of the script:

- `SITES` : name, link, color, and description for each market stall
- `PUBS` : publications
- `PLACES` : text for every building panel

## Adding a real 3D Frog Baby

1. Turn the character image into a 3D model with an image to 3D tool such as Meshy or Tripo.
2. Export as GLB, keep it under about 10 MB.
3. Save it as `assets/frogbaby.glb` and upload. The page scales and places it on its own.

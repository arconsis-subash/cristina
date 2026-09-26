Leaf Story — animated "leaf growth" timeline

This small demo lives in leaf-story/ and uses a copy of the project's timeline JSON. It references images from the existing timeline/images/ folder to avoid duplicating large files.

Quick start (serve locally):

1. From the repo root, run:
   python3 -m http.server 8000
2. Open http://localhost:8000/leaf-story/index.html

Notes:
- Data source: leaf-story/data/timeline.json (copy of timeline/data/timeline.json)
- Images are loaded from ../timeline/images/<filename> — ensure the main timeline/images folder exists and filenames match.
- This is a static client-only demo (no backend). To change events, edit the JSON copy here.

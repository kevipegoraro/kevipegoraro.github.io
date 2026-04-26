# kevipegoraro.github.io

## Overview

This project is a simple HTML webpage that demonstrates how to add and display multimedia content using HTML. It includes:

* A heading
* An audio player with autoplay and controls
* An embedded YouTube video

---

## Features

### 1. Page Title

Displays a heading

### 2. Audio Player

* Plays a local `.mp3` file
* Includes controls (play, pause, volume)
* Uses autoplay (may be restricted by browsers)

### 3. Embedded Video

* Embeds a YouTube video using an `<iframe>`
* Uses the correct `/embed/VIDEO_ID` format

---

## File Structure

```
project-folder/
│── index.html
│── audio.mp3
```

---

## How to Run

### Option 1 (Recommended)

Use a local server:

```bash
python -m http.server
```

Then open:

```
http://localhost:8000
```

### Option 2

Open `index.html` directly in a browser (may cause embed issues).

---

## How to Customize

### Change the Name

Edit the heading in `index.html`:

```html
<h1>Kevi Pegoraro Favorite Media</h1>
```

### Change Audio

Replace:

```
audio.mp3
```

with your own file (same folder, exact name).

### Change Video

1. Take a YouTube link:

   ```
   https://www.youtube.com/watch?v=VIDEO_ID
   ```
2. Convert to:

   ```
   https://www.youtube.com/embed/VIDEO_ID
   ```
3. Update the `<iframe>` `src`.

---

## Supported Formats

* Audio: `.mp3`, `.wav`
* Video (local): `.mp4`
* Embedded: YouTube via `<iframe>`

---

## Known Issues

* **Autoplay may not work** unless audio is muted
* **Error 153** can occur if:

  * Using incorrect YouTube URL
  * Opening via `file://` instead of a server
  * Network restrictions (e.g., school Wi-Fi)

---

## Technologies Used

* HTML5 (`<audio>`, `<video>`, `<iframe>`)

---

## Author

Kevi Pegoraro

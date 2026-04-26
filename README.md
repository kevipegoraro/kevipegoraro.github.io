
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Kevi Pegoraro - Favorite Media</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #1f1c2c, #928dab);
            color: #fff;
            margin: 0;
            padding: 0;
        }

        header {
            text-align: center;
            padding: 30px;
            background-color: rgba(0,0,0,0.4);
        }

        h1 {
            margin: 0;
            font-size: 2.5rem;
        }

        .container {
            max-width: 800px;
            margin: 30px auto;
            padding: 20px;
        }

        .card {
            background: rgba(0,0,0,0.5);
            padding: 20px;
            margin-bottom: 25px;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.4);
        }

        .card h2 {
            margin-top: 0;
            font-size: 1.4rem;
            border-bottom: 1px solid #ccc;
            padding-bottom: 8px;
        }

        audio, video, iframe {
            width: 100%;
            margin-top: 15px;
            border-radius: 8px;
        }

        iframe {
            height: 400px;
        }
    </style>
</head>

<body>

<header>
    <h1>Kevi Pegoraro Favorite Media</h1>
</header>

<div class="container">

    <div class="card">
        <h2>Audio - Never Gonna Give You Up</h2>
        <audio controls>
            <source src="audio.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
    </div>

    <div class="card">
        <h2>YouTube - Never Gonna Give You Up</h2>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=3XUFhpAC5IIozsMy" 
         title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; 
         clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
         referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
        </iframe>
    </div>

    <div class="card">
        <h2>Video File - Never Gonna Give You Up</h2>
        <video controls>
            <source src="video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

</div>

</body>
</html>



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

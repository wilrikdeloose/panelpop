# PanelPop Comic Viewer

A sleek, interactive comic viewing experience that presents comic panels chapter by chapter, horizontally, and transforms them into an immersive fullscreen presentation with smooth zooming transitions.

## Features

-   **Horizontal Chapter Layout:** Chapters are displayed side-by-side, allowing for horizontal scrolling through the comic.
-   **Grid-Based Chapter Panels:** Within each chapter, the cover spans the top, and panels are arranged in a responsive 3-column grid (top-to-bottom, left-to-right).
-   **Smooth Zooming Transitions:** Seamlessly zooms into each panel for focused viewing.
-   **Narration Boxes:** Supports optional narration text overlays on panels with configurable positioning.
-   **Background Effects:** Subtle background blur derived from the current panel enhances immersion.
-   **Greyscale Effect:** Non-focused panels are elegantly greyed out.
-   **Keyboard Controls:** Full control via keyboard:
    -   `Spacebar`: Start the presentation / Pause / Resume.
    -   `ArrowLeft`: Navigate to the previous panel (pauses automatic playback).
    -   `ArrowRight`: Navigate to the next panel (pauses automatic playback).
-   **Configurable Starting Point:** Choose which panel the presentation starts from.
-   **Fullscreen Presentation Mode:** Maximizes viewing area.
-   **Refined Visuals:** Hidden horizontal scrollbar and a subtle whitespace margin around zoomed panels.

## Usage

1.  Place your comic image files (e.g., `1_0.png`, `1_1.png`, ...) inside the `images/` subfolder.
2.  Configure the image sequence, chapters, and optional narration in the `config.images` array within `index.html`.
3.  Customize visual effects, layout, and timing in the `config` object in `index.html`.
4.  Open `index.html` in a modern web browser.
5.  Click the overlay or press `Spacebar` to start the presentation.

## Configuration (`config` object in `index.html`)

The viewer is highly configurable via the `config` object:

-   **`background`**: Adjust background blur, brightness, opacity, zoom, and offset.
-   **`transition`**:
    -   `transitionEffectDuration`: Duration (seconds) for effects like greyscale fade.
    -   `initialDelay`: Time (ms) the first panel is shown before animation starts.
    -   `timeBetweenSlides`: Time (ms) each subsequent panel is shown.
    -   `greyOutDelay`: Delay (ms) before zooming after greying out panels.
    -   `startingFrameIndex`: The index (starting from 0) of the panel to begin the presentation with.
-   **`layout`**: Control the gap between chapter columns (`columnGap`), image border width, and canvas padding.
-   **`effects`**: Set the intensity of the `greyscaleAmount` for inactive panels.
-   **`images`**: Define the sequence of images, their chapter, cover status, and optional narration (`line` and `position`).

Perfect for webcomics, digital storytelling, and interactive narrative presentations requiring a polished, cinematic feel.

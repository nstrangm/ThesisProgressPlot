# Thesis in progress

A build-free hallway display for the existing `scripts/thesis_progress.png`.

## GitHub Pages

Merge the accompanying pull request. In repository Settings → Pages, select **Deploy from a branch**, **main**, and **/ (root)**, if those are not already selected.

The page will be available at https://nstrangm.github.io/ThesisProgressPlot/ once GitHub finishes deploying.

## Updating the display

Continue replacing `scripts/thesis_progress.png` as usual. The page checks for a fresh image every five minutes and retains the last successfully loaded image if a refresh fails. Changes become available after the GitHub Pages deployment completes.

Use the Fullscreen button on the hallway computer. The display shows that computer's local time. The small “Image checked” label indicates when the image was successfully fetched, not when the thesis was last edited.

The page uses no external fonts, scripts, or libraries. For local file and localhost previews only, the image loads from this public repository's main branch. On GitHub Pages the image uses a relative path.

## Customization

Edit the heading, subtitle, and `quips` array in `index.html`. Set `IMAGE_PATH` if the image location changes, and `REFRESH_MS` to adjust the refresh interval. Reduced motion preferences disable the orbit animation.

# Jiohotstar App — Fullscreen Exit Ratio Bug
Bug Report 
## 1. Bug Title

Video player fails to restore default ratio after exiting full screen; black strip appears on one side (Movies & Live)

## 2. Environment

Device: iQOO Neo 10R (Model No. 12221)

OS: Origin OS 6

Network: Cellular Data

App: Jio Hotstar

App Version: 25.11.10.3

Date Tested: 11/12/2025

Reproduction Frequency: 100% (Every time)

## 3. Module

Video Player → Full Screen Toggle (Movie Player + Live Player)

## 4. Preconditions

User has opened any playable Movie or Live stream.

Video loads correctly in default embedded player size.

## 5. Steps to Reproduce

1.Open the JioHotstar app.

2.Play any movie OR open any live stream.

3.Keep the video in default (embedded) player ratio.

4.Tap the Full Screen icon to expand the video.

5.Now tap the Exit Full Screen / shrink icon to return to default ratio.

6.Observe the video frame and screen area after exiting full screen.

## 6. Expected Result

When user expands the video, it should correctly scale to full screen.

When user exits full screen, the video should return exactly to the original default ratio without any distortion.

No black bars/strips should appear on any side of the player.

## 7. Actual Result

After exiting full screen, the video fails to return to original default ratio.

A thin black strip appears on one side of the video screen.

Movies: one side becomes black.

Live streams: side near navigation buttons shows a black strip.

Video player layout becomes misaligned.

## 8. Severity

Medium → High
Affects UX for all video content (Movies + Live).

## 9. Priority

Medium

## 10. Impact

Viewing experience breaks for all video types.

Player does not fully restore after full screen toggle.

On some devices/aspect ratios, user may feel video is cropped or shifted.

Creates a perception of app instability.

## 11. Additional Notes

Issue occurs consistently on iQOO Neo 10R (Origin OS 6).

Likely related to incorrect player container resizing or safe-area inset handling on exit-fullscreen event.

Live streams and movies both affected.

# everfocus-ipcam-viewer

Everfocus is a DVR manufacturer. Like most IP camera vendors, they have terrible browser support and otherwise terrible support for viewing camera footage.

## Requirements

You need to enable MJPEG instead of H.264. MJPEG uses a bit more bandwidth, but is required to enable viewing Everfocus via the mobile site.

## Configuration

Set your IP address in the `ipCamera` variable in `index.html`.

## Enhancements

 * Stream footage at maximum capacity (previously hardcoded to 200ms)
 * Switching channels doesn't re-render the entire app
 * More efficient (renders into a single element, uses modern development practices)

## Browser support

 * Tested on the latest version of Chrome, Linux.

## Plans

I plan to include more features than Everfocus natively ships with, including:

 * Custom camera layouts
   * Name your cameras
   * View more than one camera at a time
 * Dead camera detection
 * Brightness / contrast controls
 * Digital zoom

## Development

Currently one index.html file with some modern JS.

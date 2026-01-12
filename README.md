# dxvk-frame-skipper
This DXVK patch limits the number of frames rendered on the GPU without changing the application-side FPS rate.

It is useful for games or applications that benefit from a higher internal framerate (for example, improved physics simulation) but are GPU-limited and cannot efficiently render that many frames at sufficient quality. Additionally, since only a limited number of frames can be presented on the screen due to the monitor’s refresh rate, the obvious solution is to limit the rendering framerate to the display’s refresh rate while allowing the application to run at the maximum FPS it can achieve.

This approach prevents frames that cannot be presented due to the limited refresh rate from being rendered at all, thereby saving GPU resources and reducing energy consumption.

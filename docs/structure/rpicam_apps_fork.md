# rpicam-apps-fork repository

https://github.com/secluso/rpicam-apps-fork

https://github.com/raspberrypi/rpicam-apps [v1.9.0]


Unix Socket: /tmp/rpi_raw_frame_socket
Accessed by: https://doc.rust-lang.org/std/os/unix/net/struct.UnixStream.html

Modification of rpicam-apps: https://github.com/secluso/rpicam-apps-fork/commit/37356495ce7c3c49e44e45a7f1622f04373bacba
Usage in rpi_dual_stream: 
- Opening: https://github.com/secluso/core/blob/ae2069a305cbdd65048735971585c8376042a111/camera_hub/src/raspberry_pi/rpi_dual_stream.rs#L154
- Reading: https://github.com/secluso/core/blob/ae2069a305cbdd65048735971585c8376042a111/camera_hub/src/raspberry_pi/rpi_dual_stream.rs#L129
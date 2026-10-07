# FPGA OV5640 Camera (720p)

Gowin FPGA project for capturing 1280x720 RGB565 video from an OV5640 camera and sending each image row over UDP/RGMII to an RK3588 receiver for display.

- Gowin project: `camera720.gprj`
- FPGA sources and pin/timing constraints: `src/camera720/`
- Build script: `tools/build_camera720.tcl`
- Flashable bitstream: `release/camera720_cam2_720p.fs`
- RK3588 receiver binary: `release/recv_rgb565_wayland`
- Wiring, programming, and receiver setup: `CAMERA720_CAM2_烧录说明.md`

The current FPGA project is the camera acquisition and streaming baseline. It does not yet include BMI088 acquisition, a softcore CPU, or an on-video OSD overlay.

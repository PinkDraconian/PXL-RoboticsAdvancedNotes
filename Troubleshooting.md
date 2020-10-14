---
title: Troubleshooting
created: '2020-10-01T08:51:53.659Z'
modified: '2020-10-13T12:42:08.987Z'
---

# Troubleshooting
- `VMware: vmw_ioctl_command error Invalid argument.`
  Fix by turning off OpenGL 3.3 by setting the environment variable `SVGA_VGPU10=0`.
  `export SVGA_VGPU10=0`

title: SDL2 Mail Library Instructions
---

This document will introduce how to install and demonstrate SDL2 Mail on Ubuntu.

{% note warn note %}

1. System version must be Ubuntu 20.04
2. Only run under framebuffer

{% endnote %}

## Install

1. Upgrade your system

```sh
$ sudo apt update
$ sudo apt upgrade
$ sudo reboot
```

2. Install Library

```sh
$ sudo apt install libsdl2-2.0-0 libsdl2-dev
```

## Demonstrate

1. Get source code

```sh
$ git clone https://github.com/libsdl-org/SDL
$ git checkout release-2.0.10
```

2. Compile source code

```sh
$ cd SDL/test
$ ./configure
$ make
```

3. Run

Check info 

```sh
$ ./testdisplayinfo 
NFO: See 1 displays.
INFO: 0: "0" (1920x1080, (0, 0)), 1 modes.
ERROR:     DPI: failed to query (That operation is not supported)
INFO: CURRENT: fmt=SDL_PIXELFORMAT_RGBX8888 w=1920 h=1080 refresh=60
INFO: DESKTOP: fmt=SDL_PIXELFORMAT_RGBX8888 w=1920 h=1080 refresh=60
INFO:     MODE 0: fmt=SDL_PIXELFORMAT_RGBX8888 w=1920 h=1080 refresh=60
INFO:
```

Run test demo

```sh
$ ./testgles2 
INFO: Screen bpp: 24
INFO: 
INFO: Vendor     : ARM
INFO: Renderer   : Mali-G52
INFO: Version    : OpenGL ES 3.2 git.c8adbf9.122c9daed32dbba4b3056f41a2f23c58
INFO: Extensions : GL_ARM_rgba8 GL_ARM_mali_shader_binary GL_OES_depth24 GL_OES_depth_texture GL_OES_depth_texture_cube_map GL_OES_packed_depth_stencil GL_OES_rgb8_rgba8 GL_EXT_read_format_bgra GL_OES_compressed_paletted_texture GL_OES_compressed_ETC1_RGB8_texture GL_OES_standard_derivatives GL_OES_EGL_image GL_OES_EGL_image_external GL_OES_EGL_image_external_essl3 GL_OES_EGL_sync GL_OES_texture_npot GL_OES_vertex_half_float GL_OES_required_internalformat GL_OES_vertex_array_object GL_OES_mapbuffer GL_EXT_texture_format_BGRA8888 GL_EXT_texture_rg GL_EXT_texture_type_2_10_10_10_REV GL_OES_fbo_render_mipmap GL_OES_element_index_uint GL_EXT_shadow_samplers GL_OES_texture_compression_astc GL_KHR_texture_compression_astc_ldr GL_KHR_texture_compression_astc_hdr GL_KHR_texture_compression_astc_sliced_3d GL_EXT_texture_compression_astc_decode_mode GL_EXT_texture_compression_astc_decode_mode_rgb9e5 GL_KHR_debug GL_EXT_occlusion_query_boolean GL_EXT_disjoint_timer_query GL_EXT_blend_minmax GL_EXT_discard_framebuffer GL_OES_get_program_binary GL_OES_texture_3D GL_EXT_texture_storage GL_EXT_multisampled_render_to_texture GL_OES_surfaceless_context GL_OES_texture_stencil8 GL_EXT_shader_pixel_local_storage GL_ARM_shader_framebuffer_fetch GL_ARM_shader_framebuffer_fetch_depth_stencil GL_ARM_mali_program_binary GL_EXT_sRGB GL_EXT_sRGB_write_control GL_EXT_texture_sRGB_decode GL_EXT_texture_sRGB_R8 GL_EXT_texture_sRGB_RG8 GL_KHR_blend_equation_advanced GL_KHR_blend_equation_advanced_coherent GL_OES_texture_storage_multisample_2d_array GL_OES_shader_image_atomic GL_EXT_robustness GL_EXT_draw_buffers_indexed GL_OES_draw_buffers_indexed GL_EXT_texture_border_clamp GL_OES_texture_border_clamp GL_EXT_texture_cube_map_array GL_OES_texture_cube_map_array GL_OES_sample_variables GL_OES_sample_shading GL_OES_shader_multisample_interpolation GL_EXT_shader_io_blocks GL_OES_shader_io_blocks GL_EXT_tessellation_shader GL_OES_tessellation_shader GL_EXT_primitive_bounding_box GL_OES_primitive_bounding_box GL_EXT_geometry_shader GL_OES_geometry_shader GL_ANDROID_extension_pack_es31a GL_EXT_gpu_shader5 GL_OES_gpu_shader5 GL_EXT_texture_buffer GL_OES_texture_buffer GL_EXT_copy_image GL_OES_copy_image GL_EXT_shader_non_constant_global_initializers GL_EXT_color_buffer_half_float GL_EXT_color_buffer_float GL_EXT_YUV_target GL_OVR_multiview GL_OVR_multiview2 GL_OVR_multiview_multisampled_render_to_texture GL_KHR_robustness GL_KHR_robust_buffer_access_behavior GL_EXT_draw_elements_base_vertex GL_OES_draw_elements_base_vertex GL_EXT_buffer_storage GL_EXT_texture_filter_anisotropic 
INFO: 
INFO: SDL_GL_RED_SIZE: requested 5, got 8
INFO: SDL_GL_GREEN_SIZE: requested 5, got 8
INFO: SDL_GL_BLUE_SIZE: requested 5, got 8
INFO: SDL_GL_DEPTH_SIZE: requested 16, got 24
```

When a rotating square appears on the screen, the operation is successful.
link_libraries(CVD)
project(progs)

if(CVD_HAVE_VIDEODISPLAY)
	add_executable(calibrate calibrate.cxx)
	add_executable(video_play_source video_play_source.cc)
	add_executable(cvd_display_image cvd_display_image.cxx)
	add_executable(cvd_image_viewer cvd_image_viewer.cxx)
endif()


if(CVD_HAVE_TOON)
	add_executable(se3_exp se3_exp.cxx)
	add_executable(se3_inv se3_inv.cxx)
	add_executable(se3_ln se3_ln.cxx)
	add_executable(se3_post_mul se3_post_mul.cxx)
	add_executable(se3_pre_mul se3_pre_mul.cxx)
endif()

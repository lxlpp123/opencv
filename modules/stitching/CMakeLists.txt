set(the_description "Images stitching")

if(HAVE_CUDA)
  ocv_warnings_disable(CMAKE_CXX_FLAGS -Wundef -Wmissing-declarations -Wshadow)
endif()

ocv_define_module(stitching opencv_imgproc opencv_features2d opencv_calib3d opencv_objdetect
                  OPTIONAL opencv_cuda opencv_cudaarithm opencv_cudafilters opencv_cudafeatures2d opencv_xfeatures2d)

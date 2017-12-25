
file(GLOB unetConsoleSources *.cpp)
file(GLOB unetConsoleIncludes *.h )

cuda_add_executable(unet-console ${unetConsoleSources})
target_link_libraries(unet-console nvcaffe_parser nvinfer medical-inference)

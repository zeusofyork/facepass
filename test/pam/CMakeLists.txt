# g++ -o pam_test main.cc -lpam -lpam_misc

add_executable(pam_test main.cc)
target_link_libraries(pam_test PRIVATE pam pam_misc facepass_cfg)
target_include_directories(pam_test PRIVATE 
    ${FaceConfig_INCLUDE_DIRS}
)

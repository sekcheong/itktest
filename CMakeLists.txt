cmake_minimum_required(VERSION 3.20)

project(itk_test)

include(ExternalProject)

ExternalProject_Add(ITK
    GIT_REPOSITORY
        https://github.com/InsightSoftwareConsortium/ITK.git
    GIT_TAG 
        v5.3.0
    CMAKE_ARGS 
        -DITK_SKIP_PATH_LENGTH_CHECKS=ON
)
# This is your project statement. You should always list languages;
# Listing the version is nice here since it sets lots of useful variables
cmake_minimum_required(VERSION 3.16)
project(NUMERICAL_LINEAR_ALGEBRA_BASE_PACKAGE C)

# If you set any CMAKE_ variables, that can go here.
# (But usually don't do this, except maybe for C++ standard)

set(PROJECT_INCLUDE_DIR ${PROJECT_SOURCE_DIR}/src/include)
add_library(${PROJECT_NAME} src/matrix.c src/vector.c)

include_directories(${PROJECT_INCLUDE_DIR})
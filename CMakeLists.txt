cmake_minimum_required(VERSION 3.10)
project(ng2)

set(CMAKE_CXX_STANDARD 11)

include_directories(node_modules)
include_directories(node_modules/nan)
include_directories(src)

add_executable(ng2
        node_modules/nan/nan.h
        node_modules/nan/nan_callbacks.h
        node_modules/nan/nan_callbacks_12_inl.h
        node_modules/nan/nan_callbacks_pre_12_inl.h
        node_modules/nan/nan_converters.h
        node_modules/nan/nan_converters_43_inl.h
        node_modules/nan/nan_converters_pre_43_inl.h
        node_modules/nan/nan_define_own_property_helper.h
        node_modules/nan/nan_implementation_12_inl.h
        node_modules/nan/nan_implementation_pre_12_inl.h
        node_modules/nan/nan_json.h
        node_modules/nan/nan_maybe_43_inl.h
        node_modules/nan/nan_maybe_pre_43_inl.h
        node_modules/nan/nan_new.h
        node_modules/nan/nan_object_wrap.h
        node_modules/nan/nan_persistent_12_inl.h
        node_modules/nan/nan_persistent_pre_12_inl.h
        node_modules/nan/nan_private.h
        node_modules/nan/nan_string_bytes.h
        node_modules/nan/nan_typedarray_contents.h
        node_modules/nan/nan_weak.h
        src/autodetect.cc
        src/binding.cc
        src/binding.h
        src/camera.cc
        src/camera.h
        src/camera_helpers.cc
        src/gphoto.cc
        src/gphoto.h)

cmake_minimum_required(VERSION 3.10.2)

add_library(sequence
        SHARED
        sequence.cpp
        sequence_model.cpp)

target_link_libraries(sequence

        # Link with libneuralnetworks.so for NN API
        neuralnetworks
        android
        log)

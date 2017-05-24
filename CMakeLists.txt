cmake_minimum_required(VERSION 3.5)


add_compile_options(-std=c++11)

find_library(live555 live555)

add_executable(FFmpegRTSPServer
	FFmpegDecoder.cpp
	FFmpegH264Source.cpp
	LiveServerMediaSubsession.cpp
	FFmpegH264Encoder.cpp
	LiveRTSPServer.cpp
	main.cpp)

cmake_minimum_required(VERSION 3.14)
project(shm_test VERSION 0.3.6 LANGUAGES CXX)
set(THREADS_PREFER_PTHREAD_FLAG ON)


include_directories("..")

add_executable(echo_server
        echo_server.cc)

add_executable(echo_client
        echo_client.cc)



target_link_libraries(echo_server PRIVATE
		pthread
        rt
        )
        

target_link_libraries(echo_client PRIVATE
		pthread
        rt
        )

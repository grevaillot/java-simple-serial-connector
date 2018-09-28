cmake_minimum_required(VERSION 3.4.1)

add_library( JSSCLib 
             SHARED
             src/main/cpp/_nix_based/jssc.cpp )

find_library( log-lib
              log )

target_link_libraries( JSSCLib
                       ${log-lib} )

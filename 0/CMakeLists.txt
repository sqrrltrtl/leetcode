cmake_minimum_required(VERSION 3.6)

file(GLOB sourceFiles RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} *.cpp)
foreach(oneSourceFile ${sourceFiles})
    string(REPLACE ".cpp" "" execName ${oneSourceFile})
    add_executable(${execName} ${oneSourceFile})
endforeach(oneSourceFile ${sourceFiles})

target_link_libraries(1_TwoSum printer)
target_link_libraries(15_3Sum printer)
target_link_libraries(26_RemoveDuplicatesFromSortedArray printer)
target_link_libraries(66_PlusOne printer)
target_link_libraries(75_SortColors printer)
target_link_libraries(77_Combinations printer)
target_link_libraries(80_RemoveDuplicatesFromSortedArrayII printer)

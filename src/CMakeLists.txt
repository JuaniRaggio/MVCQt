add_subdirectory(model)
add_subdirectory(view)
add_subdirectory(controller)

add_executable(QtMVCApp
    main.cpp
)

target_link_libraries(QtMVCApp
    Qt6::Widgets
    model
    view
    controller
)
target_include_directories(QtMVCApp PRIVATE ../include)

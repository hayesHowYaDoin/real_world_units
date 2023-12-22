find_package(GTest REQUIRED)

enable_testing()

add_executable(test_real_world_units
    example/test_example.cpp
)

target_link_libraries(test_real_world_units
    PUBLIC
        GTest::GTest
        GTest::Main
        Physics::Units
)

include(GoogleTest)
gtest_discover_tests(test_real_world_units)

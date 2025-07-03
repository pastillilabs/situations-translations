cmake_minimum_required(VERSION 3.27)

set(TARGET_NAME Translations)

project(${APP_NAME}${TARGET_NAME} LANGUAGES CXX)

file(GLOB TS_SOURCES CONFIGURE_DEPENDS src/*.ts)
add_custom_target(${PROJECT_NAME}
    SOURCES
        .gitignore
        AUTHORS
        LICENSE
        README.md
        ${TS_SOURCES}
)

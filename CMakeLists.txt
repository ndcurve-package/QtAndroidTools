qt_add_library(packages_QtAndroidTools STATIC)


include_directories(${CMAKE_CURRENT_LIST_DIR}/QtAndroidTools)

qt6_add_qml_module(packages_QtAndroidTools
    URI packages.QtAndroidTools
    VERSION 1.0
)

set(QTAT_APP_PERMISSIONS ON)
set(QTAT_APK_INFO ON)
set(QTAT_SCREEN ON)
set(QTAT_SYSTEM ON)
set(QTAT_BATTERY_STATE ON)
set(QTAT_SIGNAL_STRENGTH ON)
set(QTAT_IMAGES ON)
set(QTAT_NOTIFICATION ON)
set(QTAT_ADMOB_BANNER ON)
set(QTAT_ADMOB_INTERSTITIAL ON)
set(QTAT_ADMOB_REWARDED_AD ON)
set(QTAT_PLAY_STORE ON)
set(QTAT_GOOGLE_ACCOUNT ON)
set(QTAT_GOOGLE_DRIVE ON)
set(QTAT_SHARING ON)
set(QTAT_USER_MESSAGING_PLATFORM ON)
set(QTAT_AUDIO ON)

add_subdirectory(QtAndroidTools)
target_link_libraries(packages_QtAndroidTools PRIVATE QtAndroidTools)

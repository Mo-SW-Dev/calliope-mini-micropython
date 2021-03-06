# NOTE: This file is generated by yotta: changes will be overwritten!

cmake_minimum_required(VERSION 2.8.11)

include_directories("/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/source")


set(YOTTA_AUTO_BLE_CPP_FILES
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/source/services/URIBeaconConfigService.cpp"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/source/GapScanningParams.cpp"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/source/BLE.cpp"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/source/services/DFUService.cpp"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/source/DiscoveredCharacteristic.cpp"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/source/services/UARTService.cpp"
)
# force dependency on the config header for cpp files, which CMake otherwise wouldn't track:
set_property(SOURCE ${YOTTA_AUTO_BLE_CPP_FILES} PROPERTY OBJECT_DEPENDS "/home/ubuntu/Arbeitplatz/micropython/build/bbc-microbit-classic-gcc-nosd/yotta_config.h")
set(YOTTA_AUTO_BLE_HEADER_FILES
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GapAdvertisingParams.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/deprecate.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/SecurityManager.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GapScanningParams.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/URIBeaconConfigService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GattAttribute.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/DiscoveredService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/DeviceInformationService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/EddystoneService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GattService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/EddystoneConfigService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/DiscoveredCharacteristicDescriptor.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GattServerEvents.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GattServer.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GapAdvertisingData.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/HealthThermometerService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/DFUService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/iBeacon.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GapEvents.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/EnvironmentalService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GattCharacteristic.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/CharacteristicDescriptorDiscovery.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/CallChainOfFunctionPointersWithContext.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/ServiceDiscovery.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GattClient.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/Gap.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/BLEProtocol.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/UARTService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/UUID.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/FunctionPointerWithContext.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/LinkLossService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/DiscoveredCharacteristic.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/BLEInstanceBase.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/blecommon.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/SafeBool.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/BatteryService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/BLE.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/services/HeartRateService.h"
    "/home/ubuntu/Arbeitplatz/micropython/yotta_modules/ble/ble/GattCallbackParamTypes.h"
)
# force dependency on the config header for header files, which CMake otherwise wouldn't track:
set_property(SOURCE ${YOTTA_AUTO_BLE_HEADER_FILES} PROPERTY OBJECT_DEPENDS "/home/ubuntu/Arbeitplatz/micropython/build/bbc-microbit-classic-gcc-nosd/yotta_config.h")


add_library(ble
    ${YOTTA_AUTO_BLE_CPP_FILES}
    ${YOTTA_AUTO_BLE_HEADER_FILES}
)

yotta_postprocess_target(LIBRARY ble)



target_link_libraries(ble
    ble-nrf51822
    mbed-classic
)


PROJECT_NAME     := lora_s132
TARGETS          := nrf52832_xxaa
OUTPUT_DIRECTORY := _build

#SDK_ROOT := /opt/Nordic/nRF5_SDK_14.2.0_17b948a
SDK_ROOT := ../nRF_Lib
PROJ_DIR := .

$(OUTPUT_DIRECTORY)/nrf52832_xxaa.out: \
  LINKER_SCRIPT  := ble_gcc_nrf52.ld

SRC_FILES += $(PROJ_DIR)/../Apps/LoRaWAN_Demo/main.c $(PROJ_DIR)/../Apps/LoRaWAN_Demo/app_lora.c
#SRC_FILES += $(PROJ_DIR)/../Apps/Scan_Demo/main.c $(PROJ_DIR)/../Apps/Scan_Demo/app_lora.c
#SRC_FILES += $(PROJ_DIR)/../Apps/Receiver/main.c $(PROJ_DIR)/../Apps/Receiver/app_lora.c
#SRC_FILES += $(PROJ_DIR)/../Apps/Peripherals_Demo/main.c $(PROJ_DIR)/../Apps/Peripherals_Demo/app_lora.c

SRC_FILES += \
  $(SDK_ROOT)/components/boards/boards.c \
  $(SDK_ROOT)/components/libraries/bsp/bsp.c \
  $(SDK_ROOT)/components/libraries/bsp/bsp_btn_ble.c \
  $(SDK_ROOT)/components/libraries/bsp/bsp_nfc.c \
  $(SDK_ROOT)/components/toolchain/gcc/gcc_startup_nrf52.S \
  $(SDK_ROOT)/components/toolchain/system_nrf52.c \
  $(PROJ_DIR)/../Board/lora_board/board.c \
  $(PROJ_DIR)/../Board/lora_board/gpio-board.c \
  $(PROJ_DIR)/../Board/lora_board/rtc-board.c \
  $(PROJ_DIR)/../Board/lora_board/spi-board.c \
  $(PROJ_DIR)/../Board/lora_board/sx1276-board.c \
  $(PROJ_DIR)/../Board/lora_board/timer.c \
  $(PROJ_DIR)/../Board/lora_board/utilities.c \
  $(PROJ_DIR)/../Board/lora_board/utils.c \
  $(PROJ_DIR)/../Board/peripherals/rak_spi_drv.c \
  $(PROJ_DIR)/../Board/peripherals/lis3dh_driver.c \
  $(PROJ_DIR)/../Board/peripherals/rak_i2c_drv.c \
  $(PROJ_DIR)/../Board/peripherals/rak_i2c_gps_max7.c \
  $(PROJ_DIR)/../Board/peripherals/rak_i2c_lis3dh.c \
  $(PROJ_DIR)/../Board/peripherals/rak_i2c_oled.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/LoRaMac.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/LoRaMacCrypto.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/Region.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionAS923.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionAU915.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionCommon.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionEU868.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionIN865.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionKR920.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionUS915.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionUS915-Hybrid.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionCN470.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionCN779.c \
  $(PROJ_DIR)/../LoRa_Lib/mac/region/RegionEU433.c \
  $(PROJ_DIR)/../LoRa_Lib/radio/sx1276/sx1276.c \
  $(PROJ_DIR)/../LoRa_Lib/system/crypto/aes.c \
  $(PROJ_DIR)/../LoRa_Lib/system/crypto/cmac.c \
  $(PROJ_DIR)/../LoRa_Lib/system/gps.c \
  $(SDK_ROOT)/components/ble/ble_advertising/ble_advertising.c \
  $(SDK_ROOT)/components/ble/common/ble_advdata.c \
  $(SDK_ROOT)/components/ble/common/ble_conn_params.c \
  $(SDK_ROOT)/components/ble/common/ble_conn_state.c \
  $(SDK_ROOT)/components/ble/common/ble_srv_common.c \
  $(SDK_ROOT)/components/ble/nrf_ble_gatt/nrf_ble_gatt.c \
  $(SDK_ROOT)/components/ble/peer_manager/gatt_cache_manager.c \
  $(SDK_ROOT)/components/ble/peer_manager/gatts_cache_manager.c \
  $(SDK_ROOT)/components/ble/peer_manager/id_manager.c \
  $(SDK_ROOT)/components/ble/peer_manager/peer_data_storage.c \
  $(SDK_ROOT)/components/ble/peer_manager/peer_database.c \
  $(SDK_ROOT)/components/ble/peer_manager/peer_id.c \
  $(SDK_ROOT)/components/ble/peer_manager/peer_manager.c \
  $(SDK_ROOT)/components/ble/peer_manager/pm_buffer.c \
  $(SDK_ROOT)/components/ble/peer_manager/pm_mutex.c \
  $(SDK_ROOT)/components/ble/peer_manager/security_dispatcher.c \
  $(SDK_ROOT)/components/ble/peer_manager/security_manager.c \
  $(SDK_ROOT)/components/ble/ble_services/ble_nus/ble_nus.c \
  $(SDK_ROOT)/components/ble/ble_db_discovery/ble_db_discovery.c \
  $(SDK_ROOT)/components/drivers_nrf/clock/nrf_drv_clock.c \
  $(SDK_ROOT)/components/drivers_nrf/common/nrf_drv_common.c \
  $(SDK_ROOT)/components/drivers_nrf/gpiote/nrf_drv_gpiote.c \
  $(SDK_ROOT)/components/drivers_nrf/rtc/nrf_drv_rtc.c \
  $(SDK_ROOT)/components/drivers_nrf/spi_master/nrf_drv_spi.c \
  $(SDK_ROOT)/components/drivers_nrf/twi_master/nrf_drv_twi.c \
  $(SDK_ROOT)/components/drivers_nrf/uart/nrf_drv_uart.c \
  $(SDK_ROOT)/components/libraries/button/app_button.c \
  $(SDK_ROOT)/components/libraries/fifo/app_fifo.c \
  $(SDK_ROOT)/components/libraries/fstorage/nrf_fstorage.c \
  $(SDK_ROOT)/components/libraries/fstorage/nrf_fstorage_sd.c \
  $(SDK_ROOT)/components/libraries/fds/fds.c \
  $(SDK_ROOT)/components/libraries/uart/app_uart_fifo.c \
  $(SDK_ROOT)/components/libraries/strerror/nrf_strerror.c \
  $(SDK_ROOT)/components/libraries/experimental_section_vars/nrf_section_iter.c \
  $(SDK_ROOT)/components/libraries/experimental_memobj/nrf_memobj.c \
  $(SDK_ROOT)/components/libraries/atomic_fifo/nrf_atfifo.c \
  $(SDK_ROOT)/components/libraries/balloc/nrf_balloc.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf_format.c \
  $(SDK_ROOT)/components/libraries/util/app_error.c \
  $(SDK_ROOT)/components/libraries/util/app_error_weak.c \
  $(SDK_ROOT)/components/libraries/util/app_util_platform.c \
  $(SDK_ROOT)/components/libraries/util/sdk_mapped_flags.c \
  $(SDK_ROOT)/components/libraries/uart/retarget.c \
  $(SDK_ROOT)/components/libraries/pwr_mgmt/nrf_pwr_mgmt.c \
  $(SDK_ROOT)/components/libraries/util/nrf_assert.c \
  $(SDK_ROOT)/components/libraries/timer/app_timer.c \
  $(SDK_ROOT)/components/libraries/scheduler/app_scheduler.c \
  $(SDK_ROOT)/components/libraries/experimental_log/src/nrf_log_default_backends.c \
  $(SDK_ROOT)/components/libraries/experimental_log/src/nrf_log_frontend.c \
  $(SDK_ROOT)/components/libraries/experimental_log/src/nrf_log_str_formatter.c \
  $(SDK_ROOT)/components/libraries/experimental_log/src/nrf_log_backend_rtt.c \
  $(SDK_ROOT)/components/libraries/experimental_log/src/nrf_log_backend_serial.c \
  $(SDK_ROOT)/external/segger_rtt/SEGGER_RTT.c \
  $(SDK_ROOT)/external/segger_rtt/SEGGER_RTT_printf.c \
  $(SDK_ROOT)/external/segger_rtt/SEGGER_RTT_Syscalls_KEIL.c \
  $(SDK_ROOT)/components/softdevice/common/nrf_sdh_soc.c \
  $(SDK_ROOT)/components/softdevice/common/nrf_sdh.c \
  $(SDK_ROOT)/components/softdevice/common/nrf_sdh_ble.c
  
# Include folders common to all targets
INC_FOLDERS += \
  . \
  $(PROJ_DIR)/../Apps \
  $(PROJ_DIR)/../Board \
  $(PROJ_DIR)/../Board/lora_board \
  $(PROJ_DIR)/../Board/peripherals \
  $(PROJ_DIR)/../LoRa_Lib/mac \
  $(PROJ_DIR)/../LoRa_Lib/mac/region \
  $(PROJ_DIR)/../LoRa_Lib/radio \
  $(PROJ_DIR)/../LoRa_Lib/radio/sx1276 \
  $(PROJ_DIR)/../LoRa_Lib/system \
  $(PROJ_DIR)/../LoRa_Lib/system/crypto \
  $(SDK_ROOT)/external/fprintf \
  $(SDK_ROOT)/external/segger_rtt \
  $(SDK_ROOT)/components/boards \
  $(SDK_ROOT)/components/toolchain/cmsis/include \
  $(SDK_ROOT)/components/device \
  $(SDK_ROOT)/components/ble/ble_services/ble_nus \
  $(SDK_ROOT)/components/toolchain \
  $(SDK_ROOT)/components/softdevice/common \
  $(SDK_ROOT)/components/softdevice/s132/headers \
  $(SDK_ROOT)/components/softdevice/s132/headers/nrf52 \
  $(SDK_ROOT)/components/drivers_nrf/clock \
  $(SDK_ROOT)/components/drivers_nrf/common \
  $(SDK_ROOT)/components/drivers_nrf/gpiote \
  $(SDK_ROOT)/components/drivers_nrf/rtc \
  $(SDK_ROOT)/components/drivers_nrf/spi_master \
  $(SDK_ROOT)/components/drivers_nrf/timer \
  $(SDK_ROOT)/components/drivers_nrf/uart \
  $(SDK_ROOT)/components/drivers_nrf/twi_master \
  $(SDK_ROOT)/components/libraries/balloc \
  $(SDK_ROOT)/components/libraries/bsp \
  $(SDK_ROOT)/components/libraries/util \
  $(SDK_ROOT)/components/libraries/button \
  $(SDK_ROOT)/components/libraries/experimental_log \
  $(SDK_ROOT)/components/libraries/experimental_memobj \
  $(SDK_ROOT)/components/libraries/fds \
  $(SDK_ROOT)/components/libraries/fifo \
  $(SDK_ROOT)/components/libraries/fstorage \
  $(SDK_ROOT)/components/libraries/uart \
  $(SDK_ROOT)/components/libraries/experimental_section_vars \
  $(SDK_ROOT)/components/drivers_nrf/hal \
  $(SDK_ROOT)/components/libraries/strerror \
  $(SDK_ROOT)/components/libraries/experimental_log/src \
  $(SDK_ROOT)/components/libraries/timer \
  $(SDK_ROOT)/components/drivers_nrf/delay \
  $(SDK_ROOT)/components/libraries/atomic \
  $(SDK_ROOT)/components/libraries/pwr_mgmt \
  $(SDK_ROOT)/components/ble/common \
  $(SDK_ROOT)/components/libraries/mutex \
  $(SDK_ROOT)/components/ble/ble_advertising \
  $(SDK_ROOT)/components/drivers_nrf/wdt \
  $(SDK_ROOT)/components/ble/nrf_ble_gatt \
  $(SDK_ROOT)/components/libraries/mem_manager \
  $(SDK_ROOT)/components/ble/ble_db_discovery \
  $(SDK_ROOT)/components/ble/peer_manager \
  $(SDK_ROOT)/components/libraries/atomic_fifo
  
# Libraries common to all targets
LIB_FILES += \

# Optimization flags
#OPT = -O3 -g3
OPT =  -g3
# Uncomment the line below to enable link time optimization
#OPT += -flto

# C flags common to all targets
CFLAGS += $(OPT)
CFLAGS += -DREGION_EU868
CFLAGS += -DBOARD_CUSTOM
CFLAGS += -DUSE_APP_CONFIG
CFLAGS += -DCONFIG_GPIO_AS_PINRESET
CFLAGS += -DFLOAT_ABI_HARD
CFLAGS += -DBL_SETTINGS_ACCESS_ONLY
CFLAGS += -DNRF52
CFLAGS += -DNRF52832_XXAA
CFLAGS += -DNRF52_PAN_74
CFLAGS += -DNRF_SD_BLE_API_VERSION=5
CFLAGS += -DS132
CFLAGS += -DSOFTDEVICE_PRESENT
CFLAGS += -DSWI_DISABLE0
CFLAGS += -mcpu=cortex-m4
CFLAGS += -mthumb -mabi=aapcs
CFLAGS +=  -Wall
#CFLAGS +=  -Wall -Werror
CFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# keep every function in a separate section, this allows linker to discard unused ones
CFLAGS += -ffunction-sections -fdata-sections -fno-strict-aliasing
CFLAGS += -fno-builtin -fshort-enums 

# C++ flags common to all targets
CXXFLAGS += $(OPT)

# Assembler flags common to all targets
ASMFLAGS += -g3
ASMFLAGS += -mcpu=cortex-m4
ASMFLAGS += -mthumb -mabi=aapcs
ASMFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
ASMFLAGS += -DBOARD_CUSTOM
ASMFLAGS += -DCONFIG_GPIO_AS_PINRESET
ASMFLAGS += -DFLOAT_ABI_HARD
ASMFLAGS += -DNRF52
ASMFLAGS += -DNRF52832_XXAA
ASMFLAGS += -DNRF52_PAN_74
ASMFLAGS += -DNRF_SD_BLE_API_VERSION=5
ASMFLAGS += -DS132
ASMFLAGS += -DSOFTDEVICE_PRESENT
ASMFLAGS += -DSWI_DISABLE0

# Linker flags
LDFLAGS += $(OPT)
LDFLAGS += -mthumb -mabi=aapcs -L $(TEMPLATE_PATH) -T$(LINKER_SCRIPT)
LDFLAGS += -mcpu=cortex-m4
LDFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# let linker dump unused sections
LDFLAGS += -Wl,--gc-sections
# use newlib in nano version
LDFLAGS += --specs=nano.specs


# Add standard libraries at the very end of the linker input, after all objects
# that may need symbols provided by these libraries.
LIB_FILES += -lc -lnosys -lm


.PHONY: default help lora_set lora

# Default target - first one defined
default: nrf52832_xxaa


# Print all targets that can be built
help:
	@echo following targets are available:
	@echo		nrf52832_xxaa
	@echo		flash_softdevice
	@echo		sdk_config - starting external tool for editing sdk_config.h
	@echo		flash      - flashing binary

lora:	SRC_APP = $(PROJ_DIR)/../Apps/LoRaWAN_Demo/app_lora.c
lora:	SRC_APP += $(PROJ_DIR)/../Apps/LoRaWAN_Demo/main.c
lora:	SRC_FILES += $(SRC_APP) $(SRC_BODY)
lora:	$(foreach target, $(TARGETS), $(call define_target, $(target)))
#lora:	$(call prepare_build, $(TARGETS), $(OUTPUT_FILE).inc, $(OUTPUT_FILE).out)
#lora:	lora_set
lora:	default

lora_set:
	echo $(SRC_FILES)

TEMPLATE_PATH := $(SDK_ROOT)/components/toolchain/gcc


include $(TEMPLATE_PATH)/Makefile.common

$(foreach target, $(TARGETS), $(call define_target, $(target)))

.PHONY: flash flash_softdevice erase

# Flash the program
flash: $(OUTPUT_DIRECTORY)/nrf52832_xxaa.hex
	@echo Flashing: $<
	nrfjprog -f nrf52 --program $< --sectorerase
	nrfjprog -f nrf52 --reset

# Flash softdevice
flash_softdevice:
	@echo Flashing: s132_nrf52_5.0.0_softdevice.hex
	nrfjprog -f nrf52 --program $(SDK_ROOT)/components/softdevice/s132/hex/s132_nrf52_5.0.0_softdevice.hex --sectorerase
	nrfjprog -f nrf52 --reset

erase:
	nrfjprog -f nrf52 --eraseall

SDK_CONFIG_FILE := ../config/sdk_config.h
CMSIS_CONFIG_TOOL := $(SDK_ROOT)/external_tools/cmsisconfig/CMSIS_Configuration_Wizard.jar
sdk_config:
	java -jar $(CMSIS_CONFIG_TOOL) $(SDK_CONFIG_FILE)

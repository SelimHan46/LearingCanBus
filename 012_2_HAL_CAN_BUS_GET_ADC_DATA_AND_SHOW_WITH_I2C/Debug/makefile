################################################################################
# Automatically-generated file. Do not edit!
# Toolchain: GNU Tools for STM32 (10.3-2021.10)
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F4xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

OPTIONAL_TOOL_DEPS := \
$(wildcard ../makefile.defs) \
$(wildcard ../makefile.init) \
$(wildcard ../makefile.targets) \


BUILD_ARTIFACT_NAME := 012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C
BUILD_ARTIFACT_EXTENSION := elf
BUILD_ARTIFACT_PREFIX :=
BUILD_ARTIFACT := $(BUILD_ARTIFACT_PREFIX)$(BUILD_ARTIFACT_NAME)$(if $(BUILD_ARTIFACT_EXTENSION),.$(BUILD_ARTIFACT_EXTENSION),)

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.elf \

MAP_FILES += \
012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.map \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.list \


# All Target
all: main-build

# Main-build Target
main-build: 012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.elf secondary-outputs

# Tool invocations
012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.elf 012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.map: $(OBJS) $(USER_OBJS) C:\Users\90543\Desktop\Driver\canbus\012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C\STM32F407VGTX_FLASH.ld makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-gcc -o "012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m4 -T"C:\Users\90543\Desktop\Driver\canbus\012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C\STM32F407VGTX_FLASH.ld" --specs=nosys.specs -Wl,-Map="012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.map" -Wl,--gc-sections -static --specs=nano.specs -mfpu=fpv4-sp-d16 -mfloat-abi=hard -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.list: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.list"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) 012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.elf 012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.list 012_2_HAL_CAN_BUS_GET_ADC_DATA_AND_SHOW_WITH_I2C.map default.size.stdout
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST)

fail-specified-linker-script-missing:
	@echo 'Error: Cannot find the specified linker script. Check the linker settings in the build configuration.'
	@exit 2

warn-no-linker-script-specified:
	@echo 'Warning: No linker script specified. Check the linker settings in the build configuration.'

.PHONY: all clean dependents main-build fail-specified-linker-script-missing warn-no-linker-script-specified

-include ../makefile.targets

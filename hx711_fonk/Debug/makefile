################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Startup/subdir.mk
-include Src/subdir.mk
-include Drivers/STM32F1xx_HAL_Driver/Src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
hx711_fonk.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
hx711_fonk.list \

OBJCOPY_HEX += \
hx711_fonk.hex \

OBJCOPY_BIN += \
hx711_fonk.bin \


# All Target
all: hx711_fonk.elf secondary-outputs

# Tool invocations
hx711_fonk.elf: $(OBJS) $(USER_OBJS) C:\Users\F\Desktop\stm_ex\hx711_fonk\STM32F103C8TX_FLASH.ld
	arm-none-eabi-gcc -o "hx711_fonk.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\F\Desktop\stm_ex\hx711_fonk\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="hx711_fonk.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

hx711_fonk.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "hx711_fonk.list"
	@echo 'Finished building: $@'
	@echo ' '

hx711_fonk.hex: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O ihex $(EXECUTABLES) "hx711_fonk.hex"
	@echo 'Finished building: $@'
	@echo ' '

hx711_fonk.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "hx711_fonk.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_HEX) $(OBJCOPY_BIN)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets

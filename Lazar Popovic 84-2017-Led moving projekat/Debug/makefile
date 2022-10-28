################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F1xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
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
Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.list \

OBJCOPY_HEX += \
Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.hex \

OBJCOPY_BIN += \
Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.bin \


# All Target
all: Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.elf secondary-outputs

# Tool invocations
Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.elf: $(OBJS) $(USER_OBJS) C:\Users\Lazar\Desktop\Led\ moving\ projekat\Lazar\ Popovic\ 84-2017-Led\ moving\ projekat\STM32F103C6UX_FLASH.ld
	arm-none-eabi-gcc -o "Lazar Popovic 84-2017-Led moving projekat.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\Lazar\Desktop\Led moving projekat\Lazar Popovic 84-2017-Led moving projekat\STM32F103C6UX_FLASH.ld" --specs=nosys.specs -Wl,-Map="Lazar Popovic 84-2017-Led moving projekat.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "Lazar Popovic 84-2017-Led moving projekat.list"
	@echo 'Finished building: $@'
	@echo ' '

Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.hex: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O ihex $(EXECUTABLES) "Lazar Popovic 84-2017-Led moving projekat.hex"
	@echo 'Finished building: $@'
	@echo ' '

Lazar\ Popovic\ 84-2017-Led\ moving\ projekat.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "Lazar Popovic 84-2017-Led moving projekat.bin"
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

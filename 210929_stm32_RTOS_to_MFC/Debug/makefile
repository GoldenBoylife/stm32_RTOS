################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Middlewares/Third_Party/FreeRTOS/Source/portable/MemMang/subdir.mk
-include Middlewares/Third_Party/FreeRTOS/Source/portable/GCC/ARM_CM4F/subdir.mk
-include Middlewares/Third_Party/FreeRTOS/Source/CMSIS_RTOS_V2/subdir.mk
-include Middlewares/Third_Party/FreeRTOS/Source/subdir.mk
-include Drivers/STM32F4xx_HAL_Driver/Src/subdir.mk
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
210929_stm32_RTOS_to_MFC.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
210929_stm32_RTOS_to_MFC.list \

OBJCOPY_BIN += \
210929_stm32_RTOS_to_MFC.bin \


# All Target
all: 210929_stm32_RTOS_to_MFC.elf secondary-outputs

# Tool invocations
210929_stm32_RTOS_to_MFC.elf: $(OBJS) $(USER_OBJS) C:\Users\hwido\Documents\stm32_RTOS_to_MFC\210929_stm32_RTOS_to_MFC\STM32F429ZITX_FLASH.ld
	arm-none-eabi-gcc -o "210929_stm32_RTOS_to_MFC.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m4 -T"C:\Users\hwido\Documents\stm32_RTOS_to_MFC\210929_stm32_RTOS_to_MFC\STM32F429ZITX_FLASH.ld" --specs=nosys.specs -Wl,-Map="210929_stm32_RTOS_to_MFC.map" -Wl,--gc-sections -static --specs=nano.specs -mfpu=fpv4-sp-d16 -mfloat-abi=hard -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

210929_stm32_RTOS_to_MFC.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "210929_stm32_RTOS_to_MFC.list"
	@echo 'Finished building: $@'
	@echo ' '

210929_stm32_RTOS_to_MFC.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "210929_stm32_RTOS_to_MFC.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_BIN)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets

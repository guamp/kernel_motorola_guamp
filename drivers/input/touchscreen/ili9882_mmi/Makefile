ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI_ENABLE_DOUBLE_TAP)),)
	ccflags-y += -DILI_SENSOR_EN
endif
ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI_PANEL_NOTIFICATIONS)),)
	ccflags-y += -DILI_CONFIG_PANEL_NOTIFICATIONS
endif
ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI_RESUME_BY_DDI)),)
	ccflags-y += -DILI_CONFIG_RESUME_BY_DDI
endif
ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI_FW_PANEL)),)
	ccflags-y += -DILI_FW_PANEL
endif
ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI_ESD)),)
	ccflags-y += -DILI_CONFIG_ESD
endif
ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI_GESTURE)),)
	ccflags-y += -DILI_CONFIG_GESTURE
endif
ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI_PANEL_GESTURE)),)
	ccflags-y += -DILI_CONFIG_PANEL_GESTURE
endif

ili9882_mmi-objs += ili9882.o
ili9882_mmi-objs += ili9882_spi.o
ili9882_mmi-objs += ili9882_qcom.o
ili9882_mmi-objs += ili9882_ic.o
ili9882_mmi-objs += ili9882_touch.o
ili9882_mmi-objs += ili9882_mp.o
ili9882_mmi-objs += ili9882_hostdl.o
ili9882_mmi-objs += ili9882_node.o

obj-$(CONFIG_INPUT_TOUCHSCREEN_ILI_9882_MMI) += ili9882_mmi.o

# Copyright (c) 2013 The Linux Foundation. All rights reserved.
#
include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=ipq806x
BOARDNAME:=Qualcomm Atheros IPQ806X
FEATURES:=squashfs fpu ramdisk
CPU_TYPE:=cortex-a15
CPU_SUBTYPE:=neon-vfpv4
SUBTARGETS:=generic chromium

KERNEL_PATCHVER:=5.15

KERNELNAME:=zImage Image dtbs

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-leds-gpio kmod-gpio-button-hotplug swconfig \
	kmod-ata-ahci kmod-ata-ahci-platform \
	kmod-usb-ohci kmod-usb2 kmod-usb-ledtrig-usbport \
	kmod-phy-qcom-ipq806x-usb kmod-usb3 kmod-usb-dwc3-qcom \
	kmod-ath10k-ct wpad-openssl \
	uboot-envtools

$(eval $(call BuildTarget))

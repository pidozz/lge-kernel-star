#
# linux/arch/arm/vfp/Makefile
#
# Copyright (C) 2001 ARM Limited
#

# ccflags-y := -DDEBUG
# asflags-y := -DDEBUG

KBUILD_AFLAGS	:=$(KBUILD_AFLAGS:$(call as-option,-Wa$(comma)-mfloat-abi=softfp,-Wa$(comma)-msoft-float) -Wa,-mfpu=vfpv3-d16)
LDFLAGS		+=--no-warn-mismatch

obj-y			+= vfp.o

vfp-$(CONFIG_VFP)	+= vfpmodule.o entry.o vfphw.o vfpsingle.o vfpdouble.o

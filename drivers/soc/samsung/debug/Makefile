#
#  Makefile for Exynos-Debug
#

obj-$(CONFIG_DEBUG_SNAPSHOT) 		:= dss.o
dss-y 					+= debug-snapshot.o \
						debug-snapshot-log.o\
						debug-snapshot-utils.o \
						debug-snapshot-dpm.o
obj-$(CONFIG_DEBUG_SNAPSHOT_SFRDUMP)	+= debug-snapshot-sfrdump.o
obj-$(CONFIG_DEBUG_SNAPSHOT_QUICKDUMP)	+= debug-snapshot-qd.o

obj-$(CONFIG_EXYNOS_DEBUG_TEST)         += exynos-debug-test.o

ifeq ($(CONFIG_SOC_EXYNOS9110),y)
obj-$(CONFIG_EXYNOS_ITMON) += exynos9110-itmon.o
endif
ifeq ($(CONFIG_SOC_EXYNOS9810),y)
obj-$(CONFIG_EXYNOS_ITMON)              += exynos9810-itmon.o
endif

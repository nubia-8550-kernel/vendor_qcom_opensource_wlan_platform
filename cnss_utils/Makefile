# SPDX-License-Identifier: GPL-2.0-only

ccflags-y += -Wmissing-prototypes

ifeq ($(CONFIG_CNSS_OUT_OF_TREE),y)
ccflags-y += -I$(WLAN_PLATFORM_ROOT)/inc
endif

obj-$(CONFIG_CNSS_UTILS) += cnss_utils.o

obj-$(CONFIG_CNSS_QMI_SVC) += wlan_firmware_service.o
wlan_firmware_service-y := wlan_firmware_service_v01.o device_management_service_v01.o ip_multimedia_subsystem_private_service_v01.o

obj-$(CONFIG_CNSS_PLAT_IPC_QMI_SVC) += cnss_plat_ipc_qmi_svc.o
cnss_plat_ipc_qmi_svc-y := cnss_plat_ipc_qmi.o cnss_plat_ipc_service_v01.o

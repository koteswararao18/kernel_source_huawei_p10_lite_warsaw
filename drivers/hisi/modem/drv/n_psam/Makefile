-include $(srctree)/drivers/hisi/modem/config/product/$(OBB_PRODUCT_NAME)/config/balong_product_config.mk
obj-$(CONFIG_PSAM_SUPPORT)           += psam_balong.o

ifeq ($(strip $(CFG_CONFIG_MODULE_BUSSTRESS)),YES)
obj-$(CONFIG_PSAM_SUPPORT) 		     += psam_balong_test.o
else
obj-$(CONFIG_ENABLE_TEST_CODE)       += psam_balong_test.o
endif

ifeq ($(strip $(llt_gcov)),y)
GCOV_PROFILE_psam_balong.o := y
endif


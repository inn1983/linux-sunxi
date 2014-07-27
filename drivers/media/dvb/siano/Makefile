
smsmdtv-objs := smscoreapi.o sms-cards.o smsendian.o
smsdvb-objs := smsdvb-main.o

obj-$(CONFIG_SMS_SIANO_MDTV) += smsmdtv.o smsdvb.o
obj-$(CONFIG_SMS_USB_DRV) += smsusb.o

ifeq ($(CONFIG_SMS_SIANO_DEBUGFS),y)
  smsdvb-objs += smsdvb-debugfs.o
endif

ccflags-y += -Idrivers/media/dvb/dvb-core

ccflags-y += $(extra-cflags-y) $(extra-cflags-m)


#
# Makefile for ALSA
#
#
#
# RDD - HACKS!
HOST_CFLAGS += -Wno-array-bounds
KBUILD_CFLAGS += -Wno-array-bounds
CFLAGS_KERNEL += -Wno-array-bounds
CFLAGS_MODULE += -Wno-array-bounds

snd-usb-audio-objs := 	card.o \
			clock.o \
			endpoint.o \
			format.o \
			helper.o \
			mixer.o \
			mixer_quirks.o \
			pcm.o \
			proc.o \
			quirks.o \
			stream.o

snd-usbmidi-lib-objs := midi.o

# Toplevel Module Dependency
obj-$(CONFIG_SND_USB_AUDIO) += snd-usb-audio.o snd-usbmidi-lib.o

obj-$(CONFIG_SND_USB_UA101) += snd-usbmidi-lib.o
obj-$(CONFIG_SND_USB_USX2Y) += snd-usbmidi-lib.o
obj-$(CONFIG_SND_USB_US122L) += snd-usbmidi-lib.o

obj-$(CONFIG_SND) += misc/ usx2y/ caiaq/ 6fire/

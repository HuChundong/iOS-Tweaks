TARGET := iphone:clang:14.4:13.0
INSTALL_TARGET_PROCESSES = Gympass
GO_EASY_ON_ME = 1

ifeq ($(DEBUG),1)
THEOS_PACKAGE_DIR_NAME = ../../../var/www/repo.lillieweeb001/beta/debs
else
THEOS_PACKAGE_DIR_NAME = ../../../var/www/repo.lillieweeb001/debs
endif

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = GympassJBBypass
GympassJBBypass_FILES = Tweak.xm
GympassJBBypass_CFLAGS = -fobjc-arc
GympassJBBypass_FRAMEWORKS = UIKit Foundation
ARCHS = arm64 arm64e

include $(THEOS_MAKE_PATH)/tweak.mk
include $(THEOS_MAKE_PATH)/aggregate.mk

ARCHS ?= arm64 arm64e
TARGET ?= iphone:clang:15.5:13.0

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = ExampleModule
ExampleModule_BUNDLE_EXTENSION = bundle
ExampleModule_FILES = ExampleModule.m
ExampleModule_CFLAGS = -fobjc-arc
ExampleModule_LDFLAGS = -rpath /Library/Frameworks -rpath /var/jb/Library/Frameworks -rpath /usr/lib -rpath /var/jb/usr/lib
ExampleModule_INSTALL_PATH = /Library/Modulous/Modules

include $(THEOS_MAKE_PATH)/bundle.mk

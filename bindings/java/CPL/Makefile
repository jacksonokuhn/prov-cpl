#
# Core Provenance Library
#
# Copyright (c) Peter Macko
#

ROOT := ../../..


#
# Customize the build
#

INSTALL := yes

CPL_VERSION := $(shell cat "$(ROOT)/include/cpl.h" \
	| grep 'define CPL_VERSION_STR' \
	| sed 's/^[^0-9]*//g' | sed 's/"//g' | head -n 1)

MAVEN_INSTALL := yes
MAVEN_GROUP_ID := edu.harvard.pass
PROJECT_VERSION := $(CPL_VERSION)



JAVA_MODULE_DEPENDECIES := ../CPLDirect

#
# Include the magic script
#

include $(ROOT)/make/java-module.mk


# Autogenerated makefile for ViconDataStreamSDK_CPPRetimerTest

ifndef VERBOSE
.SILENT :
endif
.SUFFIXES :

ifdef CONFIG
ifneq ($(CONFIG), Debug)
ifneq ($(CONFIG), InternalRelease)
ifneq ($(CONFIG), Release)
Error: unknown configuration.
endif
endif
endif
else
CONFIG=Debug
endif

ifeq ($(CONFIG), Debug)
DEFINES=-DTCM_LINUX -DTCM_UNIX -D_DEBUG -DPROJECT_SOURCE_PATH=\".\" 
SYSTEMINCLUDEPATHS=-isystem../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/include 
INCLUDEPATHS=-I. -I../.. -I.. -I../ViconDataStreamSDK_CPP -I. -IDebug 
LIBRARYPATHS=-L../../../../lib/Debug -L../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/lib  -L../../../../bin/Debug
LIBRARIES=-lboost_atomic -lboost_chrono -lboost_container -lboost_context -lboost_coroutine -lboost_date_time -lboost_filesystem -lboost_graph -lboost_iostreams -lboost_locale -lboost_log -lboost_log_setup -lboost_math_c99 -lboost_math_c99f -lboost_math_c99l -lboost_math_tr1 -lboost_math_tr1f -lboost_math_tr1l -lboost_prg_exec_monitor -lboost_program_options -lboost_python3 -lboost_random -lboost_regex -lboost_serialization  -lboost_system -lboost_thread -lboost_timer -lboost_unit_test_framework -lboost_wave -lboost_wserialization 
DEPENDENCIES=-lStreamCommon -lViconCGStream -lViconCGStreamClient -lViconCGStreamClientSDK -lViconDataStreamSDK_CPP -lViconDataStreamSDKCore -lViconDataStreamSDKCoreUtils 
endif
ifeq ($(CONFIG), InternalRelease)
DEFINES=-DVICON_INTERNAL_RELEASE -DNDEBUG -DTCM_LINUX -DTCM_UNIX -DPROJECT_SOURCE_PATH=\".\" 
SYSTEMINCLUDEPATHS=-isystem../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/include 
INCLUDEPATHS=-I. -I../.. -I.. -I../ViconDataStreamSDK_CPP -I. -IInternalRelease 
LIBRARYPATHS=-L../../../../lib/InternalRelease -L../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/lib  -L../../../../bin/InternalRelease
LIBRARIES=-lboost_atomic -lboost_chrono -lboost_container -lboost_context -lboost_coroutine -lboost_date_time -lboost_filesystem -lboost_graph -lboost_iostreams -lboost_locale -lboost_log -lboost_log_setup -lboost_math_c99 -lboost_math_c99f -lboost_math_c99l -lboost_math_tr1 -lboost_math_tr1f -lboost_math_tr1l -lboost_prg_exec_monitor -lboost_program_options -lboost_python3 -lboost_random -lboost_regex -lboost_serialization  -lboost_system -lboost_thread -lboost_timer -lboost_unit_test_framework -lboost_wave -lboost_wserialization 
DEPENDENCIES=-lStreamCommon -lViconCGStream -lViconCGStreamClient -lViconCGStreamClientSDK -lViconDataStreamSDK_CPP -lViconDataStreamSDKCore -lViconDataStreamSDKCoreUtils 
endif
ifeq ($(CONFIG), Release)
DEFINES=-DNDEBUG -DTCM_OFF_SITE -DTCM_LINUX -DTCM_UNIX -DPROJECT_SOURCE_PATH=\".\" 
SYSTEMINCLUDEPATHS=-isystem../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/include 
INCLUDEPATHS=-I. -I../.. -I.. -I../ViconDataStreamSDK_CPP -I. -IRelease 
LIBRARYPATHS=-L../../../../lib/Release -L../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/lib  -L../../../../bin/Release
LIBRARIES=-lboost_atomic -lboost_chrono -lboost_container -lboost_context -lboost_coroutine -lboost_date_time -lboost_filesystem -lboost_graph -lboost_iostreams -lboost_locale -lboost_log -lboost_log_setup -lboost_math_c99 -lboost_math_c99f -lboost_math_c99l -lboost_math_tr1 -lboost_math_tr1f -lboost_math_tr1l -lboost_prg_exec_monitor -lboost_program_options -lboost_python3 -lboost_random -lboost_regex -lboost_serialization  -lboost_system -lboost_thread -lboost_timer -lboost_unit_test_framework -lboost_wave -lboost_wserialization 
DEPENDENCIES=-lStreamCommon -lViconCGStream -lViconCGStreamClient -lViconCGStreamClientSDK -lViconDataStreamSDK_CPP -lViconDataStreamSDKCore -lViconDataStreamSDKCoreUtils 
endif

ENV_CPU=x64
BUILDDIRECTORY=../../../../../../../../Source/Build
SOURCEDIRECTORY=../../../..
PROJECTPATH=.
BINARYDIRECTORY=../../../..
INTERMEDIATEDIRECTORY=.
LIBRARYDIRECTORY=../../../../lib
OUTPUTDIRECTORY=../../../../bin

include $(BINARYDIRECTORY)/gcc.mk

HIDE_BOOST_SCRIPT=hide_boost_version_script
ifneq ($(HIDE_BOOST),)
    HIDE_BOOST_LD_PARAM= -Wl,--version-script=$(HIDE_BOOST_SCRIPT)
    HIDE_BOOST_LD_PREREQ=$(HIDE_BOOST_SCRIPT)
endif
all: all_$(CONFIG)

all_Debug: $(OUTPUTDIRECTORY)/$(CONFIG)/ViconDataStreamSDK_CPPRetimerTest
all_InternalRelease: $(OUTPUTDIRECTORY)/$(CONFIG)/ViconDataStreamSDK_CPPRetimerTest
all_Release: $(OUTPUTDIRECTORY)/$(CONFIG)/ViconDataStreamSDK_CPPRetimerTest

OBJECTS=$(CONFIG)/ViconDataStreamSDK_CPPRetimerTest.o

CXXFLAGS+=$(SYSTEMINCLUDEPATHS) $(INCLUDEPATHS) $(DEFINES)
CCFLAGS+=$(SYSTEMINCLUDEPATHS) $(INCLUDEPATHS) $(DEFINES)
LDFLAGS+=$(LIBRARYPATHS)
# Android toolchain does not include librt but integrates some of its functionality into Android libc.
ifndef ANDROID_TARGET_ARCH
LDFLAGS+=-lrt
endif


$(OUTPUTDIRECTORY)/Debug/ViconDataStreamSDK_CPPRetimerTest: makefile $(OBJECTS) $(LIBRARYDIRECTORY)/$(CONFIG)/libStreamCommon.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStream.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClient.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClientSDK.a $(OUTPUTDIRECTORY)/$(CONFIG)/libViconDataStreamSDK_CPP.so $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCoreUtils.a
	@echo \[1\;32mLinking EXE $@\[0m
	@mkdir -p $(@D)
	$(LD) -Wl,--as-needed -export-dynamic $(LDFLAGS) -o $@ $(OBJECTS) -Wl,--start-group $(DEPENDENCIES) $(LIBRARIES) -Wl,--end-group -pthread -ldl -Wl,-rpath='$$ORIGIN:.' -Wl,-rpath-link=.:$(@D)

$(OUTPUTDIRECTORY)/InternalRelease/ViconDataStreamSDK_CPPRetimerTest: makefile $(OBJECTS) $(LIBRARYDIRECTORY)/$(CONFIG)/libStreamCommon.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStream.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClient.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClientSDK.a $(OUTPUTDIRECTORY)/$(CONFIG)/libViconDataStreamSDK_CPP.so $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCoreUtils.a
	@echo \[1\;32mLinking EXE $@\[0m
	@mkdir -p $(@D)
	$(LD) -Wl,--as-needed -export-dynamic $(LDFLAGS) -o $@ $(OBJECTS) -Wl,--start-group $(DEPENDENCIES) $(LIBRARIES) -Wl,--end-group -pthread -ldl -Wl,-rpath='$$ORIGIN:.' -Wl,-rpath-link=.:$(@D)

$(OUTPUTDIRECTORY)/Release/ViconDataStreamSDK_CPPRetimerTest: makefile $(OBJECTS) $(LIBRARYDIRECTORY)/$(CONFIG)/libStreamCommon.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStream.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClient.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClientSDK.a $(OUTPUTDIRECTORY)/$(CONFIG)/libViconDataStreamSDK_CPP.so $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCoreUtils.a
	@echo \[1\;32mLinking EXE $@\[0m
	@mkdir -p $(@D)
	$(LD) -Wl,--as-needed -export-dynamic $(LDFLAGS) -o $@ $(OBJECTS) -Wl,--start-group $(DEPENDENCIES) $(LIBRARIES) -Wl,--end-group -pthread -ldl -Wl,-rpath='$$ORIGIN:.' -Wl,-rpath-link=.:$(@D)

# Source Files
$(CONFIG)/ViconDataStreamSDK_CPPRetimerTest.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDK_CPPRetimerTest/ViconDataStreamSDK_CPPRetimerTest.cpp
	@echo \[1\;34mCompiling ViconDataStreamSDK_CPPRetimerTest.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDK_CPPRetimerTest/ViconDataStreamSDK_CPPRetimerTest.cpp

-include $(CONFIG)/ViconDataStreamSDK_CPPRetimerTest.d

# Other Files

clean:
	@echo \[1\;31mCleaning $(CONFIG) build\[0m
	find . -path '*/$(CONFIG)/*' \( -name '*.[od]' -o -name '*.gch' \) -exec rm -f {} ';' 
	rm -f moc_*.cxx

$(HIDE_BOOST_SCRIPT): makefile
	echo -n >$@
	echo "{" >>$@
	echo "  local: *N5boost*; *NK5boost*;" >>$@
	echo "};" >>$@

# Autogenerated makefile for ViconDataStreamSDK_CPP

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
DEFINES=-DTCM_LINUX -DTCM_UNIX -D_DEBUG -DPROJECT_SOURCE_PATH=\".\" -DRELEASE_SOFTWARE 
SYSTEMINCLUDEPATHS=-isystem../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/include 
INCLUDEPATHS=-I. -I../.. -I.. -I. -IDebug 
LIBRARYPATHS=-L../../../../lib/Debug -L../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/lib  -L../../../../bin/Debug
LIBRARIES=-lboost_atomic -lboost_chrono -lboost_container -lboost_context -lboost_coroutine -lboost_date_time -lboost_filesystem -lboost_graph -lboost_iostreams -lboost_locale -lboost_log -lboost_log_setup -lboost_math_c99 -lboost_math_c99f -lboost_math_c99l -lboost_math_tr1 -lboost_math_tr1f -lboost_math_tr1l -lboost_prg_exec_monitor -lboost_program_options -lboost_python3 -lboost_random -lboost_regex -lboost_serialization  -lboost_system -lboost_thread -lboost_timer -lboost_unit_test_framework -lboost_wave -lboost_wserialization 
DEPENDENCIES=-lStreamCommon -lViconCGStream -lViconCGStreamClient -lViconCGStreamClientSDK -lViconDataStreamSDKCore -lViconDataStreamSDKCoreUtils 
endif
ifeq ($(CONFIG), InternalRelease)
DEFINES=-DVICON_INTERNAL_RELEASE -DNDEBUG -DTCM_LINUX -DTCM_UNIX -DPROJECT_SOURCE_PATH=\".\" -DRELEASE_SOFTWARE 
SYSTEMINCLUDEPATHS=-isystem../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/include 
INCLUDEPATHS=-I. -I../.. -I.. -I. -IInternalRelease 
LIBRARYPATHS=-L../../../../lib/InternalRelease -L../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/lib  -L../../../../bin/InternalRelease
LIBRARIES=-lboost_atomic -lboost_chrono -lboost_container -lboost_context -lboost_coroutine -lboost_date_time -lboost_filesystem -lboost_graph -lboost_iostreams -lboost_locale -lboost_log -lboost_log_setup -lboost_math_c99 -lboost_math_c99f -lboost_math_c99l -lboost_math_tr1 -lboost_math_tr1f -lboost_math_tr1l -lboost_prg_exec_monitor -lboost_program_options -lboost_python3 -lboost_random -lboost_regex -lboost_serialization  -lboost_system -lboost_thread -lboost_timer -lboost_unit_test_framework -lboost_wave -lboost_wserialization 
DEPENDENCIES=-lStreamCommon -lViconCGStream -lViconCGStreamClient -lViconCGStreamClientSDK -lViconDataStreamSDKCore -lViconDataStreamSDKCoreUtils 
endif
ifeq ($(CONFIG), Release)
DEFINES=-DNDEBUG -DTCM_OFF_SITE -DTCM_LINUX -DTCM_UNIX -DPROJECT_SOURCE_PATH=\".\" -DRELEASE_SOFTWARE 
SYSTEMINCLUDEPATHS=-isystem../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/include 
INCLUDEPATHS=-I. -I../.. -I.. -I. -IRelease 
LIBRARYPATHS=-L../../../../lib/Release -L../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/lib  -L../../../../bin/Release
LIBRARIES=-lboost_atomic -lboost_chrono -lboost_container -lboost_context -lboost_coroutine -lboost_date_time -lboost_filesystem -lboost_graph -lboost_iostreams -lboost_locale -lboost_log -lboost_log_setup -lboost_math_c99 -lboost_math_c99f -lboost_math_c99l -lboost_math_tr1 -lboost_math_tr1f -lboost_math_tr1l -lboost_prg_exec_monitor -lboost_program_options -lboost_python3 -lboost_random -lboost_regex -lboost_serialization  -lboost_system -lboost_thread -lboost_timer -lboost_unit_test_framework -lboost_wave -lboost_wserialization 
DEPENDENCIES=-lStreamCommon -lViconCGStream -lViconCGStreamClient -lViconCGStreamClientSDK -lViconDataStreamSDKCore -lViconDataStreamSDKCoreUtils 
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

all_Debug: $(OUTPUTDIRECTORY)/$(CONFIG)/libViconDataStreamSDK_CPP.so
all_InternalRelease: $(OUTPUTDIRECTORY)/$(CONFIG)/libViconDataStreamSDK_CPP.so
all_Release: $(OUTPUTDIRECTORY)/$(CONFIG)/libViconDataStreamSDK_CPP.so

OBJECTS=$(CONFIG)/DataStreamClient.o $(CONFIG)/DataStreamRetimingClient.o

CXXFLAGS+=$(SYSTEMINCLUDEPATHS) $(INCLUDEPATHS) $(DEFINES)
CCFLAGS+=$(SYSTEMINCLUDEPATHS) $(INCLUDEPATHS) $(DEFINES)
LDFLAGS+=$(LIBRARYPATHS)
ifeq ($(CXX_VERSION_5_0), q)
CXXFLAGS+=-std=c++14
else
CXXFLAGS+=-std=c++1y
endif
# Android toolchain does not include librt but integrates some of its functionality into Android libc.
ifndef ANDROID_TARGET_ARCH
LDFLAGS+=-lrt
endif


$(OUTPUTDIRECTORY)/Debug/libViconDataStreamSDK_CPP.so: makefile $(OBJECTS) $(LIBRARYDIRECTORY)/$(CONFIG)/libStreamCommon.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStream.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClient.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClientSDK.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCoreUtils.a $(HIDE_BOOST_LD_PREREQ)
	@echo \[1\;32mLinking dll $@\[0m
	@mkdir -p $(@D)
	$(LD) -fPIC -shared -Wl,--as-needed $(LDFLAGS) -o $@ $(OBJECTS) -Wl,--start-group $(DEPENDENCIES) $(LIBRARIES) -Wl,--end-group -pthread -ldl -Wl,-rpath='$$ORIGIN':$(@D) $(HIDE_BOOST_LD_PARAM)

$(OUTPUTDIRECTORY)/InternalRelease/libViconDataStreamSDK_CPP.so: makefile $(OBJECTS) $(LIBRARYDIRECTORY)/$(CONFIG)/libStreamCommon.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStream.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClient.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClientSDK.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCoreUtils.a $(HIDE_BOOST_LD_PREREQ)
	@echo \[1\;32mLinking dll $@\[0m
	@mkdir -p $(@D)
	$(LD) -fPIC -shared -Wl,--as-needed $(LDFLAGS) -o $@ $(OBJECTS) -Wl,--start-group $(DEPENDENCIES) $(LIBRARIES) -Wl,--end-group -pthread -ldl -Wl,-rpath='$$ORIGIN':$(@D) $(HIDE_BOOST_LD_PARAM)

$(OUTPUTDIRECTORY)/Release/libViconDataStreamSDK_CPP.so: makefile $(OBJECTS) $(LIBRARYDIRECTORY)/$(CONFIG)/libStreamCommon.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStream.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClient.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconCGStreamClientSDK.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCoreUtils.a $(HIDE_BOOST_LD_PREREQ)
	@echo \[1\;32mLinking dll $@\[0m
	@mkdir -p $(@D)
	$(LD) -fPIC -shared -Wl,--as-needed $(LDFLAGS) -o $@ $(OBJECTS) -Wl,--start-group $(DEPENDENCIES) $(LIBRARIES) -Wl,--end-group -pthread -ldl -Wl,-rpath='$$ORIGIN':$(@D) $(HIDE_BOOST_LD_PARAM)

# Source Files
$(CONFIG)/DataStreamClient.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDK_CPP/DataStreamClient.cpp
	@echo \[1\;34mCompiling DataStreamClient.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDK_CPP/DataStreamClient.cpp

-include $(CONFIG)/DataStreamClient.d

$(CONFIG)/DataStreamRetimingClient.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDK_CPP/DataStreamRetimingClient.cpp
	@echo \[1\;34mCompiling DataStreamRetimingClient.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDK_CPP/DataStreamRetimingClient.cpp

-include $(CONFIG)/DataStreamRetimingClient.d

# Header Files
# Resource Files
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

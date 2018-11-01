# Makefile for ViconDataStreamSDKCore

ifndef VERBOSE
.SILENT :
endif
.SUFFIXES :

ifdef CONFIG
ifneq ($(CONFIG),Debug)
ifneq ($(CONFIG),InternalRelease)
ifneq ($(CONFIG),Release)
Error: unknown configuration.
endif
endif
endif
else
CONFIG=Debug
endif

INCLUDEPATHS=../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/include . .. ../.. 
INCLUDEPATHS_Debug=Debug 
INCLUDEPATHS_InternalRelease=InternalRelease 
INCLUDEPATHS_Release=Release 
LIBRARYPATHS=../../../../thirdparty/Boost/boost-1.58.0-dynamic-linux-x64/installed/lib 
LIBRARYPATHS_Debug=../../../../lib/Debug ../../../../bin/Debug
LIBRARYPATHS_InternalRelease=../../../../lib/InternalRelease ../../../../bin/InternalRelease
LIBRARYPATHS_Release=../../../../lib/Release ../../../../bin/Release
DEPENDENCIES=ViconCGStreamClientSDK ViconCGStreamClient ViconCGStream StreamCommon 
LIBRARIES=
LIBRARIES_Debug=boost_wserialization boost_wave boost_unit_test_framework boost_timer boost_thread boost_system boost_signals boost_serialization boost_regex boost_random boost_python boost_program_options boost_prg_exec_monitor boost_math_tr1l boost_math_tr1f boost_math_tr1 boost_math_c99l boost_math_c99f boost_math_c99 boost_log_setup boost_log boost_locale boost_iostreams boost_graph boost_filesystem boost_date_time boost_coroutine boost_context boost_container boost_chrono boost_atomic 
LIBRARIES_InternalRelease=boost_wserialization boost_wave boost_unit_test_framework boost_timer boost_thread boost_system boost_signals boost_serialization boost_regex boost_random boost_python boost_program_options boost_prg_exec_monitor boost_math_tr1l boost_math_tr1f boost_math_tr1 boost_math_c99l boost_math_c99f boost_math_c99 boost_log_setup boost_log boost_locale boost_iostreams boost_graph boost_filesystem boost_date_time boost_coroutine boost_context boost_container boost_chrono boost_atomic 
LIBRARIES_Release=boost_wserialization boost_wave boost_unit_test_framework boost_timer boost_thread boost_system boost_signals boost_serialization boost_regex boost_random boost_python boost_program_options boost_prg_exec_monitor boost_math_tr1l boost_math_tr1f boost_math_tr1 boost_math_c99l boost_math_c99f boost_math_c99 boost_log_setup boost_log boost_locale boost_iostreams boost_graph boost_filesystem boost_date_time boost_coroutine boost_context boost_container boost_chrono boost_atomic 
DEFINES=TCM_LINUX TCM_UNIX PROJECT_SOURCE_PATH=\"/home/swtest/workspace/DatastreamSDK_Linux_64_Branch_Release/Binary/bin/Release/deployment/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore\" 
DEFINES_Debug=_DEBUG 
DEFINES_InternalRelease=VICON_INTERNAL_RELEASE NDEBUG 
DEFINES_Release=NDEBUG TCM_OFF_SITE 
ENV_CPU=x64

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

all_Debug: $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a
all_InternalRelease: $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a
all_Release: $(LIBRARYDIRECTORY)/$(CONFIG)/libViconDataStreamSDKCore.a

OBJECTS=$(CONFIG)/ClientUtils.o $(CONFIG)/CoreClient.o $(CONFIG)/AxisMapping.o $(CONFIG)/RetimingClient.o $(CONFIG)/RetimerUtils.o 

CXXFLAGS=$(CXXFLAGS_$(CONFIG)) $(L_INCLUDEPATHS) $(L_INCLUDEPATHS_$(CONFIG)) $(L_INCLUDES) $(L_INCLUDES_$(CONFIG)) $(L_DEFINES) $(L_DEFINES_$(CONFIG))
CCFLAGS=$(CCFLAGS_$(CONFIG)) $(L_INCLUDEPATHS) $(L_INCLUDEPATHS_$(CONFIG)) $(L_INCLUDES) $(L_INCLUDES_$(CONFIG)) $(L_DEFINES) $(L_DEFINES_$(CONFIG))
LDFLAGS=$(LDFLAGS_$(CONFIG)) $(L_LIBRARYPATHS) $(L_LIBRARYPATHS_$(CONFIG))
CXXFLAGS+=-Wno-unused-local-typedefs
CXXFLAGS+=-Wno-delete-non-virtual-dtor -std=c++14
#Android toolchain does not include librt but integrates some of its functionality into Android libc.
ifndef ANDROID_TARGET_ARCH
LDFLAGS+=-lrt
endif


$(LIBRARYDIRECTORY)/Debug/libViconDataStreamSDKCore.a: makefile $(OBJECTS)
	@echo \[1\;35mLinking archive library $@\[0m
	@mkdir -p $(@D)
	$(AR) rcs $@ $(OBJECTS)

$(LIBRARYDIRECTORY)/InternalRelease/libViconDataStreamSDKCore.a: makefile $(OBJECTS)
	@echo \[1\;35mLinking archive library $@\[0m
	@mkdir -p $(@D)
	$(AR) rcs $@ $(OBJECTS)

$(LIBRARYDIRECTORY)/Release/libViconDataStreamSDKCore.a: makefile $(OBJECTS)
	@echo \[1\;35mLinking archive library $@\[0m
	@mkdir -p $(@D)
	$(AR) rcs $@ $(OBJECTS)

# Source Files
$(CONFIG)/ClientUtils.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/ClientUtils.cpp
	@echo \[1\;34mCompiling ClientUtils.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/ClientUtils.cpp

-include $(CONFIG)/ClientUtils.d

$(CONFIG)/CoreClient.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/CoreClient.cpp
	@echo \[1\;34mCompiling CoreClient.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/CoreClient.cpp

-include $(CONFIG)/CoreClient.d

$(CONFIG)/AxisMapping.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/AxisMapping.cpp
	@echo \[1\;34mCompiling AxisMapping.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/AxisMapping.cpp

-include $(CONFIG)/AxisMapping.d

$(CONFIG)/RetimingClient.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/RetimingClient.cpp
	@echo \[1\;34mCompiling RetimingClient.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/RetimingClient.cpp

-include $(CONFIG)/RetimingClient.d

$(CONFIG)/RetimerUtils.o: makefile $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/RetimerUtils.cpp
	@echo \[1\;34mCompiling RetimerUtils.cpp\[0m
	@mkdir -p $(@D)
	find $(CONFIG) -name *.gch -exec cp '{}' . \;
	$(CXX) -fPIC -MMD -MP -I$(CONFIG)/ $(CXXFLAGS)  -o $@ -c $(SOURCEDIRECTORY)/Vicon/CrossMarket/DataStream/ViconDataStreamSDKCore/RetimerUtils.cpp

-include $(CONFIG)/RetimerUtils.d

# Header Files
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

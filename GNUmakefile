# $Id: GNUmakefile,v 1.11 2004/12/08 21:20:43 marcel Exp $

#include $(GNUSTEP_MAKEFILES)/common.make

LIBRARY_NAME = libMPWFoundation

GNUSTEP_LOCAL_ADDITIONAL_MAKEFILES=base.make
include $(GNUSTEP_MAKEFILES)/common.make

libMPWFoundation_DLL_DEF = MPWFoundation.def

disabled_libMPWFoundation_HEADER_FILES = \
	AccessorMacros.h		\
	CodingAdditions.h		\
	DebugMacros.h			\
	FIFO.h				\
	MPWASCII85Stream.h		\
	MPWAssociation.h		\
	MPWAsyncProxy.h			\
	MPWByteStream.h			\
	MPWEnumFilter.h			\
	MPWEnumSelectFilter.h		\
	MPWEnumeratorBase.h		\
	MPWEnumeratorEnumerator.h	\
	MPWEnumeratorSource.h		\
	MPWFakedReturnMethodSignature.h	\
	MPWFilterStream.h		\
	MPWFlattenStream.h		\
	MPWFoundation.h			\
	MPWHierarchicalStream.h		\
	MPWIgnoreTrampoline.h		\
	MPWJetStream.h			\
	MPWLZWStream.h			\
	MPWMsgExpression.h		\
	MPWObject.h			\
	MPWObjectReference.h			\
	MPWObjectCache.h		\
	MPWPSByteStream.h		\
	MPWParallelStream.h		\
	MPWPoint.h			\
	MPWPropertyListStream.h		\
	MPWRealArray.h			\
	MPWRect.h			\
	MPWRuntimeAdditions.h		\
	MPWScanner.h			\
	MPWStream.h			\
	MPWSubData.h			\
	MPWTrampoline.h			\
	MPWUShortArray.h		\
	MPWUniqueString.h		\
	NSArrayFiltering.h		\
	NSArrayFilters.h		\
	NSBundleConveniences.h		\
	NSCaseInsensitiveUniqueString.h	\
	NSConditionLockSem.h		\
	NSDictAdditions.h		\
	NSEnumFilter.h			\
	NSEnumObjectFilter.h		\
	NSEnumeratorFiltering.h		\
	NSInvocationAdditions.h		\
	NSInvocationAdditions_lookup.h	\
	NSNil.h				\
	NSObjectAdditions.h		\
	NSObjectFiltering.h		\
	NSObjectInterThreadMessaging.h	\
	NSRectAdditions.h		\
	NSSelectEnumerator.h		\
	NSStringAdditions.h		\
	NSThreadInterThreadMessaging.h	\
	bytecoding.h			\

disabled_libMPWFoundation_HEADER_FILES_INSTALL_DIR = /MPWFoundation

libMPWFoundation_OBJC_FILES = \
	MPWObject.m NSNil.m NSInvocationAdditions.m \
	NSStringAdditions.m CodingAdditions.m MPWObjectCache.m \
	NSRectAdditions.m MPWScanner.m NSDictAdditions.m\
	MPWRuntimeAdditions.m NSObjectAdditions.m MPWPoint.m\
	MPWRect.m NSDataPrivateMemoryMapping.m MPWTrampoline.m\
	MPWMsgExpression.m MPWAssociation.m MPWIgnoreTrampoline.m \
	NSBundleConveniences.m MPWObjectReference.m \

libMPWFoundation_C_FILES =  bytecoding.c

libMPWFoundation_SUBPROJECTS = \
	Collections.subproj	\
	Streams.subproj		\
	Comm.subproj		\


libMPWFoundation_LIBRARIES_DEPEND_UPON += -lgnustep-base -lobjc-gnu.1

# LDFLAGS += -L /C/GNUstep/System/Libraries/ix86/mingw32/gnu-gnu-gnu/ 
OBJCFLAGS += -Wno-import


libMPWFoundation_INCLUDE_DIRS += -I.headers -I. -I..

-include GNUmakefile.preamble
include $(GNUSTEP_MAKEFILES)/library.make
-include GNUmakefile.postamble

before-all ::
	
#	@$(MKDIRS) $(libMPWFoundation_HEADER_FILES_DIR)
#	cp *.h $(libMPWFoundation_HEADER_FILES_DIR)
#	cp Collections.subproj/*.h $(libMPWFoundation_HEADER_FILES_DIR)
#	cp Comm.subproj/*.h        $(libMPWFoundation_HEADER_FILES_DIR)
#	cp Streams.subproj/*.h     $(libMPWFoundation_HEADER_FILES_DIR)
#	cp Threading.subproj/*.h   $(libMPWFoundation_HEADER_FILES_DIR)

after-clean ::
	rm -rf .headers

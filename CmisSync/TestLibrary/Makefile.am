ASSEMBLY = TestLibrary
TARGET = library

ASSEMBLY_INFO_SOURCE =  \
	Properties/AssemblyInfo.cs

LIBS = $(LOG4NET_LIBS) $(DATALIBS) $(JSON_LIBS) $(DOTCMISLIBS) \
	   $(LIBS_CMISSYNCLIB_DEPS) \
	   $(NUNIT_LIBS) \
	   -r:$(srcdir)/lib/Moq.dll \
	   -r:$(srcdir)/lib/xunit.dll \
	   -r:$(srcdir)/lib/xunit.extensions.dll

SOURCES =  \
	CmisSyncTests.cs \
	WatcherTest.cs \
	CmisDatabaseTest.cs \
	ChunkedStreamTest.cs \
	SyncEventQueueTest.cs \
	SyncEventManagerTest.cs \
	EventTypesTest.cs \
	FSDeletionHandlerTest.cs \
	DebugLoggingHandlerTest.cs \
	LocalFilesystemActivityGenerator.cs \
	ConfigurationTest.cs \
	EncodingTest.cs

EXTRA_DIST = TestLibrary.csproj \
	lib/Moq.dll \
	lib/xunit.dll \
	lib/xunit.extensions.dll

include $(top_srcdir)/build/build.mk

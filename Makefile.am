bin_SCRIPTS = scripts/bin/*

bin_PROGRAMS = hshell
hshell_SOURCES = src/hal_shell_client.c
hshell_CPPFLAGS = -I$(top_srcdir)/sonic -I$(includedir)/sonic
hshell_LIBADD = -lsonic_common -lsonic_logging -lsonic_object_library

pyutilsdir=$(libdir)/sonic
pyutils_SCRIPTS = scripts/lib/python/*.py

nobase_include_HEADERS=sonic/hal_if_mapping.h sonic/nas_types.h sonic/nas_switch.h sonic/nas_base_utils.h sonic/nas_base_obj.h sonic/nas_vlan_consts.h sonic/nas_qos_consts.h sonic/nas_ndi_obj_id_table.h sonic/nas_if_utils.h

lib_LTLIBRARIES=libsonic_nas_common.la

libsonic_nas_common_la_SOURCES= src/hal_if_mapping.cpp src/nas_switch.c src/nas_switch_utl.cpp src/nas_base_utils.cpp src/nas_base_obj.cpp src/nas_base_ndi_utl.cpp src/nas_ndi_obj_id_table.cpp src/nas_if_utils.cpp

libsonic_nas_common_la_CPPFLAGS= -D_FILE_OFFSET_BITS=64 -I$(top_srcdir)/sonic -I$(includedir)/sonic

libsonic_nas_common_la_CXXFLAGS=-std=c++11

libsonic_nas_common_la_LDFLAGS=-shared -version-info 1:1:0

libsonic_nas_common_la_LIBADD=-lsonic_common -lsonic_object_library -lsonic_cps_class_map -lsonic_logging

systemdconfdir=/lib/systemd/system
systemdconf_DATA = scripts/init/*.service

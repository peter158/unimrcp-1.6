AM_CPPFLAGS                = $(UNIMRCP_PLUGIN_INCLUDES)

plugin_LTLIBRARIES         = alicloudrecog.la


# alicloudrecog_la_SOURCES       = src/alicloud_recog_engine.c
alicloudrecog_la_SOURCES       = src/alicloud_recog_engine.cpp
alicloudrecog_la_LDFLAGS       = $(UNIMRCP_PLUGIN_OPTS) \ 
                                -L$(top_srcdir)/plugins/alicloud-recog/NlsSdk3.X/lib/ \
                                -lalibabacloud-idst-common -lalibabacloud-idst-speech
alicloudrecog_ladir            =$(libdir)
alicloudrecog_la_DATA          =$(top_srcdir)/plugins/alicloud-recog/NlsSdk3.X/lib/libalibabacloud-idst-speech.so \
                                $(top_srcdir)/plugins/alicloud-recog/NlsSdk3.X/lib/libalibabacloud-idst-common.so

include $(top_srcdir)/build/rules/uniplugin.am
UNIMRCP_PLUGIN_INCLUDES         += -I$(top_srcdir)/plugins/alicloud-recog/NlsSdk3.X/include
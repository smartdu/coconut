# 此文件由makeobj.sh自动生成
############################################################
# 项目名 : 
# 模块名 : 
# 备  注 : 
############################################################

###### 源文件配置区
#@ c_FILE
c_FILE		=	\
			list.c \
			LOGC.c \
			fasterhttp.c \
			tcpdaemon_lib.c \
			rbtree.c rbtree_ins.o \
			coconut.c \

###### 目标文件、安装目录配置区
include makeinstall
BIN		=	coconut
BININST		=	$(_BININST)

###### 编译选项
CFLAGS		=	$(_CFLAGS) \
			-std=gnu99 \

###### 链接选项
LFLAGS		=	$(_LFLAGS) \
			-lcrypto \
			-lssl \
			-lz \
			-ldl \

###### 额外宏定义区
CLEAN_ADDITION	=

###### 加载mktpl模板库
#@ make_all
#@ make_clean
#@ make_install
#@ make_install_BININST
#@ make_uninstall
#@ make_uninstall_BININST
include $(MKTPLDIR)/makeobj_$(MKTPLOS).inc

###### 目标文件依赖关系
coconut		:	$(c_FILE_o)
	$(CC) -o $@ $(c_FILE_o) $(LFLAGS)


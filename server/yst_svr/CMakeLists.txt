INCLUDE_DIRECTORIES(${TOP_SOURCE_DIR}/libs/include)
INCLUDE_DIRECTORIES(${IPCAM_SOURCE_DIR}/libs/include/ivp)
INCLUDE_DIRECTORIES(${IPCAM_SOURCE_DIR}/libs/include/mml/core)
INCLUDE_DIRECTORIES(${TOP_SOURCE_DIR}/server/sctrl)
INCLUDE_DIRECTORIES(${IPCAM_SOURCE_DIR}/server/sport)
INCLUDE_DIRECTORIES(${IPCAM_SOURCE_DIR}/server/tuya)
INCLUDE_DIRECTORIES(${TOP_SOURCE_DIR}/module/include)
INCLUDE_DIRECTORIES(${TOP_SOURCE_DIR}/porting/include)
INCLUDE_DIRECTORIES(${TOP_SOURCE_DIR}/porting/${BOARD}/include)

PROJECT(YST_SVR_LIB)

SET(YST_SVR_SRC
		MRemoteCfg.c
		mtransmit.c
		rcmodule.c
		yst_firmup.c
        )

ADD_LIBRARY(yst_svr STATIC ${YST_SVR_SRC})
 
 

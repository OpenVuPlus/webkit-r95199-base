SET(WebKit2_INCLUDE_DIRECTORIES
    "${WEBKIT2_DIR}"
    "${WEBKIT2_DIR}/Platform"
    "${WEBKIT2_DIR}/Platform/CoreIPC"
    "${WEBKIT2_DIR}/PluginProcess"
    "${WEBKIT2_DIR}/Shared"
    "${WEBKIT2_DIR}/Shared/API"
    "${WEBKIT2_DIR}/Shared/API/c"
    "${WEBKIT2_DIR}/Shared/CoreIPCSupport"
    "${WEBKIT2_DIR}/Shared/Plugins"
    "${WEBKIT2_DIR}/Shared/Plugins/Netscape"
    "${WEBKIT2_DIR}/Shared/Plugins/Netscape/x11"
    "${WEBKIT2_DIR}/Shared/efl"
    "${WEBKIT2_DIR}/UIProcess"
    "${WEBKIT2_DIR}/UIProcess/API"
    "${WEBKIT2_DIR}/UIProcess/API/C"
    "${WEBKIT2_DIR}/UIProcess/API/cpp"
    "${WEBKIT2_DIR}/UIProcess/Authentication"
    "${WEBKIT2_DIR}/UIProcess/Downloads"
    "${WEBKIT2_DIR}/UIProcess/Launcher"
    "${WEBKIT2_DIR}/UIProcess/Plugins"
    "${WEBKIT2_DIR}/UIProcess/efl"
    "${WEBKIT2_DIR}/WebProcess"
    "${WEBKIT2_DIR}/WebProcess/ApplicationCache"
    "${WEBKIT2_DIR}/WebProcess/Authentication"
    "${WEBKIT2_DIR}/WebProcess/Cookies"
    "${WEBKIT2_DIR}/WebProcess/Downloads"
    "${WEBKIT2_DIR}/WebProcess/FullScreen"
    "${WEBKIT2_DIR}/WebProcess/Geolocation"
    "${WEBKIT2_DIR}/WebProcess/IconDatabase"
    "${WEBKIT2_DIR}/WebProcess/InjectedBundle"
    "${WEBKIT2_DIR}/WebProcess/InjectedBundle/API"
    "${WEBKIT2_DIR}/WebProcess/InjectedBundle/API/c"
    "${WEBKIT2_DIR}/WebProcess/InjectedBundle/DOM"
    "${WEBKIT2_DIR}/WebProcess/KeyValueStorage"
    "${WEBKIT2_DIR}/WebProcess/Launching"
    "${WEBKIT2_DIR}/WebProcess/MediaCache"
    "${WEBKIT2_DIR}/WebProcess/ResourceCache"
    "${WEBKIT2_DIR}/WebProcess/Plugins"
    "${WEBKIT2_DIR}/WebProcess/Plugins/Netscape"
    "${WEBKIT2_DIR}/WebProcess/WebCoreSupport"
    "${WEBKIT2_DIR}/WebProcess/WebPage"
    "${WEBCORE_DIR}"
    "${WEBCORE_DIR}/accessibility"
    "${WEBCORE_DIR}/bindings/js"
    "${WEBCORE_DIR}/bindings"
    "${WEBCORE_DIR}/bridge"
    "${WEBCORE_DIR}/bridge/jsc"
    "${WEBCORE_DIR}/css"
    "${WEBCORE_DIR}/dom"
    "${WEBCORE_DIR}/editing"
    "${WEBCORE_DIR}/history"
    "${WEBCORE_DIR}/html"
    "${WEBCORE_DIR}/loader"
    "${WEBCORE_DIR}/loader/icon"
    "${WEBCORE_DIR}/loader/cache"
    "${WEBCORE_DIR}/page"
    "${WEBCORE_DIR}/page/animation"
    "${WEBCORE_DIR}/platform"
    "${WEBCORE_DIR}/platform/animation"
    "${WEBCORE_DIR}/platform/graphics"
    "${WEBCORE_DIR}/platform/graphics/transforms"
    "${WEBCORE_DIR}/platform/network"
    "${WEBCORE_DIR}/platform/sql"
    "${WEBCORE_DIR}/platform/text"
    "${WEBCORE_DIR}/plugins"
    "${WEBCORE_DIR}/rendering"
    "${WEBCORE_DIR}/rendering/style"
    "${WEBCORE_DIR}/storage"
    "${WEBCORE_DIR}/svg"
    "${WEBCORE_DIR}/svg/properties"
    "${JAVASCRIPTCORE_DIR}"
    "${JAVASCRIPTCORE_DIR}/ForwardingHeaders"
    "${JAVASCRIPTCORE_DIR}/API"
    "${JAVASCRIPTCORE_DIR}/assembler"
    "${JAVASCRIPTCORE_DIR}/bytecode"
    "${JAVASCRIPTCORE_DIR}/bytecompiler"
    "${JAVASCRIPTCORE_DIR}/collector/handles"
    "${JAVASCRIPTCORE_DIR}/heap"
    "${JAVASCRIPTCORE_DIR}/interpreter"
    "${JAVASCRIPTCORE_DIR}/jit"
    "${JAVASCRIPTCORE_DIR}/parser"
    "${JAVASCRIPTCORE_DIR}/profiler"
    "${JAVASCRIPTCORE_DIR}/runtime"
    "${JAVASCRIPTCORE_DIR}/wtf"
    "${DERIVED_SOURCES_DIR}"
    "${DERIVED_SOURCES_WEBCORE_DIR}"
    "${DERIVED_SOURCES_WEBKIT2_DIR}"
    "${DERIVED_SOURCES_WEBKIT2_DIR}/include"
    "${CMAKE_BINARY_DIR}"
    "${CMAKE_SOURCE_DIR}"
)

SET(WebKit2_SOURCES
    Platform/CoreIPC/ArgumentDecoder.cpp
    Platform/CoreIPC/ArgumentEncoder.cpp
    Platform/CoreIPC/Attachment.cpp
    Platform/CoreIPC/BinarySemaphore.cpp
    Platform/CoreIPC/Connection.cpp
    Platform/CoreIPC/DataReference.cpp

    Platform/Logging.cpp
    Platform/Module.cpp
    Platform/RunLoop.cpp
    Platform/WorkQueue.cpp

    PluginProcess/PluginControllerProxy.cpp
    PluginProcess/PluginProcess.cpp
    PluginProcess/WebProcessConnection.cpp

    Shared/API/c/WKArray.cpp
    Shared/API/c/WKCertificateInfo.cpp
    Shared/API/c/WKContextMenuItem.cpp
    Shared/API/c/WKData.cpp
    Shared/API/c/WKDictionary.cpp
    Shared/API/c/WKError.cpp
    Shared/API/c/WKGraphicsContext.cpp
    Shared/API/c/WKImage.cpp
    Shared/API/c/WKMutableArray.cpp
    Shared/API/c/WKMutableDictionary.cpp
    Shared/API/c/WKNumber.cpp
    Shared/API/c/WKSecurityOrigin.cpp
    Shared/API/c/WKSerializedScriptValue.cpp
    Shared/API/c/WKString.cpp
    Shared/API/c/WKType.cpp
    Shared/API/c/WKURL.cpp
    Shared/API/c/WKURLRequest.cpp
    Shared/API/c/WKURLResponse.cpp
    Shared/API/c/WKUserContentURLPattern.cpp

    Shared/ShareableBitmap.cpp
    Shared/ChildProcess.cpp
    Shared/ImmutableArray.cpp
    Shared/ImmutableDictionary.cpp
    Shared/MutableArray.cpp
    Shared/MutableDictionary.cpp
    Shared/OriginAndDatabases.cpp
    Shared/PlatformPopupMenuData.cpp
    Shared/PrintInfo.cpp

    Shared/Plugins/Netscape/NetscapePluginModule.cpp
    Shared/Plugins/Netscape/NetscapePluginModuleNone.cpp

    Shared/Plugins/NPIdentifierData.cpp
    Shared/Plugins/NPObjectMessageReceiver.cpp
    Shared/Plugins/NPObjectProxy.cpp
    Shared/Plugins/NPRemoteObjectMap.cpp
    Shared/Plugins/NPVariantData.cpp
    Shared/Plugins/PluginProcessCreationParameters.cpp

    Shared/SecurityOriginData.cpp
    Shared/SessionState.cpp
    Shared/StatisticsData.cpp
    Shared/UpdateInfo.cpp
    Shared/VisitedLinkTable.cpp
    Shared/WebBackForwardListItem.cpp
    Shared/WebContextMenuItem.cpp
    Shared/WebContextMenuItemData.cpp
    Shared/WebError.cpp
    Shared/WebEventConversion.cpp
    Shared/WebEvent.cpp
    Shared/WebGeolocationPosition.cpp
    Shared/WebGraphicsContext.cpp
    Shared/WebImage.cpp
    Shared/WebKeyboardEvent.cpp
    Shared/WebMouseEvent.cpp
    Shared/WebOpenPanelParameters.cpp
    Shared/WebPageCreationParameters.cpp
    Shared/WebPageGroupData.cpp
    Shared/WebPlatformTouchPoint.cpp
    Shared/WebPopupItem.cpp
    Shared/WebPreferencesStore.cpp
    Shared/WebProcessCreationParameters.cpp
    Shared/WebTouchEvent.cpp
    Shared/WebURLRequest.cpp
    Shared/WebURLResponse.cpp
    Shared/WebWheelEvent.cpp

    UIProcess/API/C/WKApplicationCacheManager.cpp
    UIProcess/API/C/WKAuthenticationChallenge.cpp
    UIProcess/API/C/WKAuthenticationDecisionListener.cpp
    UIProcess/API/C/WKBackForwardList.cpp
    UIProcess/API/C/WKBackForwardListItem.cpp
    UIProcess/API/C/WKContext.cpp
    UIProcess/API/C/WKCookieManager.cpp
    UIProcess/API/C/WKCredential.cpp
    UIProcess/API/C/WKDatabaseManager.cpp
    UIProcess/API/C/WKDownload.cpp
    UIProcess/API/C/WKFormSubmissionListener.cpp
    UIProcess/API/C/WKFrame.cpp
    UIProcess/API/C/WKFramePolicyListener.cpp
    UIProcess/API/C/WKIconDatabase.cpp
    UIProcess/API/C/WKInspector.cpp
    UIProcess/API/C/WKKeyValueStorageManager.cpp
    UIProcess/API/C/WKMediaCacheManager.cpp
    UIProcess/API/C/WKNavigationData.cpp
    UIProcess/API/C/WKOpenPanelParameters.cpp
    UIProcess/API/C/WKOpenPanelResultListener.cpp
    UIProcess/API/C/WKPage.cpp
    UIProcess/API/C/WKPageGroup.cpp
    UIProcess/API/C/WKPluginSiteDataManager.cpp
    UIProcess/API/C/WKPreferences.cpp
    UIProcess/API/C/WKProtectionSpace.cpp
    UIProcess/API/C/WKResourceCacheManager.cpp

    UIProcess/Authentication/AuthenticationChallengeProxy.cpp
    UIProcess/Authentication/AuthenticationDecisionListener.cpp
    UIProcess/Authentication/WebCredential.cpp
    UIProcess/Authentication/WebProtectionSpace.cpp

    UIProcess/BackingStore.cpp

    UIProcess/Downloads/DownloadProxy.cpp

    UIProcess/DrawingAreaProxy.cpp
    UIProcess/DrawingAreaProxyImpl.cpp
    UIProcess/FindIndicator.cpp
    UIProcess/GeolocationPermissionRequestManagerProxy.cpp
    UIProcess/GeolocationPermissionRequestProxy.cpp

    UIProcess/Launcher/ProcessLauncher.cpp
    UIProcess/Launcher/ThreadLauncher.cpp

    UIProcess/Plugins/PluginInfoStore.cpp
    UIProcess/Plugins/PluginProcessManager.cpp
    UIProcess/Plugins/PluginProcessProxy.cpp
    UIProcess/Plugins/WebPluginSiteDataManager.cpp

    UIProcess/ResponsivenessTimer.cpp
    UIProcess/TiledDrawingAreaProxy.cpp
    UIProcess/VisitedLinkProvider.cpp
    UIProcess/WebApplicationCacheManagerProxy.cpp
    UIProcess/WebBackForwardList.cpp
    UIProcess/WebContext.cpp
    UIProcess/WebContextInjectedBundleClient.cpp
    UIProcess/WebContextMenuProxy.cpp
    UIProcess/WebCookieManagerProxy.cpp
    UIProcess/WebCookieManagerProxyClient.cpp
    UIProcess/WebDatabaseManagerProxyClient.cpp
    UIProcess/WebDatabaseManagerProxy.cpp
    UIProcess/WebDownloadClient.cpp
    UIProcess/WebEditCommandProxy.cpp
    UIProcess/WebFindClient.cpp
    UIProcess/WebFormClient.cpp
    UIProcess/WebFormSubmissionListenerProxy.cpp
    UIProcess/WebFrameListenerProxy.cpp
    UIProcess/WebFramePolicyListenerProxy.cpp
    UIProcess/WebFrameProxy.cpp
    UIProcess/WebFullScreenManagerProxy.cpp
    UIProcess/WebGeolocationManagerProxy.cpp
    UIProcess/WebGeolocationProvider.cpp
    UIProcess/WebHistoryClient.cpp
    UIProcess/WebIconDatabase.cpp
    UIProcess/WebIconDatabaseClient.cpp
    UIProcess/WebInspectorProxy.cpp
    UIProcess/WebKeyValueStorageManagerProxy.cpp
    UIProcess/WebMediaCacheManagerProxy.cpp
    UIProcess/WebLoaderClient.cpp
    UIProcess/WebNavigationData.cpp
    UIProcess/WebOpenPanelResultListenerProxy.cpp
    UIProcess/WebPageContextMenuClient.cpp
    UIProcess/WebPageGroup.cpp
    UIProcess/WebPageProxy.cpp
    UIProcess/WebPolicyClient.cpp
    UIProcess/WebPreferences.cpp
    UIProcess/WebProcessProxy.cpp
    UIProcess/WebResourceCacheManagerProxy.cpp
    UIProcess/WebResourceLoadClient.cpp
    UIProcess/WebUIClient.cpp

    WebProcess/ApplicationCache/WebApplicationCacheManager.cpp

    WebProcess/Authentication/AuthenticationManager.cpp

    WebProcess/Cookies/WebCookieManager.cpp

    WebProcess/Downloads/Download.cpp
    WebProcess/Downloads/DownloadManager.cpp

    WebProcess/FullScreen/WebFullScreenManager.cpp

    WebProcess/Geolocation/GeolocationPermissionRequestManager.cpp
    WebProcess/Geolocation/WebGeolocationManager.cpp

    WebProcess/IconDatabase/WebIconDatabaseProxy.cpp

    WebProcess/InjectedBundle/API/c/WKBundleBackForwardList.cpp
    WebProcess/InjectedBundle/API/c/WKBundleBackForwardListItem.cpp
    WebProcess/InjectedBundle/API/c/WKBundle.cpp
    WebProcess/InjectedBundle/API/c/WKBundleFrame.cpp
    WebProcess/InjectedBundle/API/c/WKBundleHitTestResult.cpp
    WebProcess/InjectedBundle/API/c/WKBundleNavigationAction.cpp
    WebProcess/InjectedBundle/API/c/WKBundleInspector.cpp
    WebProcess/InjectedBundle/API/c/WKBundleNodeHandle.cpp
    WebProcess/InjectedBundle/API/c/WKBundlePage.cpp
    WebProcess/InjectedBundle/API/c/WKBundlePageGroup.cpp
    WebProcess/InjectedBundle/API/c/WKBundlePageOverlay.cpp
    WebProcess/InjectedBundle/API/c/WKBundleRangeHandle.cpp
    WebProcess/InjectedBundle/API/c/WKBundleScriptWorld.cpp

    WebProcess/InjectedBundle/DOM/InjectedBundleNodeHandle.cpp
    WebProcess/InjectedBundle/DOM/InjectedBundleRangeHandle.cpp

    WebProcess/InjectedBundle/InjectedBundle.cpp
    WebProcess/InjectedBundle/InjectedBundleBackForwardList.cpp
    WebProcess/InjectedBundle/InjectedBundleBackForwardListItem.cpp
    WebProcess/InjectedBundle/InjectedBundleClient.cpp
    WebProcess/InjectedBundle/InjectedBundleHitTestResult.cpp
    WebProcess/InjectedBundle/InjectedBundleNavigationAction.cpp
    WebProcess/InjectedBundle/InjectedBundlePageContextMenuClient.cpp
    WebProcess/InjectedBundle/InjectedBundlePageEditorClient.cpp
    WebProcess/InjectedBundle/InjectedBundlePageFormClient.cpp
    WebProcess/InjectedBundle/InjectedBundlePageLoaderClient.cpp
    WebProcess/InjectedBundle/InjectedBundlePagePolicyClient.cpp
    WebProcess/InjectedBundle/InjectedBundlePageResourceLoadClient.cpp
    WebProcess/InjectedBundle/InjectedBundlePageUIClient.cpp
    WebProcess/InjectedBundle/InjectedBundleScriptWorld.cpp

    WebProcess/KeyValueStorage/WebKeyValueStorageManager.cpp

    WebProcess/MediaCache/WebMediaCacheManager.cpp

    WebProcess/Plugins/Netscape/JSNPMethod.cpp
    WebProcess/Plugins/Netscape/JSNPObject.cpp
    WebProcess/Plugins/Netscape/NetscapeBrowserFuncs.cpp
    WebProcess/Plugins/Netscape/NetscapePlugin.cpp
    WebProcess/Plugins/Netscape/NetscapePluginNone.cpp
    WebProcess/Plugins/Netscape/NetscapePluginStream.cpp
    WebProcess/Plugins/Netscape/NPJSObject.cpp
    WebProcess/Plugins/Netscape/NPRuntimeObjectMap.cpp
    WebProcess/Plugins/Netscape/NPRuntimeUtilities.cpp

    WebProcess/Plugins/Plugin.cpp
    WebProcess/Plugins/PluginProcessConnection.cpp
    WebProcess/Plugins/PluginProcessConnectionManager.cpp
    WebProcess/Plugins/PluginProxy.cpp
    WebProcess/Plugins/PluginView.cpp

    WebProcess/ResourceCache/WebResourceCacheManager.cpp

    WebProcess/WebCoreSupport/WebChromeClient.cpp
    WebProcess/WebCoreSupport/WebContextMenuClient.cpp
    WebProcess/WebCoreSupport/WebDatabaseManager.cpp
    WebProcess/WebCoreSupport/WebDragClient.cpp
    WebProcess/WebCoreSupport/WebEditorClient.cpp
    WebProcess/WebCoreSupport/WebFrameLoaderClient.cpp
    WebProcess/WebCoreSupport/WebGeolocationClient.cpp
    WebProcess/WebCoreSupport/WebInspectorClient.cpp
    WebProcess/WebCoreSupport/WebInspectorFrontendClient.cpp
    WebProcess/WebCoreSupport/WebPlatformStrategies.cpp
    WebProcess/WebCoreSupport/WebPopupMenu.cpp
    WebProcess/WebCoreSupport/WebSearchPopupMenu.cpp

    WebProcess/WebPage/DecoderAdapter.cpp
    WebProcess/WebPage/DrawingArea.cpp
    WebProcess/WebPage/DrawingAreaImpl.cpp
    WebProcess/WebPage/EncoderAdapter.cpp
    WebProcess/WebPage/FindController.cpp
    WebProcess/WebPage/LayerTreeHost.cpp
    WebProcess/WebPage/PageOverlay.cpp
    WebProcess/WebPage/TiledDrawingArea.cpp
    WebProcess/WebPage/WebBackForwardListProxy.cpp
    WebProcess/WebPage/WebContextMenu.cpp
    WebProcess/WebPage/WebEditCommand.cpp
    WebProcess/WebPage/WebFrame.cpp
    WebProcess/WebPage/WebInspector.cpp
    WebProcess/WebPage/WebOpenPanelResultListener.cpp
    WebProcess/WebPage/WebPage.cpp
    WebProcess/WebPage/WebPageGroupProxy.cpp

    WebProcess/WebProcess.cpp
)

SET(WebKit2_MESSAGES_IN_FILES
    UIProcess/WebMediaCacheManagerProxy.messages.in
    UIProcess/WebCookieManagerProxy.messages.in
    UIProcess/Plugins/PluginProcessProxy.messages.in
    UIProcess/WebInspectorProxy.messages.in
    UIProcess/WebFullScreenManagerProxy.messages.in
    UIProcess/WebDatabaseManagerProxy.messages.in
    UIProcess/WebPageProxy.messages.in
    UIProcess/WebIconDatabase.messages.in
    UIProcess/Downloads/DownloadProxy.messages.in
    UIProcess/WebContext.messages.in
    UIProcess/WebGeolocationManagerProxy.messages.in
    UIProcess/DrawingAreaProxy.messages.in
    UIProcess/WebKeyValueStorageManagerProxy.messages.in
    UIProcess/WebResourceCacheManagerProxy.messages.in
    UIProcess/WebProcessProxy.messages.in
    UIProcess/WebApplicationCacheManagerProxy.messages.in
    PluginProcess/WebProcessConnection.messages.in
    PluginProcess/PluginControllerProxy.messages.in
    PluginProcess/PluginProcess.messages.in
    Shared/Plugins/NPObjectMessageReceiver.messages.in
    WebProcess/ApplicationCache/WebApplicationCacheManager.messages.in
    WebProcess/MediaCache/WebMediaCacheManager.messages.in
    WebProcess/Plugins/PluginProxy.messages.in
    WebProcess/WebProcess.messages.in
    WebProcess/Geolocation/WebGeolocationManager.messages.in
    WebProcess/WebCoreSupport/WebDatabaseManager.messages.in
    WebProcess/IconDatabase/WebIconDatabaseProxy.messages.in
    WebProcess/Authentication/AuthenticationManager.messages.in
    WebProcess/ResourceCache/WebResourceCacheManager.messages.in
    WebProcess/FullScreen/WebFullScreenManager.messages.in
    WebProcess/Cookies/WebCookieManager.messages.in
    WebProcess/KeyValueStorage/WebKeyValueStorageManager.messages.in
    WebProcess/WebPage/WebPage.messages.in
    WebProcess/WebPage/WebInspector.messages.in
    WebProcess/WebPage/DrawingArea.messages.in
)

# Create JavaScript C++ code given an IDL input
FOREACH (_file ${WebKit2_MESSAGES_IN_FILES})
    GET_FILENAME_COMPONENT (_name ${_file} NAME_WE)
    ADD_CUSTOM_COMMAND(
        OUTPUT ${DERIVED_SOURCES_WEBKIT2_DIR}/${_name}MessageReceiver.cpp ${DERIVED_SOURCES_WEBKIT2_DIR}/${_name}Messages.h
        MAIN_DEPENDENCY ${_file}
        COMMAND ${PYTHON_EXECUTABLE} ${WEBKIT2_DIR}/Scripts/generate-message-receiver.py ${_file} > ${DERIVED_SOURCES_WEBKIT2_DIR}/${_name}MessageReceiver.cpp
        COMMAND ${PYTHON_EXECUTABLE} ${WEBKIT2_DIR}/Scripts/generate-messages-header.py ${_file} > ${DERIVED_SOURCES_WEBKIT2_DIR}/${_name}Messages.h
        WORKING_DIRECTORY ${WEBKIT2_DIR}
        VERBATIM)

    LIST(APPEND WebKit2_SOURCES ${DERIVED_SOURCES_WEBKIT2_DIR}/${_name}MessageReceiver.cpp)
ENDFOREACH ()

SET(WebKit2_LIBRARIES
    ${WebCore_LIBRARY_NAME}
)

SET(WebProcess_NAME ../Programs/WebProcess)
SET(WebProcess_SOURCES "")

SET(WebProcess_LIBRARIES
    ${JavaScriptCore_LIBRARY_NAME}
    ${WebCore_LIBRARY_NAME}
    ${WebKit2_LIBRARY_NAME}
)

SET(ForwardingHeaders_NAME )
SET(ForwardingNetworkHeaders_NAME )
INCLUDE_IF_EXISTS(${WEBKIT2_DIR}/CMakeLists${PORT}.txt)

ADD_DEFINITIONS(-DBUILDING_WEBKIT)
ADD_DEFINITIONS(-DWTF_USE_JSC=1)
INCLUDE_DIRECTORIES(${WebKit2_INCLUDE_DIRECTORIES})
ADD_LIBRARY(${WebKit2_LIBRARY_NAME} ${WebKit2_LIBRARY_TYPE} ${WebKit2_SOURCES})

ADD_DEPENDENCIES(${WebKit2_LIBRARY_NAME} ${WebCore_LIBRARY_NAME})
ADD_DEPENDENCIES(${WebKit2_LIBRARY_NAME} ${ForwardingHeaders_NAME})
ADD_DEPENDENCIES(${WebKit2_LIBRARY_NAME} ${ForwardingNetworkHeaders_NAME})
TARGET_LINK_LIBRARIES(${WebKit2_LIBRARY_NAME} ${WebKit2_LIBRARIES})

ADD_EXECUTABLE(${WebProcess_NAME} ${WebProcess_SOURCES})
TARGET_LINK_LIBRARIES(${WebProcess_NAME} ${WebProcess_LIBRARIES})

SET_TARGET_PROPERTIES(${WebKit2_LIBRARY_NAME} PROPERTIES VERSION ${PROJECT_VERSION} SOVERSION ${PROJECT_VERSION_MAJOR})
IF (WebKit2_LINK_FLAGS)
    ADD_TARGET_PROPERTIES(${WebKit2_LIBRARY_NAME} LINK_FLAGS "${WebKit2_LINK_FLAGS}")
    ADD_TARGET_PROPERTIES(${WebProcess_NAME} LINK_FLAGS "${WebKit2_LINK_FLAGS}")
ENDIF ()

INSTALL(TARGETS ${WebKit2_LIBRARY_NAME} DESTINATION lib)

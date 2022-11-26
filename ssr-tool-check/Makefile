# SPDX-License-Identifier: GPL-2.0-only
#
# Copyright (C) 2017-2020 Yousong Zhou <yszhou4tech@gmail.com>
# Copyright (C) 2018 Lean <coolsnowwolf@gmail.com>
# Copyright (C) 2021 ImmortalWrt.org

include $(TOPDIR)/rules.mk

PKG_NAME:=ssr-tool-check
PKG_VERSION:=0.0.1
PKG_RELEASE:=1

PKG_LICENSE:=GPL-3.0
PKG_LICENSE_FILES:=LICENSE

PKG_USE_MIPS16:=0
PKG_BUILD_PARALLEL:=1
PKG_INSTALL:=1

include $(INCLUDE_DIR)/package.mk

define Package/ssr-tool-check
  SECTION:=net
  CATEGORY:=Network
  SUBMENU:=Web Servers/Proxies
  TITLE:=ssr-tool-check ssr-check
  URL:=https://github.com/shadowsocksrr/shadowsocksr-libev
endef

define Package/ssr-tool-check/install
  $(INSTALL_DIR) $(1)/usr/bin
  $(INSTALL_BIN) $(PKG_INSTALL_DIR)/usr/bin/ss-check $(1)/usr/bin/ssr-check
endef

$(eval $(call BuildPackage,ssr-tool-check))

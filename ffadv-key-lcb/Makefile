#
# Copyright (C) 2006-2012 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

# Package content copyright (C) 
#      2012 Freifunk Rheinland e. V. <http://www.freifunk-rheinland.net/>


include $(TOPDIR)/rules.mk

PKG_NAME:=ffadv-key-lcb
PKG_VERSION:=20120624
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/ffadv-key-lcb
  SECTION:=base
  CATEGORY:=Utilities
  SUBMENU:=Freifunk Advanced
  PKGARCH:=all
  DEFAULT:=n
  TITLE:=SSH maintenance key (FFNE lcb)
  MAINTAINER:=Linus Broich <cyrus@lambdacore.de>
  URL:=http://freifunk-rheinland.net
  DEPENDS:=+dropbear
endef

define Package/ffadv-key-lcb/description
  SSH key for maintenance
endef

define Build/Prepare
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffadv-key-lcb/install
	mkdir -p $(1)/CONTROL
	$(INSTALL_BIN) ./ipkg/ffadv-key-lcb.postinst $(1)/CONTROL/postinst
	$(INSTALL_BIN) ./ipkg/ffadv-key-lcb.postrm $(1)/CONTROL/postrm
endef

$(eval $(call BuildPackage,ffadv-key-lcb))

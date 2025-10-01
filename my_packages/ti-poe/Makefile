include $(TOPDIR)/rules.mk

PKG_NAME:=ti-poe
PKG_VERSION:=1.0
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/SolidRun/ti-poe.git
PKG_SOURCE_PROTO:=git
PKG_SOURCE_VERSION:=8dfc35df52cb606c972cbb06d464148079a92b6b
PKG_MIRROR_HASH:=56cd7fd5c78b62f006cba20a1cefaf4a4a66d570ef9a2454904028161999ea9e

PKG_MAINTAINER:=Alexey Belyaev <spider@spider.vc>

include $(INCLUDE_DIR)/package.mk

define Package/ti-poe
  SECTION:=net
  CATEGORY:=Utilities
  TITLE:=ti-poe Linux port of TI TPS23880 firmware upload and monitor code
  URL:=https://github.com/SolidRun/ti-poe.git
  DEPENDS:=+kmod-i2c-core
endef

define Package/ti-poe/description
  Linux port of TI TPS23880 firmware upload and monitor code
endef

define Package/ti-poe/install
	$(INSTALL_DIR) $(1)/usr/bin
endef

define Build/Prepare
	$(call Build/Prepare/Default)
endef

$(eval $(call BuildPackage,ti-poe))

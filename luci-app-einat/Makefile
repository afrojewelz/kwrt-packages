# SPDX-License-Identifier: MIT
#
# Copyright (C) 2024-2025 Anya Lin <https://github.com/muink>

include $(TOPDIR)/rules.mk

LUCI_NAME:=luci-app-einat

LUCI_TITLE:=LuCI Support for einat
LUCI_PKGARCH:=all
LUCI_DEPENDS:=+einat-ebpf

LUCI_DESCRIPTION:=eBPF-based Endpoint-Independent NAT

PKG_MAINTAINER:=Anya Lin <hukk1996@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

PKG_UNPACK=$(CURDIR)/.prepare.sh $(PKG_NAME) $(CURDIR) $(PKG_BUILD_DIR)

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature

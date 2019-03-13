sdFAT FS support for Linux Kernel 4.4 & 5.0
=====================================

sdFAT is unified FAT-based filesystem which supports FAT12/16/32(VFAT)/64(exFAT). sdFAT supports winnt short-name rule.

Suggested Kernel config:

    CONFIG_SDFAT_FS=y
    CONFIG_SDFAT_DELAYED_META_DIRTY=y
    CONFIG_SDFAT_SUPPORT_DIR_SYNC=y
    CONFIG_SDFAT_DEFAULT_CODEPAGE=437
    CONFIG_SDFAT_DEFAULT_IOCHARSET="utf8"
    CONFIG_SDFAT_ALIGNED_MPAGE_WRITE=y
    CONFIG_SDFAT_VIRTUAL_XATTR=y
    CONFIG_SDFAT_VIRTUAL_XATTR_SELINUX_LABEL="u:object_r:vfat:s0"
    CONFIG_SDFAT_DEBUG=y
    CONFIG_SDFAT_DBG_MSG=y
    CONFIG_SDFAT_STATISTICS=y

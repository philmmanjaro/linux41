# Based on the file created for Arch Linux by:
# Tobias Powalowski <tpowa@archlinux.org>
# Thomas Baechler <thomas@archlinux.org>

# Maintainer: Philip Müller <philm@manjaro.org>
# Maintainer: Guinux <guillaume@manjaro.org>
# Maintainer: Rob McCathie <rob@manjaro.org>

pkgbase=linux41
pkgname=('linux41' 'linux41-headers')
_kernelname=-MANJARO
_basekernel=4.1
_basever=41
_aufs=20150629
_bfq=v7r8
_rc=rc0.b12.cecae36074
_bisect=cecae360744d958c0af562e806dbd4632be13efc
pkgver=${_basekernel}${_rc}
pkgrel=1
arch=('i686' 'x86_64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('xmlto' 'docbook-xsl' 'kmod' 'inetutils' 'bc')
options=('!strip')
source=("$pkgbase-$pkgver.tar.gz::https://github.com/torvalds/linux/archive/$_bisect.tar.gz"
        #"https://www.kernel.org/pub/linux/kernel/v4.x/testing/linux-${_basekernel}-${_rc}.tar.xz"
        #"https://www.kernel.org/pub/linux/kernel/v4.x/linux-${_basekernel}.tar.xz"
        #"http://www.kernel.org/pub/linux/kernel/v4.x/patch-${pkgver}.xz"
        # the main kernel config files
        'config' 'config.x86_64' 'config.aufs'
        # standard config files for mkinitcpio ramdisk
        "${pkgname}.preset"
        "aufs4.1-${_aufs}.patch.bz2"
        'aufs4-base.patch'
        'aufs4-kbuild.patch'
        'aufs4-loopback.patch'
        'aufs4-mmap.patch'
        'aufs4-standalone.patch'
        'tmpfs-idr.patch'
        'vfs-ino.patch'
        'http://sources.gentoo.org/cgi-bin/viewvc.cgi/linux-patches/genpatches-2.6/trunk/3.15/1700_enable-thinkpad-micled.patch'
        'http://sources.gentoo.org/cgi-bin/viewvc.cgi/linux-patches/genpatches-2.6/trunk/3.15/2700_ThinkPad-30-brightness-control-fix.patch'
        "0001-block-cgroups-kconfig-build-bits-for-BFQ-${_bfq}.patch::ftp://teambelgium.net/bfq/patches/4.0.0-${_bfq}/0001-block-cgroups-kconfig-build-bits-for-BFQ-${_bfq}-4.0.patch"
        "0002-block-introduce-the-BFQ-${_bfq}-I-O-sched.patch::ftp://teambelgium.net/bfq/patches/4.0.0-${_bfq}/0002-block-introduce-the-BFQ-${_bfq}-I-O-sched-for-4.0.patch"
        "0003-block-bfq-add-Early-Queue-Merge-EQM-to-BFQ-${_bfq}.patch::ftp://teambelgium.net/bfq/patches/4.0.0-${_bfq}/0003-block-bfq-add-Early-Queue-Merge-EQM-to-BFQ-${_bfq}-for-4.0.0.patch"
        # ARCH Patches
        'change-default-console-loglevel.patch'
        '0001-block-loop-convert-to-per-device-workqueue.patch'
        '0002-block-loop-avoiding-too-many-pending-per-work-I-O.patch'
        '0003-bluetooth-btbcm-allow-btbcm_read_verbose_config-to-f.patch'
        '0004-bitmap-enable-booting-for-dm-md-raid1.patch'
)
sha256sums=('e5785385a88e77ac8c3e45ddbeb30e0f897ebb4954b10f2dc11827ee76910291'
            'ac1e6e6d4a03a080bef97987364f08b8c3d7af4e6ba95215a1b32305591b9e85'
            '3435ad970f6fc9b7ac9c026a69fb8c6805675a6ac0c1027bf6fd3cc5ef26d7f2'
            'd1cecc720df66c70f43bdb86e0169d6b756161c870db8d7d39c32c04dc36ed36'
            '6d058de24e029651eef6e7e0133616eddf710aa51dfbba1652026f57a35e42ad'
            '58c9b0fdbbb5ec33d337a3bcf80b68b0b97b5c0a28dfc351e0950db9a2958e3a'
            'b20a0ddb146d1e7e861dbdf1c6f99b92a822ff975e30fff8f3cea29e257fcfb9'
            '68baa54faa3dbb76522b1f311c8b4e780e4244836c1ae5396a8d943842ee80a7'
            '56b136946bbdc29e0cbd88a9ecba125e37049e9febc262b69958e7e533f93e63'
            '1743a764597b0bdcb967f502c517d10e46ec05fbb9217ae4813d2739477ecbfc'
            '99febb7e7399ea6237b42bb07e2fc877ab9eaa1d68339839ed958ad4ac248a74'
            '1f64e8e78169bc7b3658e2e948cea9d88724cef419b6e9af25101e247796cd5a'
            '9129c349305fa1d003bd47fdf11a768a69805c852a3c269af5a04f0d6f50eeea'
            '461aa0da7de8bda9474797339532304894b55825be34f8c009244da8c00c5b41'
            'a3f85c3c35ee478fd174f8aaa6ca15e5fad8612b42ca4d90cc3ef79b49a99989'
            'ec0ca3c8051ea6d9a27a450998af8162464c224299deefc29044172940e96975'
            'c5c2c48638c2a8180948bd118ffcc33c8b7ff5f9f1e4b04c8e2cafeca2bde87b'
            '4f30f76adbdf49aec8d41ac27ad212734500c272f3cba594f134a7bc263820d9'
            '44e7e15c95af9676f715569e72688fd64304a70d2854b0f804c156d4961c72c0'
            '9e1d3fd95d768a46353593f6678513839cedb98ee66e83d9323233104ec3b23f'
            'bbe3631c737ed8329a1b7a9610cc0a07330c14194da5e9afec7705e7f37eeb81'
            '08f69d122021e1d13c31e5987c23021916a819846c47247b3f1cee2ef99d7f82'
            '959c4d71b5dc50434eeecf3a8608758f57f111c6e999289c435b13fc8c6be5f0')

prepare() {
  #cd "${srcdir}/linux-${_basekernel}-${_rc}"
  cd "${srcdir}/linux-${_bisect}"

  # add upstream patch
  #patch -p1 -i "${srcdir}/patch-${pkgver}"

  # add latest fixes from stable queue, if needed
  # http://git.kernel.org/?p=linux/kernel/git/stable/stable-queue.git
  # enable only if you have "gen-stable-queue-patch.sh" executed before
  #patch -Np1 -i "${srcdir}/prepatch-${_basekernel}`date +%Y%m%d`"

  # Fix deadlock with stacked loop devices (FS#45129)
  # http://marc.info/?l=linux-kernel&m=143280649731902&w=2
  #patch -Np1 -i ../0001-block-loop-convert-to-per-device-workqueue.patch
  #patch -Np1 -i ../0002-block-loop-avoiding-too-many-pending-per-work-I-O.patch

  # Fix bluetooth chip initialization on some macbooks (FS#45554)
  # http://marc.info/?l=linux-bluetooth&m=143690738728402&w=2
  # https://bugzilla.kernel.org/show_bug.cgi?id=100651
  #patch -Np1 -i ../0003-bluetooth-btbcm-allow-btbcm_read_verbose_config-to-f.patch

  # Fix kernel oops when booting with root on RAID1 LVM (FS#45548)
  # https://bugzilla.kernel.org/show_bug.cgi?id=100491#c24
  #patch -Np1 -i ../0004-bitmap-enable-booting-for-dm-md-raid1.patch

  # set DEFAULT_CONSOLE_LOGLEVEL to 4 (same value as the 'quiet' kernel param)
  # remove this when a Kconfig knob is made available by upstream
  # (relevant patch sent upstream: https://lkml.org/lkml/2011/7/26/227)
  patch -p1 -i "${srcdir}/change-default-console-loglevel.patch"

  # add Gentoo patches
  patch -Np1 -i "${srcdir}/1700_enable-thinkpad-micled.patch"
  patch -Np1 -i "${srcdir}/2700_ThinkPad-30-brightness-control-fix.patch"

  # fix aufs4
  sed -i -e 's|f_dentry|f_path.dentry|g' "${srcdir}/aufs4-loopback.patch"

  # add aufs4 support
  #patch -Np1 -i "${srcdir}/aufs4.1-${_aufs}.patch"
  #patch -Np1 -i "${srcdir}/aufs4-base.patch"
  #patch -Np1 -i "${srcdir}/aufs4-kbuild.patch"
  #patch -Np1 -i "${srcdir}/aufs4-loopback.patch"
  #patch -Np1 -i "${srcdir}/aufs4-mmap.patch"
  #patch -Np1 -i "${srcdir}/aufs4-standalone.patch"
  #patch -Np1 -i "${srcdir}/tmpfs-idr.patch"
  #patch -Np1 -i "${srcdir}/vfs-ino.patch"

  # add BFQ scheduler
  patch -Np1 -i "${srcdir}/0001-block-cgroups-kconfig-build-bits-for-BFQ-${_bfq}.patch"
  patch -Np1 -i "${srcdir}/0002-block-introduce-the-BFQ-${_bfq}-I-O-sched.patch"
  patch -Np1 -i "${srcdir}/0003-block-bfq-add-Early-Queue-Merge-EQM-to-BFQ-${_bfq}.patch"

  if [ "${CARCH}" = "x86_64" ]; then
    cat "${srcdir}/config.x86_64" > ./.config
  else
    cat "${srcdir}/config" > ./.config
  fi

  cat "${srcdir}/config.aufs" >> ./.config

  if [ "${_kernelname}" != "" ]; then
    sed -i "s|CONFIG_LOCALVERSION=.*|CONFIG_LOCALVERSION=\"${_kernelname}\"|g" ./.config
    sed -i "s|CONFIG_LOCALVERSION_AUTO=.*|CONFIG_LOCALVERSION_AUTO=n|" ./.config
  fi

  # set extraversion to pkgrel
  sed -ri "s|^(EXTRAVERSION =).*|\1 -${pkgrel}|" Makefile

  # don't run depmod on 'make install'. We'll do this ourselves in packaging
  sed -i '2iexit 0' scripts/depmod.sh

  # normally not needed
  make clean

  # get kernel version
  make prepare

  # load configuration
  # Configure the kernel. Replace the line below with one of your choice.
  #make menuconfig # CLI menu for configuration
  #make nconfig # new CLI menu for configuration
  #make xconfig # X-based configuration
  #make oldconfig # using old config from previous kernel version
  # ... or manually edit .config

  # rewrite configuration
  yes "" | make config >/dev/null
}

build() {
  #cd "${srcdir}/linux-${_basekernel}-${_rc}"
  cd "${srcdir}/linux-${_bisect}"

  # build!
  make ${MAKEFLAGS} LOCALVERSION= bzImage modules
}

package_linux41() {
  pkgdesc="The ${pkgbase/linux/Linux} kernel and modules"
  depends=('coreutils' 'linux-firmware' 'kmod' 'mkinitcpio>=0.7')
  optdepends=('crda: to set the correct wireless channels of your country')
  provides=("linux=${pkgver}")
  install=${pkgname}.install

  #cd "${srcdir}/linux-${_basekernel}-${_rc}"
  cd "${srcdir}/linux-${_bisect}"

  KARCH=x86

  # get kernel version
  _kernver="$(make LOCALVERSION= kernelrelease)"

  mkdir -p "${pkgdir}"/{lib/modules,lib/firmware,boot}
  make LOCALVERSION= INSTALL_MOD_PATH="${pkgdir}" modules_install
  cp arch/$KARCH/boot/bzImage "${pkgdir}/boot/vmlinuz-${_basekernel}-${CARCH}"

  # add kernel version
  if [ "${CARCH}" = "x86_64" ]; then
     echo "${pkgver}-${pkgrel}-MANJARO x64" > "${pkgdir}/boot/${pkgbase}-${CARCH}.kver"
  else
     echo "${pkgver}-${pkgrel}-MANJARO x32" > "${pkgdir}/boot/${pkgbase}-${CARCH}.kver"
  fi

  # set correct depmod command for install
  cp -f "${startdir}/${install}" "${startdir}/${install}.pkg"
  true && install=${install}.pkg
  sed \
    -e  "s/RELEASE=.*/RELEASE=${pkgver}-${pkgrel}/g" \
    -e  "s/KERNEL_VERSION=.*/KERNEL_VERSION=${_kernver}/g" \
    -e  "s/KERNEL_BASE=.*/KERNEL_BASE=${_basekernel}/g" \
    -e  "s/BASEVER=.*/BASEVER=${_basever}/g" \
    -e  "s/ARCH=.*/ARCH=${CARCH}/g" \
    -i "${startdir}/${install}"

  # install mkinitcpio preset file for kernel
  install -D -m644 "${srcdir}/${pkgname}.preset" "${pkgdir}/etc/mkinitcpio.d/${pkgbase}.preset"
  sed \
    -e "s|ALL_kver=.*|ALL_kver=\"/boot/vmlinuz-${_basekernel}-${CARCH}\"|g" \
    -e "s|default_image=.*|default_image=\"/boot/initramfs-${_basekernel}-${CARCH}.img\"|g" \
    -e "s|fallback_image=.*|fallback_image=\"/boot/initramfs-${_basekernel}-${CARCH}-fallback.img\"|g" \
    -i "${pkgdir}/etc/mkinitcpio.d/${pkgname}.preset"

  # remove build and source links
  rm -f "${pkgdir}"/lib/modules/${_kernver}/{source,build}
  # remove the firmware
  rm -rf "${pkgdir}/lib/firmware"
  # gzip -9 all modules to save 100MB of space
  find "${pkgdir}" -name '*.ko' -exec gzip -9 {} \;
  # make room for external modules
  ln -s "../extramodules-${_basekernel}${_kernelname:--MANJARO}" "${pkgdir}/lib/modules/${_kernver}/extramodules"
  # add real version for building modules and running depmod from post_install/upgrade
  mkdir -p "${pkgdir}/lib/modules/extramodules-${_basekernel}${_kernelname:--MANJARO}"
  echo "${_kernver}" > "${pkgdir}/lib/modules/extramodules-${_basekernel}${_kernelname:--MANJARO}/version"

  # Now we call depmod...
  depmod -b "${pkgdir}" -F System.map "${_kernver}"

  # move module tree /lib -> /usr/lib
  mkdir -p "${pkgdir}/usr"
  mv "${pkgdir}/lib" "${pkgdir}/usr/"

  # add vmlinux
  install -D -m644 vmlinux "${pkgdir}/usr/lib/modules/${_kernver}/build/vmlinux" 
}

package_linux41-headers() {
  pkgdesc="Header files and scripts for building modules for ${pkgbase/linux/Linux} kernel"
  provides=("linux-headers=$pkgver")

  install -dm755 "${pkgdir}/usr/lib/modules/${_kernver}"

  #cd "${srcdir}/linux-${_basekernel}-${_rc}"
  cd "${srcdir}/linux-${_bisect}"

  install -D -m644 Makefile \
    "${pkgdir}/usr/lib/modules/${_kernver}/build/Makefile"
  install -D -m644 kernel/Makefile \
    "${pkgdir}/usr/lib/modules/${_kernver}/build/kernel/Makefile"
  install -D -m644 .config \
    "${pkgdir}/usr/lib/modules/${_kernver}/build/.config"

  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/include"

  for i in acpi asm-generic config crypto drm generated keys linux math-emu \
    media net pcmcia scsi sound trace uapi video xen; do
    cp -a include/${i} "${pkgdir}/usr/lib/modules/${_kernver}/build/include/"
  done

  # copy arch includes for external modules
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/arch/x86"
  cp -a arch/x86/include "${pkgdir}/usr/lib/modules/${_kernver}/build/arch/x86/"

  # copy files necessary for later builds, like nvidia and vmware
  cp Module.symvers "${pkgdir}/usr/lib/modules/${_kernver}/build"
  cp -a scripts "${pkgdir}/usr/lib/modules/${_kernver}/build"

  # fix permissions on scripts dir
  chmod og-w -R "${pkgdir}/usr/lib/modules/${_kernver}/build/scripts"
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/.tmp_versions"

  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/arch/${KARCH}/kernel"

  cp arch/${KARCH}/Makefile "${pkgdir}/usr/lib/modules/${_kernver}/build/arch/${KARCH}/"

  if [ "${CARCH}" = "i686" ]; then
    cp arch/${KARCH}/Makefile_32.cpu "${pkgdir}/usr/lib/modules/${_kernver}/build/arch/${KARCH}/"
  fi

  cp arch/${KARCH}/kernel/asm-offsets.s "${pkgdir}/usr/lib/modules/${_kernver}/build/arch/${KARCH}/kernel/"

  # add docbook makefile
  install -D -m644 Documentation/DocBook/Makefile \
    "${pkgdir}/usr/lib/modules/${_kernver}/build/Documentation/DocBook/Makefile"

  # add dm headers
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/md"
  cp drivers/md/*.h "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/md"

  # add inotify.h
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/include/linux"
  cp include/linux/inotify.h "${pkgdir}/usr/lib/modules/${_kernver}/build/include/linux/"

  # add wireless headers
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/net/mac80211/"
  cp net/mac80211/*.h "${pkgdir}/usr/lib/modules/${_kernver}/build/net/mac80211/"

  # add dvb headers for external modules
  # in reference to:
  # http://bugs.archlinux.org/task/9912
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/dvb-core"
  cp drivers/media/dvb-core/*.h "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/dvb-core/"
  # and...
  # http://bugs.archlinux.org/task/11194
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/include/config/dvb/"
  cp include/config/dvb/*.h "${pkgdir}/usr/lib/modules/${_kernver}/build/include/config/dvb/"

  # add dvb headers for http://mcentral.de/hg/~mrec/em28xx-new
  # in reference to:
  # http://bugs.archlinux.org/task/13146
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/dvb-frontends/"
  cp drivers/media/dvb-frontends/lgdt330x.h "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/dvb-frontends/"
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/i2c/"
  cp drivers/media/i2c/msp3400-driver.h "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/i2c/"

  # add dvb headers
  # in reference to:
  # http://bugs.archlinux.org/task/20402
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/usb/dvb-usb"
  cp drivers/media/usb/dvb-usb/*.h "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/usb/dvb-usb/"
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/dvb-frontends"
  cp drivers/media/dvb-frontends/*.h "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/dvb-frontends/"
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/tuners"
  cp drivers/media/tuners/*.h "${pkgdir}/usr/lib/modules/${_kernver}/build/drivers/media/tuners/"

  # add xfs and shmem for aufs building
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/fs/xfs/libxfs"
  mkdir -p "${pkgdir}/usr/lib/modules/${_kernver}/build/mm"
  cp fs/xfs/libxfs/xfs_sb.h "${pkgdir}/usr/lib/modules/${_kernver}/build/fs/xfs/libxfs/xfs_sb.h"

  # copy in Kconfig files
  for i in $(find . -name "Kconfig*"); do
    mkdir -p "${pkgdir}"/usr/lib/modules/${_kernver}/build/`echo ${i} | sed 's|/Kconfig.*||'`
    cp ${i} "${pkgdir}/usr/lib/modules/${_kernver}/build/${i}"
  done

  chown -R root.root "${pkgdir}/usr/lib/modules/${_kernver}/build"
  find "${pkgdir}/usr/lib/modules/${_kernver}/build" -type d -exec chmod 755 {} \;

  # strip scripts directory
  find "${pkgdir}/usr/lib/modules/${_kernver}/build/scripts" -type f -perm -u+w 2>/dev/null | while read binary ; do
    case "$(file -bi "${binary}")" in
      *application/x-sharedlib*) # Libraries (.so)
        /usr/bin/strip ${STRIP_SHARED} "${binary}";;
      *application/x-archive*) # Libraries (.a)
        /usr/bin/strip ${STRIP_STATIC} "${binary}";;
      *application/x-executable*) # Binaries
        /usr/bin/strip ${STRIP_BINARIES} "${binary}";;
    esac
  done

  # remove unneeded architectures
  rm -rf "${pkgdir}"/usr/lib/modules/${_kernver}/build/arch/{alpha,arc,arm,arm26,arm64,avr32,blackfin,c6x,cris,frv,h8300,hexagon,ia64,m32r,m68k,m68knommu,metag,mips,microblaze,mn10300,openrisc,parisc,powerpc,ppc,s390,score,sh,sh64,sparc,sparc64,tile,unicore32,um,v850,xtensa}
}

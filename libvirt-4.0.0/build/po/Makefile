# Makefile for PO directory in any package using GNU gettext.
# Copyright (C) 1995-1997, 2000-2007 by Ulrich Drepper <drepper@gnu.ai.mit.edu>
#
# This file can be copied and used freely without restrictions.  It can
# be used in projects which are not available under the GNU General Public
# License but which still want to provide support for the GNU gettext
# functionality.
# Please note that the actual code of GNU gettext is covered by the GNU
# General Public License and is *not* in the public domain.
#
# Origin: gettext-0.17
GETTEXT_MACRO_VERSION = 0.17

PACKAGE = libvirt
VERSION = 4.0.0
PACKAGE_BUGREPORT = libvir-list@redhat.com

SHELL = /bin/sh


srcdir = ../../po
top_srcdir = ../..
VPATH = ../../po

prefix = /usr
exec_prefix = ${prefix}
datarootdir = ${prefix}/share
datadir = ${datarootdir}
localedir = ${datarootdir}/locale
gettextsrcdir = $(datadir)/gettext/po

INSTALL = /usr/bin/install -c
INSTALL_DATA = ${INSTALL} -m 644

# We use $(mkdir_p).
# In automake <= 1.9.x, $(mkdir_p) is defined either as "mkdir -p --" or as
# "$(mkinstalldirs)" or as "$(install_sh) -d". For these automake versions,
# ${SHELL} /home/v-jiezhao/libvirt-4.0.0/build-aux/install-sh does not start with $(SHELL), so we add it.
# In automake >= 1.10, /bin/mkdir -p is derived from ${MKDIR_P}, which is defined
# either as "/path/to/mkdir -p" or ".../install-sh -c -d". For these automake
# versions, $(mkinstalldirs) and $(install_sh) are unused.
mkinstalldirs = $(SHELL) ${SHELL} /home/v-jiezhao/libvirt-4.0.0/build-aux/install-sh -d
install_sh = $(SHELL) ${SHELL} /home/v-jiezhao/libvirt-4.0.0/build-aux/install-sh
MKDIR_P = /bin/mkdir -p
mkdir_p = /bin/mkdir -p

GMSGFMT_ = :
GMSGFMT_no = :
GMSGFMT_yes = :
GMSGFMT = $(GMSGFMT_$(USE_MSGCTXT))
MSGFMT_ = :
MSGFMT_no = :
MSGFMT_yes = :
MSGFMT = $(MSGFMT_$(USE_MSGCTXT))
XGETTEXT_ = :
XGETTEXT_no = :
XGETTEXT_yes = :
XGETTEXT = $(XGETTEXT_$(USE_MSGCTXT))
MSGMERGE = msgmerge
MSGMERGE_UPDATE = : --update
MSGINIT = msginit
MSGCONV = msgconv
MSGFILTER = msgfilter

POFILES =  $(srcdir)/af.po $(srcdir)/am.po $(srcdir)/anp.po $(srcdir)/ar.po $(srcdir)/as.po $(srcdir)/ast.po $(srcdir)/bal.po $(srcdir)/be.po $(srcdir)/bg.po $(srcdir)/bn.po $(srcdir)/bn_IN.po $(srcdir)/bo.po $(srcdir)/br.po $(srcdir)/brx.po $(srcdir)/bs.po $(srcdir)/ca.po $(srcdir)/cs.po $(srcdir)/cy.po $(srcdir)/da.po $(srcdir)/de.po $(srcdir)/de_CH.po $(srcdir)/el.po $(srcdir)/en_GB.po $(srcdir)/eo.po $(srcdir)/es.po $(srcdir)/et.po $(srcdir)/eu.po $(srcdir)/fa.po $(srcdir)/fi.po $(srcdir)/fr.po $(srcdir)/gl.po $(srcdir)/gu.po $(srcdir)/he.po $(srcdir)/hi.po $(srcdir)/hr.po $(srcdir)/hu.po $(srcdir)/ia.po $(srcdir)/id.po $(srcdir)/ilo.po $(srcdir)/is.po $(srcdir)/it.po $(srcdir)/ja.po $(srcdir)/ka.po $(srcdir)/kk.po $(srcdir)/km.po $(srcdir)/kn.po $(srcdir)/ko.po $(srcdir)/kw.po $(srcdir)/kw@kkcor.po $(srcdir)/kw@uccor.po $(srcdir)/kw_GB.po $(srcdir)/ky.po $(srcdir)/lt.po $(srcdir)/lv.po $(srcdir)/mai.po $(srcdir)/mk.po $(srcdir)/ml.po $(srcdir)/mn.po $(srcdir)/mr.po $(srcdir)/ms.po $(srcdir)/nb.po $(srcdir)/nds.po $(srcdir)/ne.po $(srcdir)/nl.po $(srcdir)/nn.po $(srcdir)/nso.po $(srcdir)/or.po $(srcdir)/pa.po $(srcdir)/pl.po $(srcdir)/pt.po $(srcdir)/pt_BR.po $(srcdir)/ro.po $(srcdir)/ru.po $(srcdir)/si.po $(srcdir)/sk.po $(srcdir)/sl.po $(srcdir)/sq.po $(srcdir)/sr.po $(srcdir)/sr@latin.po $(srcdir)/sv.po $(srcdir)/ta.po $(srcdir)/te.po $(srcdir)/tg.po $(srcdir)/th.po $(srcdir)/tr.po $(srcdir)/tw.po $(srcdir)/uk.po $(srcdir)/ur.po $(srcdir)/vi.po $(srcdir)/wba.po $(srcdir)/yo.po $(srcdir)/zh_CN.po $(srcdir)/zh_HK.po $(srcdir)/zh_TW.po $(srcdir)/zu.po
GMOFILES =  $(srcdir)/af.gmo $(srcdir)/am.gmo $(srcdir)/anp.gmo $(srcdir)/ar.gmo $(srcdir)/as.gmo $(srcdir)/ast.gmo $(srcdir)/bal.gmo $(srcdir)/be.gmo $(srcdir)/bg.gmo $(srcdir)/bn.gmo $(srcdir)/bn_IN.gmo $(srcdir)/bo.gmo $(srcdir)/br.gmo $(srcdir)/brx.gmo $(srcdir)/bs.gmo $(srcdir)/ca.gmo $(srcdir)/cs.gmo $(srcdir)/cy.gmo $(srcdir)/da.gmo $(srcdir)/de.gmo $(srcdir)/de_CH.gmo $(srcdir)/el.gmo $(srcdir)/en_GB.gmo $(srcdir)/eo.gmo $(srcdir)/es.gmo $(srcdir)/et.gmo $(srcdir)/eu.gmo $(srcdir)/fa.gmo $(srcdir)/fi.gmo $(srcdir)/fr.gmo $(srcdir)/gl.gmo $(srcdir)/gu.gmo $(srcdir)/he.gmo $(srcdir)/hi.gmo $(srcdir)/hr.gmo $(srcdir)/hu.gmo $(srcdir)/ia.gmo $(srcdir)/id.gmo $(srcdir)/ilo.gmo $(srcdir)/is.gmo $(srcdir)/it.gmo $(srcdir)/ja.gmo $(srcdir)/ka.gmo $(srcdir)/kk.gmo $(srcdir)/km.gmo $(srcdir)/kn.gmo $(srcdir)/ko.gmo $(srcdir)/kw.gmo $(srcdir)/kw@kkcor.gmo $(srcdir)/kw@uccor.gmo $(srcdir)/kw_GB.gmo $(srcdir)/ky.gmo $(srcdir)/lt.gmo $(srcdir)/lv.gmo $(srcdir)/mai.gmo $(srcdir)/mk.gmo $(srcdir)/ml.gmo $(srcdir)/mn.gmo $(srcdir)/mr.gmo $(srcdir)/ms.gmo $(srcdir)/nb.gmo $(srcdir)/nds.gmo $(srcdir)/ne.gmo $(srcdir)/nl.gmo $(srcdir)/nn.gmo $(srcdir)/nso.gmo $(srcdir)/or.gmo $(srcdir)/pa.gmo $(srcdir)/pl.gmo $(srcdir)/pt.gmo $(srcdir)/pt_BR.gmo $(srcdir)/ro.gmo $(srcdir)/ru.gmo $(srcdir)/si.gmo $(srcdir)/sk.gmo $(srcdir)/sl.gmo $(srcdir)/sq.gmo $(srcdir)/sr.gmo $(srcdir)/sr@latin.gmo $(srcdir)/sv.gmo $(srcdir)/ta.gmo $(srcdir)/te.gmo $(srcdir)/tg.gmo $(srcdir)/th.gmo $(srcdir)/tr.gmo $(srcdir)/tw.gmo $(srcdir)/uk.gmo $(srcdir)/ur.gmo $(srcdir)/vi.gmo $(srcdir)/wba.gmo $(srcdir)/yo.gmo $(srcdir)/zh_CN.gmo $(srcdir)/zh_HK.gmo $(srcdir)/zh_TW.gmo $(srcdir)/zu.gmo
UPDATEPOFILES =  af.po-update am.po-update anp.po-update ar.po-update as.po-update ast.po-update bal.po-update be.po-update bg.po-update bn.po-update bn_IN.po-update bo.po-update br.po-update brx.po-update bs.po-update ca.po-update cs.po-update cy.po-update da.po-update de.po-update de_CH.po-update el.po-update en_GB.po-update eo.po-update es.po-update et.po-update eu.po-update fa.po-update fi.po-update fr.po-update gl.po-update gu.po-update he.po-update hi.po-update hr.po-update hu.po-update ia.po-update id.po-update ilo.po-update is.po-update it.po-update ja.po-update ka.po-update kk.po-update km.po-update kn.po-update ko.po-update kw.po-update kw@kkcor.po-update kw@uccor.po-update kw_GB.po-update ky.po-update lt.po-update lv.po-update mai.po-update mk.po-update ml.po-update mn.po-update mr.po-update ms.po-update nb.po-update nds.po-update ne.po-update nl.po-update nn.po-update nso.po-update or.po-update pa.po-update pl.po-update pt.po-update pt_BR.po-update ro.po-update ru.po-update si.po-update sk.po-update sl.po-update sq.po-update sr.po-update sr@latin.po-update sv.po-update ta.po-update te.po-update tg.po-update th.po-update tr.po-update tw.po-update uk.po-update ur.po-update vi.po-update wba.po-update yo.po-update zh_CN.po-update zh_HK.po-update zh_TW.po-update zu.po-update
DUMMYPOFILES =  af.nop am.nop anp.nop ar.nop as.nop ast.nop bal.nop be.nop bg.nop bn.nop bn_IN.nop bo.nop br.nop brx.nop bs.nop ca.nop cs.nop cy.nop da.nop de.nop de_CH.nop el.nop en_GB.nop eo.nop es.nop et.nop eu.nop fa.nop fi.nop fr.nop gl.nop gu.nop he.nop hi.nop hr.nop hu.nop ia.nop id.nop ilo.nop is.nop it.nop ja.nop ka.nop kk.nop km.nop kn.nop ko.nop kw.nop kw@kkcor.nop kw@uccor.nop kw_GB.nop ky.nop lt.nop lv.nop mai.nop mk.nop ml.nop mn.nop mr.nop ms.nop nb.nop nds.nop ne.nop nl.nop nn.nop nso.nop or.nop pa.nop pl.nop pt.nop pt_BR.nop ro.nop ru.nop si.nop sk.nop sl.nop sq.nop sr.nop sr@latin.nop sv.nop ta.nop te.nop tg.nop th.nop tr.nop tw.nop uk.nop ur.nop vi.nop wba.nop yo.nop zh_CN.nop zh_HK.nop zh_TW.nop zu.nop
DISTFILES.common = Makefile.in.in remove-potcdate.sin \
$(DISTFILES.common.extra1) $(DISTFILES.common.extra2) $(DISTFILES.common.extra3)
DISTFILES = $(DISTFILES.common) Makevars POTFILES.in \
$(POFILES) $(GMOFILES) \
$(DISTFILES.extra1) $(DISTFILES.extra2) $(DISTFILES.extra3)

POTFILES = \
     ../../daemon/admin.c \
     ../../daemon/admin_dispatch.h \
     ../../daemon/admin_server.c \
     ../../daemon/libvirtd-config.c \
     ../../daemon/libvirtd.c \
     ../../daemon/qemu_dispatch.h \
     ../../daemon/remote.c \
     ../../daemon/remote_dispatch.h \
     ../../daemon/stream.c \
     ../../gnulib/lib/gai_strerror.c \
     ../../gnulib/lib/getopt.c \
     ../../gnulib/lib/regcomp.c \
     ../../src/access/viraccessdriverpolkit.c \
     ../../src/access/viraccessmanager.c \
     ../../src/bhyve/bhyve_capabilities.c \
     ../../src/bhyve/bhyve_command.c \
     ../../src/bhyve/bhyve_device.c \
     ../../src/bhyve/bhyve_domain.c \
     ../../src/bhyve/bhyve_driver.c \
     ../../src/bhyve/bhyve_monitor.c \
     ../../src/bhyve/bhyve_parse_command.c \
     ../../src/bhyve/bhyve_process.c \
     ../../src/conf/capabilities.c \
     ../../src/conf/cpu_conf.c \
     ../../src/conf/device_conf.c \
     ../../src/conf/domain_addr.c \
     ../../src/conf/domain_capabilities.c \
     ../../src/conf/domain_conf.c \
     ../../src/conf/domain_event.c \
     ../../src/conf/interface_conf.c \
     ../../src/conf/netdev_bandwidth_conf.c \
     ../../src/conf/netdev_vlan_conf.c \
     ../../src/conf/netdev_vport_profile_conf.c \
     ../../src/conf/network_conf.c \
     ../../src/conf/networkcommon_conf.c \
     ../../src/conf/node_device_conf.c \
     ../../src/conf/numa_conf.c \
     ../../src/conf/nwfilter_conf.c \
     ../../src/conf/nwfilter_params.c \
     ../../src/conf/object_event.c \
     ../../src/conf/secret_conf.c \
     ../../src/conf/snapshot_conf.c \
     ../../src/conf/storage_adapter_conf.c \
     ../../src/conf/storage_conf.c \
     ../../src/conf/virchrdev.c \
     ../../src/conf/virdomainobjlist.c \
     ../../src/conf/virnetworkobj.c \
     ../../src/conf/virnodedeviceobj.c \
     ../../src/conf/virnwfilterobj.c \
     ../../src/conf/virsavecookie.c \
     ../../src/conf/virsecretobj.c \
     ../../src/conf/virstorageobj.c \
     ../../src/cpu/cpu.c \
     ../../src/cpu/cpu_arm.c \
     ../../src/cpu/cpu_map.c \
     ../../src/cpu/cpu_ppc64.c \
     ../../src/cpu/cpu_s390.c \
     ../../src/cpu/cpu_x86.c \
     ../../src/datatypes.c \
     ../../src/driver.c \
     ../../src/esx/esx_driver.c \
     ../../src/esx/esx_network_driver.c \
     ../../src/esx/esx_storage_backend_iscsi.c \
     ../../src/esx/esx_storage_backend_vmfs.c \
     ../../src/esx/esx_storage_driver.c \
     ../../src/esx/esx_stream.c \
     ../../src/esx/esx_util.c \
     ../../src/esx/esx_vi.c \
     ../../src/esx/esx_vi_methods.c \
     ../../src/esx/esx_vi_types.c \
     ../../src/hyperv/hyperv_driver.c \
     ../../src/hyperv/hyperv_util.c \
     ../../src/hyperv/hyperv_wmi.c \
     ../../src/interface/interface_backend_netcf.c \
     ../../src/interface/interface_backend_udev.c \
     ../../src/internal.h \
     ../../src/libvirt-admin.c \
     ../../src/libvirt-domain-snapshot.c \
     ../../src/libvirt-domain.c \
     ../../src/libvirt-host.c \
     ../../src/libvirt-lxc.c \
     ../../src/libvirt-network.c \
     ../../src/libvirt-nodedev.c \
     ../../src/libvirt-nwfilter.c \
     ../../src/libvirt-qemu.c \
     ../../src/libvirt-secret.c \
     ../../src/libvirt-storage.c \
     ../../src/libvirt-stream.c \
     ../../src/libvirt.c \
     ../../src/libxl/libxl_capabilities.c \
     ../../src/libxl/libxl_conf.c \
     ../../src/libxl/libxl_domain.c \
     ../../src/libxl/libxl_driver.c \
     ../../src/libxl/libxl_migration.c \
     ../../src/locking/lock_daemon.c \
     ../../src/locking/lock_daemon_dispatch.c \
     ../../src/locking/lock_driver_lockd.c \
     ../../src/locking/lock_driver_sanlock.c \
     ../../src/locking/lock_manager.c \
     ../../src/locking/sanlock_helper.c \
     ../../src/logging/log_daemon.c \
     ../../src/logging/log_daemon_dispatch.c \
     ../../src/logging/log_handler.c \
     ../../src/logging/log_manager.c \
     ../../src/lxc/lxc_cgroup.c \
     ../../src/lxc/lxc_conf.c \
     ../../src/lxc/lxc_container.c \
     ../../src/lxc/lxc_controller.c \
     ../../src/lxc/lxc_domain.c \
     ../../src/lxc/lxc_driver.c \
     ../../src/lxc/lxc_fuse.c \
     ../../src/lxc/lxc_hostdev.c \
     ../../src/lxc/lxc_native.c \
     ../../src/lxc/lxc_process.c \
     ../../src/network/bridge_driver.c \
     ../../src/network/bridge_driver_linux.c \
     ../../src/network/leaseshelper.c \
     ../../src/node_device/node_device_driver.c \
     ../../src/node_device/node_device_hal.c \
     ../../src/node_device/node_device_udev.c \
     ../../src/nwfilter/nwfilter_dhcpsnoop.c \
     ../../src/nwfilter/nwfilter_driver.c \
     ../../src/nwfilter/nwfilter_ebiptables_driver.c \
     ../../src/nwfilter/nwfilter_gentech_driver.c \
     ../../src/nwfilter/nwfilter_learnipaddr.c \
     ../../src/openvz/openvz_conf.c \
     ../../src/openvz/openvz_driver.c \
     ../../src/openvz/openvz_util.c \
     ../../src/phyp/phyp_driver.c \
     ../../src/qemu/qemu_agent.c \
     ../../src/qemu/qemu_alias.c \
     ../../src/qemu/qemu_block.c \
     ../../src/qemu/qemu_capabilities.c \
     ../../src/qemu/qemu_cgroup.c \
     ../../src/qemu/qemu_command.c \
     ../../src/qemu/qemu_conf.c \
     ../../src/qemu/qemu_domain.c \
     ../../src/qemu/qemu_domain_address.c \
     ../../src/qemu/qemu_driver.c \
     ../../src/qemu/qemu_hostdev.c \
     ../../src/qemu/qemu_hotplug.c \
     ../../src/qemu/qemu_interface.c \
     ../../src/qemu/qemu_migration.c \
     ../../src/qemu/qemu_migration_cookie.c \
     ../../src/qemu/qemu_monitor.c \
     ../../src/qemu/qemu_monitor_json.c \
     ../../src/qemu/qemu_monitor_text.c \
     ../../src/qemu/qemu_parse_command.c \
     ../../src/qemu/qemu_process.c \
     ../../src/remote/remote_client_bodies.h \
     ../../src/remote/remote_driver.c \
     ../../src/rpc/virkeepalive.c \
     ../../src/rpc/virnetclient.c \
     ../../src/rpc/virnetclientprogram.c \
     ../../src/rpc/virnetclientstream.c \
     ../../src/rpc/virnetdaemon.c \
     ../../src/rpc/virnetlibsshsession.c \
     ../../src/rpc/virnetmessage.c \
     ../../src/rpc/virnetsaslcontext.c \
     ../../src/rpc/virnetserver.c \
     ../../src/rpc/virnetserverclient.c \
     ../../src/rpc/virnetservermdns.c \
     ../../src/rpc/virnetserverprogram.c \
     ../../src/rpc/virnetserverservice.c \
     ../../src/rpc/virnetsocket.c \
     ../../src/rpc/virnetsshsession.c \
     ../../src/rpc/virnettlscontext.c \
     ../../src/secret/secret_driver.c \
     ../../src/security/security_apparmor.c \
     ../../src/security/security_dac.c \
     ../../src/security/security_driver.c \
     ../../src/security/security_manager.c \
     ../../src/security/security_selinux.c \
     ../../src/security/virt-aa-helper.c \
     ../../src/storage/parthelper.c \
     ../../src/storage/storage_backend.c \
     ../../src/storage/storage_backend_disk.c \
     ../../src/storage/storage_backend_fs.c \
     ../../src/storage/storage_backend_gluster.c \
     ../../src/storage/storage_backend_iscsi.c \
     ../../src/storage/storage_backend_logical.c \
     ../../src/storage/storage_backend_mpath.c \
     ../../src/storage/storage_backend_rbd.c \
     ../../src/storage/storage_backend_scsi.c \
     ../../src/storage/storage_backend_sheepdog.c \
     ../../src/storage/storage_backend_vstorage.c \
     ../../src/storage/storage_backend_zfs.c \
     ../../src/storage/storage_driver.c \
     ../../src/storage/storage_source.c \
     ../../src/storage/storage_util.c \
     ../../src/test/test_driver.c \
     ../../src/uml/uml_conf.c \
     ../../src/uml/uml_driver.c \
     ../../src/util/iohelper.c \
     ../../src/util/viralloc.c \
     ../../src/util/viraudit.c \
     ../../src/util/virauth.c \
     ../../src/util/virauthconfig.c \
     ../../src/util/virbitmap.c \
     ../../src/util/virbuffer.c \
     ../../src/util/vircgroup.c \
     ../../src/util/virclosecallbacks.c \
     ../../src/util/vircommand.c \
     ../../src/util/virconf.c \
     ../../src/util/vircrypto.c \
     ../../src/util/virdbus.c \
     ../../src/util/virdnsmasq.c \
     ../../src/util/virerror.c \
     ../../src/util/virerror.h \
     ../../src/util/vireventpoll.c \
     ../../src/util/virfcp.c \
     ../../src/util/virfdstream.c \
     ../../src/util/virfile.c \
     ../../src/util/virfilecache.c \
     ../../src/util/virfirewall.c \
     ../../src/util/virfirmware.c \
     ../../src/util/virhash.c \
     ../../src/util/virhook.c \
     ../../src/util/virhostcpu.c \
     ../../src/util/virhostdev.c \
     ../../src/util/virhostmem.c \
     ../../src/util/viridentity.c \
     ../../src/util/virinitctl.c \
     ../../src/util/viriptables.c \
     ../../src/util/viriscsi.c \
     ../../src/util/virjson.c \
     ../../src/util/virkeyfile.c \
     ../../src/util/virlease.c \
     ../../src/util/virlockspace.c \
     ../../src/util/virlog.c \
     ../../src/util/virmacmap.c \
     ../../src/util/virmdev.c \
     ../../src/util/virnetdev.c \
     ../../src/util/virnetdevbandwidth.c \
     ../../src/util/virnetdevbridge.c \
     ../../src/util/virnetdevip.c \
     ../../src/util/virnetdevmacvlan.c \
     ../../src/util/virnetdevmidonet.c \
     ../../src/util/virnetdevopenvswitch.c \
     ../../src/util/virnetdevtap.c \
     ../../src/util/virnetdevveth.c \
     ../../src/util/virnetdevvportprofile.c \
     ../../src/util/virnetlink.c \
     ../../src/util/virnodesuspend.c \
     ../../src/util/virnuma.c \
     ../../src/util/virobject.c \
     ../../src/util/virpci.c \
     ../../src/util/virperf.c \
     ../../src/util/virpidfile.c \
     ../../src/util/virpolkit.c \
     ../../src/util/virportallocator.c \
     ../../src/util/virprocess.c \
     ../../src/util/virqemu.c \
     ../../src/util/virrandom.c \
     ../../src/util/virrotatingfile.c \
     ../../src/util/virscsi.c \
     ../../src/util/virscsihost.c \
     ../../src/util/virscsivhost.c \
     ../../src/util/virsecret.c \
     ../../src/util/virsexpr.c \
     ../../src/util/virsocketaddr.c \
     ../../src/util/virstorageencryption.c \
     ../../src/util/virstoragefile.c \
     ../../src/util/virstring.c \
     ../../src/util/virsysinfo.c \
     ../../src/util/virthreadjob.c \
     ../../src/util/virthreadpool.c \
     ../../src/util/virtime.c \
     ../../src/util/virtpm.c \
     ../../src/util/virtypedparam.c \
     ../../src/util/viruri.c \
     ../../src/util/virusb.c \
     ../../src/util/virutil.c \
     ../../src/util/virvhba.c \
     ../../src/util/virxml.c \
     ../../src/vbox/vbox_MSCOMGlue.c \
     ../../src/vbox/vbox_XPCOMCGlue.c \
     ../../src/vbox/vbox_common.c \
     ../../src/vbox/vbox_driver.c \
     ../../src/vbox/vbox_network.c \
     ../../src/vbox/vbox_snapshot_conf.c \
     ../../src/vbox/vbox_storage.c \
     ../../src/vbox/vbox_tmpl.c \
     ../../src/vmware/vmware_conf.c \
     ../../src/vmware/vmware_driver.c \
     ../../src/vmx/vmx.c \
     ../../src/vz/vz_driver.c \
     ../../src/vz/vz_sdk.c \
     ../../src/vz/vz_utils.c \
     ../../src/vz/vz_utils.h \
     ../../src/xen/block_stats.c \
     ../../src/xen/xen_driver.c \
     ../../src/xen/xen_hypervisor.c \
     ../../src/xen/xen_inotify.c \
     ../../src/xen/xend_internal.c \
     ../../src/xen/xm_internal.c \
     ../../src/xen/xs_internal.c \
     ../../src/xenapi/xenapi_driver.c \
     ../../src/xenapi/xenapi_utils.c \
     ../../src/xenconfig/xen_common.c \
     ../../src/xenconfig/xen_sxpr.c \
     ../../src/xenconfig/xen_xl.c \
     ../../src/xenconfig/xen_xm.c \
     ../../tests/virpolkittest.c \
     ../../tools/libvirt-guests.sh.in \
     ../../tools/virsh-console.c \
     ../../tools/virsh-domain-monitor.c \
     ../../tools/virsh-domain.c \
     ../../tools/virsh-edit.c \
     ../../tools/virsh-host.c \
     ../../tools/virsh-interface.c \
     ../../tools/virsh-network.c \
     ../../tools/virsh-nodedev.c \
     ../../tools/virsh-nwfilter.c \
     ../../tools/virsh-pool.c \
     ../../tools/virsh-secret.c \
     ../../tools/virsh-snapshot.c \
     ../../tools/virsh-util.c \
     ../../tools/virsh-volume.c \
     ../../tools/virsh.c \
     ../../tools/virt-admin.c \
     ../../tools/virt-host-validate-bhyve.c \
     ../../tools/virt-host-validate-common.c \
     ../../tools/virt-host-validate-lxc.c \
     ../../tools/virt-host-validate-qemu.c \
     ../../tools/virt-host-validate.c \
     ../../tools/virt-login-shell.c \
     ../../tools/vsh.c \
     ../../tools/vsh.h

CATALOGS =  af.gmo am.gmo anp.gmo ar.gmo as.gmo ast.gmo bal.gmo be.gmo bg.gmo bn.gmo bn_IN.gmo bo.gmo br.gmo brx.gmo bs.gmo ca.gmo cs.gmo cy.gmo da.gmo de.gmo de_CH.gmo el.gmo en_GB.gmo eo.gmo es.gmo et.gmo eu.gmo fa.gmo fi.gmo fr.gmo gl.gmo gu.gmo he.gmo hi.gmo hr.gmo hu.gmo ia.gmo id.gmo ilo.gmo is.gmo it.gmo ja.gmo ka.gmo kk.gmo km.gmo kn.gmo ko.gmo kw.gmo kw@kkcor.gmo kw@uccor.gmo kw_GB.gmo ky.gmo lt.gmo lv.gmo mai.gmo mk.gmo ml.gmo mn.gmo mr.gmo ms.gmo nb.gmo nds.gmo ne.gmo nl.gmo nn.gmo nso.gmo or.gmo pa.gmo pl.gmo pt.gmo pt_BR.gmo ro.gmo ru.gmo si.gmo sk.gmo sl.gmo sq.gmo sr.gmo sr@latin.gmo sv.gmo ta.gmo te.gmo tg.gmo th.gmo tr.gmo tw.gmo uk.gmo ur.gmo vi.gmo wba.gmo yo.gmo zh_CN.gmo zh_HK.gmo zh_TW.gmo zu.gmo

# Makevars gets inserted here. (Don't remove this line!)
# Makefile variables for PO directory in any package using GNU gettext.

# Usually the message domain is the same as the package name.
DOMAIN = $(PACKAGE)

# These two variables depend on the location of this directory.
subdir = po
top_builddir = ..

# These options get passed to xgettext.
XGETTEXT_OPTIONS = --keyword=_ --keyword=N_ \
          \
 --flag=_:1:pass-c-format\
 --flag=N_:1:pass-c-format\
 --flag=error:3:c-format --flag=error_at_line:5:c-format\
\
 --flag=virAsprintf:2:c-format\
 --from-code=UTF-8\
 $${end_of_xgettext_options+}

# This is the copyright holder that gets inserted into the header of the
# $(DOMAIN).pot file.  Set this to the copyright holder of the surrounding
# package.  (Note that the msgstr strings, extracted from the package's
# sources, belong to the copyright holder of the package.)  Translators are
# expected to transfer the copyright for their translations to this person
# or entity, or to disclaim their copyright.  The empty string stands for
# the public domain; in this case the translators are expected to disclaim
# their copyright.
COPYRIGHT_HOLDER = Red Hat, Inc.

# This is the email address or URL to which the translators shall report
# bugs in the untranslated strings:
# - Strings which are not entire sentences, see the maintainer guidelines
#   in the GNU gettext documentation, section 'Preparing Strings'.
# - Strings which use unclear terms or require additional context to be
#   understood.
# - Strings which make invalid assumptions about notation of date, time or
#   money.
# - Pluralisation problems.
# - Incorrect English spelling.
# - Incorrect formatting.
# It can be your email address, or a mailing list address where translators
# can write to without being subscribed, or the URL of a web page through
# which the translators can contact you.
MSGID_BUGS_ADDRESS = libvir-list@redhat.com

# This is the list of locale categories, beyond LC_MESSAGES, for which the
# message catalogs shall be used.  It is usually empty.
EXTRA_LOCALE_CATEGORIES = 

.SUFFIXES:
.SUFFIXES: .po .gmo .mo .sed .sin .nop .po-create .po-update

.po.mo:
	@echo "$(MSGFMT) -c -o $@ $<"; \
	$(MSGFMT) -c -o t-$@ $< && mv t-$@ $@

.po.gmo:
	@lang=`echo $* | sed -e 's,.*/,,'`; \
	test "$(srcdir)" = . && cdcmd="" || cdcmd="cd $(srcdir) && "; \
	echo "$${cdcmd}rm -f $${lang}.gmo && $(GMSGFMT) -c --statistics -o $${lang}.gmo $${lang}.po"; \
	cd $(srcdir) && rm -f $${lang}.gmo && $(GMSGFMT) -c --statistics -o t-$${lang}.gmo $${lang}.po && mv t-$${lang}.gmo $${lang}.gmo

.sin.sed:
	sed -e '/^#/d' $< > t-$@
	mv t-$@ $@


all: check-macro-version all-yes

all-yes: stamp-po
all-no:

# Ensure that the gettext macros and this Makefile.in.in are in sync.
check-macro-version:
	@test "$(GETTEXT_MACRO_VERSION)" = "0.17" \
	  || { echo "*** error: gettext infrastructure mismatch: using a Makefile.in.in from gettext version $(GETTEXT_MACRO_VERSION) but the autoconf macros are from gettext version 0.17" 1>&2; \
	       exit 1; \
	     }

# $(srcdir)/$(DOMAIN).pot is only created when needed. When xgettext finds no
# internationalized messages, no $(srcdir)/$(DOMAIN).pot is created (because
# we don't want to bother translators with empty POT files). We assume that
# LINGUAS is empty in this case, i.e. $(POFILES) and $(GMOFILES) are empty.
# In this case, stamp-po is a nop (i.e. a phony target).

# stamp-po is a timestamp denoting the last time at which the CATALOGS have
# been loosely updated. Its purpose is that when a developer or translator
# checks out the package via CVS, and the $(DOMAIN).pot file is not in CVS,
# "make" will update the $(DOMAIN).pot and the $(CATALOGS), but subsequent
# invocations of "make" will do nothing. This timestamp would not be necessary
# if updating the $(CATALOGS) would always touch them; however, the rule for
# $(POFILES) has been designed to not touch files that don't need to be
# changed.
stamp-po: $(srcdir)/$(DOMAIN).pot
	test ! -f $(srcdir)/$(DOMAIN).pot || \
	  test -z "$(GMOFILES)" || $(MAKE) $(GMOFILES)
	@test ! -f $(srcdir)/$(DOMAIN).pot || { \
	  echo "touch stamp-po" && \
	  echo timestamp > stamp-poT && \
	  mv stamp-poT stamp-po; \
	}

# Note: Target 'all' must not depend on target '$(DOMAIN).pot-update',
# otherwise packages like GCC can not be built if only parts of the source
# have been downloaded.

# This target rebuilds $(DOMAIN).pot; it is an expensive operation.
# Note that $(DOMAIN).pot is not touched if it doesn't need to be changed.
$(DOMAIN).pot-update: $(POTFILES) $(srcdir)/POTFILES.in remove-potcdate.sed
	if LC_ALL=C grep 'GNU libvirt' $(top_srcdir)/* 2>/dev/null | grep -v 'libtool:' >/dev/null; then \
	  package_gnu='GNU '; \
	else \
	  package_gnu=''; \
	fi; \
	if test -n '$(MSGID_BUGS_ADDRESS)' || test '$(PACKAGE_BUGREPORT)' = '@'PACKAGE_BUGREPORT'@'; then \
	  msgid_bugs_address='$(MSGID_BUGS_ADDRESS)'; \
	else \
	  msgid_bugs_address='$(PACKAGE_BUGREPORT)'; \
	fi; \
	case `$(XGETTEXT) --version | sed 1q | sed -e 's,^[^0-9]*,,'` in \
	  '' | 0.[0-9] | 0.[0-9].* | 0.1[0-5] | 0.1[0-5].* | 0.16 | 0.16.[0-1]*) \
	    $(XGETTEXT) --default-domain=$(DOMAIN) --directory=$(top_srcdir) \
	      --add-comments=TRANSLATORS: $(XGETTEXT_OPTIONS)  --flag=asprintf:2:c-format --flag=vasprintf:2:c-format --flag=error:3:c-format --flag=error_at_line:5:c-format \
	      --files-from=$(srcdir)/POTFILES.in \
	      --copyright-holder='$(COPYRIGHT_HOLDER)' \
	      --msgid-bugs-address="$$msgid_bugs_address" \
	    ;; \
	  *) \
	    $(XGETTEXT) --default-domain=$(DOMAIN) --directory=$(top_srcdir) \
	      --add-comments=TRANSLATORS: $(XGETTEXT_OPTIONS)  --flag=asprintf:2:c-format --flag=vasprintf:2:c-format --flag=error:3:c-format --flag=error_at_line:5:c-format \
	      --files-from=$(srcdir)/POTFILES.in \
	      --copyright-holder='$(COPYRIGHT_HOLDER)' \
	      --package-name="$${package_gnu}libvirt" \
	      --package-version='4.0.0' \
	      --msgid-bugs-address="$$msgid_bugs_address" \
	    ;; \
	esac
	test ! -f $(DOMAIN).po || { \
	  if test -f $(srcdir)/$(DOMAIN).pot; then \
	    sed -f remove-potcdate.sed < $(srcdir)/$(DOMAIN).pot > $(DOMAIN).1po && \
	    sed -f remove-potcdate.sed < $(DOMAIN).po > $(DOMAIN).2po && \
	    if cmp $(DOMAIN).1po $(DOMAIN).2po >/dev/null 2>&1; then \
	      rm -f $(DOMAIN).1po $(DOMAIN).2po $(DOMAIN).po; \
	    else \
	      rm -f $(DOMAIN).1po $(DOMAIN).2po $(srcdir)/$(DOMAIN).pot && \
	      mv $(DOMAIN).po $(srcdir)/$(DOMAIN).pot; \
	    fi; \
	  else \
	    mv $(DOMAIN).po $(srcdir)/$(DOMAIN).pot; \
	  fi; \
	}

# This rule has no dependencies: we don't need to update $(DOMAIN).pot at
# every "make" invocation, only create it when it is missing.
# Only "make $(DOMAIN).pot-update" or "make dist" will force an update.
$(srcdir)/$(DOMAIN).pot:
	$(MAKE) $(DOMAIN).pot-update

# This target rebuilds a PO file if $(DOMAIN).pot has changed.
# Note that a PO file is not touched if it doesn't need to be changed.
$(POFILES): $(srcdir)/$(DOMAIN).pot
	@lang=`echo $@ | sed -e 's,.*/,,' -e 's/\.po$$//'`; \
	if test -f "$(srcdir)/$${lang}.po"; then \
	  test "$(srcdir)" = . && cdcmd="" || cdcmd="cd $(srcdir) && "; \
	  echo "$${cdcmd}$(MSGMERGE_UPDATE) $${lang}.po $(DOMAIN).pot"; \
	  cd $(srcdir) && $(MSGMERGE_UPDATE) $${lang}.po $(DOMAIN).pot; \
	else \
	  $(MAKE) $${lang}.po-create; \
	fi


install: install-exec install-data
install-exec:
install-data: install-data-yes
	if test "$(PACKAGE)" = "gettext-tools"; then \
	  $(mkdir_p) $(DESTDIR)$(gettextsrcdir); \
	  for file in $(DISTFILES.common) Makevars.template; do \
	    $(INSTALL_DATA) $(srcdir)/$$file \
			    $(DESTDIR)$(gettextsrcdir)/$$file; \
	  done; \
	  for file in Makevars; do \
	    rm -f $(DESTDIR)$(gettextsrcdir)/$$file; \
	  done; \
	else \
	  : ; \
	fi
install-data-no: all
install-data-yes: all
	$(mkdir_p) $(DESTDIR)$(datadir)
	@catalogs='$(CATALOGS)'; \
	for cat in $$catalogs; do \
	  cat=`basename $$cat`; \
	  lang=`echo $$cat | sed -e 's/\.gmo$$//'`; \
	  dir=$(localedir)/$$lang/LC_MESSAGES; \
	  $(mkdir_p) $(DESTDIR)$$dir; \
	  if test -r $$cat; then realcat=$$cat; else realcat=$(srcdir)/$$cat; fi; \
	  $(INSTALL_DATA) $$realcat $(DESTDIR)$$dir/$(DOMAIN).mo; \
	  echo "installing $$realcat as $(DESTDIR)$$dir/$(DOMAIN).mo"; \
	  for lc in '' $(EXTRA_LOCALE_CATEGORIES); do \
	    if test -n "$$lc"; then \
	      if (cd $(DESTDIR)$(localedir)/$$lang && LC_ALL=C ls -l -d $$lc 2>/dev/null) | grep ' -> ' >/dev/null; then \
	        link=`cd $(DESTDIR)$(localedir)/$$lang && LC_ALL=C ls -l -d $$lc | sed -e 's/^.* -> //'`; \
	        mv $(DESTDIR)$(localedir)/$$lang/$$lc $(DESTDIR)$(localedir)/$$lang/$$lc.old; \
	        mkdir $(DESTDIR)$(localedir)/$$lang/$$lc; \
	        (cd $(DESTDIR)$(localedir)/$$lang/$$lc.old && \
	         for file in *; do \
	           if test -f $$file; then \
	             ln -s ../$$link/$$file $(DESTDIR)$(localedir)/$$lang/$$lc/$$file; \
	           fi; \
	         done); \
	        rm -f $(DESTDIR)$(localedir)/$$lang/$$lc.old; \
	      else \
	        if test -d $(DESTDIR)$(localedir)/$$lang/$$lc; then \
	          :; \
	        else \
	          rm -f $(DESTDIR)$(localedir)/$$lang/$$lc; \
	          mkdir $(DESTDIR)$(localedir)/$$lang/$$lc; \
	        fi; \
	      fi; \
	      rm -f $(DESTDIR)$(localedir)/$$lang/$$lc/$(DOMAIN).mo; \
	      ln -s ../LC_MESSAGES/$(DOMAIN).mo $(DESTDIR)$(localedir)/$$lang/$$lc/$(DOMAIN).mo 2>/dev/null || \
	      ln $(DESTDIR)$(localedir)/$$lang/LC_MESSAGES/$(DOMAIN).mo $(DESTDIR)$(localedir)/$$lang/$$lc/$(DOMAIN).mo 2>/dev/null || \
	      cp -p $(DESTDIR)$(localedir)/$$lang/LC_MESSAGES/$(DOMAIN).mo $(DESTDIR)$(localedir)/$$lang/$$lc/$(DOMAIN).mo; \
	      echo "installing $$realcat link as $(DESTDIR)$(localedir)/$$lang/$$lc/$(DOMAIN).mo"; \
	    fi; \
	  done; \
	done

install-strip: install

installdirs: installdirs-exec installdirs-data
installdirs-exec:
installdirs-data: installdirs-data-yes
	if test "$(PACKAGE)" = "gettext-tools"; then \
	  $(mkdir_p) $(DESTDIR)$(gettextsrcdir); \
	else \
	  : ; \
	fi
installdirs-data-no:
installdirs-data-yes:
	$(mkdir_p) $(DESTDIR)$(datadir)
	@catalogs='$(CATALOGS)'; \
	for cat in $$catalogs; do \
	  cat=`basename $$cat`; \
	  lang=`echo $$cat | sed -e 's/\.gmo$$//'`; \
	  dir=$(localedir)/$$lang/LC_MESSAGES; \
	  $(mkdir_p) $(DESTDIR)$$dir; \
	  for lc in '' $(EXTRA_LOCALE_CATEGORIES); do \
	    if test -n "$$lc"; then \
	      if (cd $(DESTDIR)$(localedir)/$$lang && LC_ALL=C ls -l -d $$lc 2>/dev/null) | grep ' -> ' >/dev/null; then \
	        link=`cd $(DESTDIR)$(localedir)/$$lang && LC_ALL=C ls -l -d $$lc | sed -e 's/^.* -> //'`; \
	        mv $(DESTDIR)$(localedir)/$$lang/$$lc $(DESTDIR)$(localedir)/$$lang/$$lc.old; \
	        mkdir $(DESTDIR)$(localedir)/$$lang/$$lc; \
	        (cd $(DESTDIR)$(localedir)/$$lang/$$lc.old && \
	         for file in *; do \
	           if test -f $$file; then \
	             ln -s ../$$link/$$file $(DESTDIR)$(localedir)/$$lang/$$lc/$$file; \
	           fi; \
	         done); \
	        rm -f $(DESTDIR)$(localedir)/$$lang/$$lc.old; \
	      else \
	        if test -d $(DESTDIR)$(localedir)/$$lang/$$lc; then \
	          :; \
	        else \
	          rm -f $(DESTDIR)$(localedir)/$$lang/$$lc; \
	          mkdir $(DESTDIR)$(localedir)/$$lang/$$lc; \
	        fi; \
	      fi; \
	    fi; \
	  done; \
	done

# Define this as empty until I found a useful application.
installcheck:

uninstall: uninstall-exec uninstall-data
uninstall-exec:
uninstall-data: uninstall-data-yes
	if test "$(PACKAGE)" = "gettext-tools"; then \
	  for file in $(DISTFILES.common) Makevars.template; do \
	    rm -f $(DESTDIR)$(gettextsrcdir)/$$file; \
	  done; \
	else \
	  : ; \
	fi
uninstall-data-no:
uninstall-data-yes:
	catalogs='$(CATALOGS)'; \
	for cat in $$catalogs; do \
	  cat=`basename $$cat`; \
	  lang=`echo $$cat | sed -e 's/\.gmo$$//'`; \
	  for lc in LC_MESSAGES $(EXTRA_LOCALE_CATEGORIES); do \
	    rm -f $(DESTDIR)$(localedir)/$$lang/$$lc/$(DOMAIN).mo; \
	  done; \
	done

check: all

info dvi ps pdf html tags TAGS ctags CTAGS ID:

mostlyclean:
	rm -f remove-potcdate.sed
	rm -f stamp-poT
	rm -f core core.* $(DOMAIN).po $(DOMAIN).1po $(DOMAIN).2po *.new.po
	rm -fr *.o

clean: mostlyclean

distclean: clean
	rm -f Makefile Makefile.in POTFILES *.mo

maintainer-clean: distclean
	@echo "This command is intended for maintainers to use;"
	@echo "it deletes files that may require special tools to rebuild."
	rm -f stamp-po $(GMOFILES)

distdir = $(top_builddir)/$(PACKAGE)-$(VERSION)/$(subdir)
dist distdir:
	$(MAKE) update-po
	@$(MAKE) dist2
# This is a separate target because 'update-po' must be executed before.
dist2: stamp-po $(DISTFILES)
	dists="$(DISTFILES)"; \
	if test "$(PACKAGE)" = "gettext-tools"; then \
	  dists="$$dists Makevars.template"; \
	fi; \
	if test -f $(srcdir)/$(DOMAIN).pot; then \
	  dists="$$dists $(DOMAIN).pot stamp-po"; \
	fi; \
	if test -f $(srcdir)/ChangeLog; then \
	  dists="$$dists ChangeLog"; \
	fi; \
	for i in 0 1 2 3 4 5 6 7 8 9; do \
	  if test -f $(srcdir)/ChangeLog.$$i; then \
	    dists="$$dists ChangeLog.$$i"; \
	  fi; \
	done; \
	if test -f $(srcdir)/LINGUAS; then dists="$$dists LINGUAS"; fi; \
	for file in $$dists; do \
	  if test -f $$file; then \
	    cp -p $$file $(distdir) || exit 1; \
	  else \
	    cp -p $(srcdir)/$$file $(distdir) || exit 1; \
	  fi; \
	done

update-po: Makefile
	$(MAKE) $(DOMAIN).pot-update
	test -z "$(UPDATEPOFILES)" || $(MAKE) $(UPDATEPOFILES)
	$(MAKE) update-gmo

# General rule for creating PO files.

.nop.po-create:
	@lang=`echo $@ | sed -e 's/\.po-create$$//'`; \
	echo "File $$lang.po does not exist. If you are a translator, you can create it through 'msginit'." 1>&2; \
	exit 1

# General rule for updating PO files.

.nop.po-update:
	@lang=`echo $@ | sed -e 's/\.po-update$$//'`; \
	if test "$(PACKAGE)" = "gettext-tools"; then PATH=`pwd`/../src:$$PATH; fi; \
	tmpdir=`pwd`; \
	echo "$$lang:"; \
	test "$(srcdir)" = . && cdcmd="" || cdcmd="cd $(srcdir) && "; \
	echo "$${cdcmd}$(MSGMERGE) $$lang.po $(DOMAIN).pot -o $$lang.new.po"; \
	cd $(srcdir); \
	if $(MSGMERGE) $$lang.po $(DOMAIN).pot -o $$tmpdir/$$lang.new.po; then \
	  if cmp $$lang.po $$tmpdir/$$lang.new.po >/dev/null 2>&1; then \
	    rm -f $$tmpdir/$$lang.new.po; \
	  else \
	    if mv -f $$tmpdir/$$lang.new.po $$lang.po; then \
	      :; \
	    else \
	      echo "msgmerge for $$lang.po failed: cannot move $$tmpdir/$$lang.new.po to $$lang.po" 1>&2; \
	      exit 1; \
	    fi; \
	  fi; \
	else \
	  echo "msgmerge for $$lang.po failed!" 1>&2; \
	  rm -f $$tmpdir/$$lang.new.po; \
	fi

$(DUMMYPOFILES):

update-gmo: Makefile $(GMOFILES)
	@:

Makefile: Makefile.in.in Makevars $(top_builddir)/config.status POTFILES.in
	cd $(top_builddir) \
	  && $(SHELL) ./config.status $(subdir)/$@.in po-directories

force:

# Tell versions [3.59,3.63) of GNU make not to export all variables.
# Otherwise a system limit (for SysV at least) may be exceeded.
.NOEXPORT:
# Special Makefile rules for English message catalogs with quotation marks.

DISTFILES.common.extra1 = quot.sed boldquot.sed en@quot.header en@boldquot.header insert-header.sin Rules-quot

.SUFFIXES: .insert-header .po-update-en

en@quot.po-create:
	$(MAKE) en@quot.po-update
en@boldquot.po-create:
	$(MAKE) en@boldquot.po-update

en@quot.po-update: en@quot.po-update-en
en@boldquot.po-update: en@boldquot.po-update-en

.insert-header.po-update-en:
	@lang=`echo $@ | sed -e 's/\.po-update-en$$//'`; \
	if test "$(PACKAGE)" = "gettext"; then PATH=`pwd`/../src:$$PATH; GETTEXTLIBDIR=`cd $(top_srcdir)/src && pwd`; export GETTEXTLIBDIR; fi; \
	tmpdir=`pwd`; \
	echo "$$lang:"; \
	ll=`echo $$lang | sed -e 's/@.*//'`; \
	LC_ALL=C; export LC_ALL; \
	cd $(srcdir); \
	if $(MSGINIT) -i $(DOMAIN).pot --no-translator -l $$ll -o - 2>/dev/null | sed -f $$tmpdir/$$lang.insert-header | $(MSGCONV) -t UTF-8 | $(MSGFILTER) sed -f `echo $$lang | sed -e 's/.*@//'`.sed 2>/dev/null > $$tmpdir/$$lang.new.po; then \
	  if cmp $$lang.po $$tmpdir/$$lang.new.po >/dev/null 2>&1; then \
	    rm -f $$tmpdir/$$lang.new.po; \
	  else \
	    if mv -f $$tmpdir/$$lang.new.po $$lang.po; then \
	      :; \
	    else \
	      echo "creation of $$lang.po failed: cannot move $$tmpdir/$$lang.new.po to $$lang.po" 1>&2; \
	      exit 1; \
	    fi; \
	  fi; \
	else \
	  echo "creation of $$lang.po failed!" 1>&2; \
	  rm -f $$tmpdir/$$lang.new.po; \
	fi

en@quot.insert-header: insert-header.sin
	sed -e '/^#/d' -e 's/HEADER/en@quot.header/g' $(srcdir)/insert-header.sin > en@quot.insert-header

en@boldquot.insert-header: insert-header.sin
	sed -e '/^#/d' -e 's/HEADER/en@boldquot.header/g' $(srcdir)/insert-header.sin > en@boldquot.insert-header

mostlyclean: mostlyclean-quot
mostlyclean-quot:
	rm -f *.insert-header

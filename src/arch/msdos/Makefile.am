## Makefile.am for the MS-DOS version of `libarch.a'.

if USE_MIDAS_SOUND
libarch_a_LIBADD = vmidas.o
endif

INCLUDES = \
	@ARCH_INCLUDES@ \
	-I$(top_builddir)/src \
	-I$(top_srcdir)/src \
	-I$(top_srcdir)/src/drive \
	-I$(top_srcdir)/src/vdrive \
	-I$(top_srcdir)/src/raster \
	-I$(top_srcdir)/src/c64 \
	-I$(top_srcdir)/src/c64dtv \
	-I$(top_srcdir)/src/c128 \
	-I$(top_srcdir)/src/cbm2 \
	-I$(top_srcdir)/src/vic20 \
	-I$(top_srcdir)/src/pet \
	-I$(top_srcdir)/src/plus4 \
	-I$(top_srcdir)/src/sid \
	-I$(top_srcdir)/src/userport \
	-I$(top_srcdir)/src/lib/p64 \
	-I$(top_srcdir)/src/platform \
	-I$(top_srcdir)/src/imagecontents

libarch_a_DEPENDENCIES = @DOS_TFE_PCAP_LIB@

noinst_LIBRARIES = libarch.a

libpcap_nodma.a:
	(echo fixing dos_pcap; cp `$(CC) -print-file-name=libpcap.a` libpcap_nodma.a; ar -d libpcap_nodma.a dma.o)

libarch_a_SOURCES = \
	archdep.c \
	archdep.h \
	c128ui.c \
	c64ui.c \
	c64dtvui.c \
	catweaselmkiii.c \
	cbm2ui.c \
	cbm5x0ui.c \
	cbmcharsets.c \
	cbmcharsets.h \
	console.c \
	grabkey.c \
	grabkey.h \
	hardsid.c \
	joy.c \
	joy.h \
	kbd.c \
	kbd.h \
	lightpendrv.c \
	lightpendrv.h \
	menudefs.c \
	menudefs.h \
	mousedrv.c \
	mousedrv.h \
	msdosmain.c \
	parsid.c \
	petui.c \
	plus4ui.c \
	signals.c \
	socketimpl.h \
	statusbar.c \
	statusbar.h \
	rawnetarch.c \
	tui.c \
	tui.h \
	tui_backend.c \
	tui_backend.h \
	tuicharset.c \
	tuicharset.h \
	tuiimagebrowser.c \
	tuiimagebrowser.h \
	tuifs.c \
	tuifs.h \
	tuimenu.c \
	tuimenu.h \
	tuiview.c \
	tuiview.h \
	types.h \
	ui.c \
	ui.h \
	uiattach.h \
	uiattach.c \
	uiburstmod.c \
	uiburstmod.h \
	uic64_256k.c \
	uic64_256k.h \
	uic64cart.c \
	uic64cart.h \
	uic64dtv.c \
	uic64dtv.h \
	uic64dtvmodel.c \
	uic64dtvmodel.h \
	uic64model.c \
	uic64model.h \
	uic128model.c \
	uic128model.h \
	uicbm2model.c \
	uicbm2model.h \
	uicbm5x0model.c \
	uicbm5x0model.h \
	uiciamodel.c \
	uiciamodel.h \
	uicmdline.c \
	uidigimax.c \
	uidigimax.h \
	uidqbb.c \
	uidqbb.h \
	uidrive.c \
	uidrive.h \
	uids12c887rtc.c \
	uids12c887rtc.h \
	uieasyflash.c \
	uieasyflash.h \
	uiexpert.c \
	uiexpert.h \
	uigeoram.c \
	uigeoram.h \
	uiide64.c \
	uiide64.h \
	uiisepic.c \
	uiisepic.h \
	uijoystick.c \
	uijoystick.h \
	uilightpen.c \
	uilightpen.h \
	uimagicvoice.c \
	uimagicvoice.h \
	uimon.c \
	uimmc64.c \
	uimmc64.h \
	uimmcreplay.c \
	uimmcreplay.h \
	uinetplay.c \
	uinetplay.h \
	uiperipherial.c \
	uiperipherial.h \
	uipetmodel.c \
	uipetmodel.h \
	uipetdww.c \
	uipetdww.h \
	uipetreu.c \
	uipetreu.h \
	uiplus4cart.c \
	uiplus4cart.h \
	uiplus4model.c \
	uiplus4model.h \
 	uiplus256k.c \
 	uiplus256k.h \
	uiplus60k.c \
	uiplus60k.h \
	uiprinter.c \
	uiprinter.h \
	uiramcart.c \
	uiramcart.h \
	uiretroreplay.c \
	uiretroreplay.h \
	uireu.c \
	uireu.h \
	uiscreenshot.c \
	uiscreenshot.h \
	uisidc64.c \
	uisidc64.h \
	uisidc128.c \
	uisidc128.h \
	uisidcart.c \
	uisidcart.h \
	uisidcbm2.c \
	uisidcbm2.h \
	uisiddtv.c \
	uisiddtv.h \
	uisnapshot.c \
	uisnapshot.h \
	uisound.c \
	uisound.h \
	uisoundexpander.c \
	uisoundexpander.h \
	uisoundsampler.c \
	uisoundsampler.h \
	uitfe.c \
	uitfe.h \
	uiv364speech.c \
	uiv364speech.h \
	uivideo.c \
	uivideo.h \
	vic20ui.c \
	video.c \
	videoarch.h \
	vsidui.c \
	vsync.c

EXTRA_DIST = \
	vmidas.c \
	vmidas.h \
	make-bindist.sh

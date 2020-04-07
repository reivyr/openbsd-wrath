# $OpenBSD: Makefile.template,v 1.87 2020/03/22 17:18:01 cwen Exp $

COMMENT =	Fork of LordHavoc's DarkPlaces Quake engine

V =	1.2.1

DISTNAME =	wrath-${V}

GH_ACCOUNT =	KillPixelGames
GH_PROJECT =	wrath-darkplaces
GH_COMMIT =	ae8a4c06f2b2b088a537bb75c439817f4a009d6a

CATEGORIES =	games

MAINTAINER =	Paul Valencia <reivyr@tutanota.com>

# GPLv2
PERMIT_PACKAGE =	Yes

WANTLIB += SDL2 X11 c jpeg m z

LIB_DEPENDS =		devel/sdl2 \
			graphics/jpeg

USE_GMAKE =		Yes
MAKE_FILE =		makefile
ALL_TARGET =		sdl2-release

do-install:
	${INSTALL_PROGRAM} ${WRKBUILD}/darkplaces-sdl ${PREFIX}/bin/wrath

.include <bsd.port.mk>

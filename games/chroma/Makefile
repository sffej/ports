COMMENT =	abstract puzzle game

DISTNAME =	chroma-1.13
REVISION =	3
EXTRACT_SUFX =	.tar.bz2
FIX_EXTRACT_PERMISSIONS=Yes

CATEGORIES =	games x11

HOMEPAGE =	http://level7.org.uk/chroma/

MAINTAINER =	LEVAI Daniel <leva@ecentrum.hu>

# GPLv2
PERMIT_PACKAGE =	Yes

WANTLIB =  SDL SDL_image c freetype iconv intl curses pthread z

SITES=		${HOMEPAGE}/download/

CONFIGURE_STYLE =	gnu

LIB_DEPENDS =	devel/gettext,-runtime \
		devel/sdl-image
CFLAGS +=	-fgnu89-inline


.include <bsd.port.mk>

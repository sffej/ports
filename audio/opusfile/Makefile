COMMENT =		high-level decoding and seeking API for Opus files

VERSION =		0.12
DISTNAME =		opusfile-${VERSION}
CATEGORIES =		audio

SHARED_LIBS +=		opusfile                  1.0 # 4.5
SHARED_LIBS +=		opusurl                   1.0 # 4.5

HOMEPAGE =		https://opus-codec.org/
MAINTAINER =		Christian Weisgerber <naddy@openbsd.org>

# BSD
PERMIT_PACKAGE =	Yes

WANTLIB =		crypto m ogg opus ssl

SITES =		https://downloads.xiph.org/releases/opus/ \
		https://github.com/xiph/opusfile/releases/download/v${VERSION}/

LIB_DEPENDS =		audio/libogg \
			audio/opus

DEBUG_PACKAGES =	${BUILD_PACKAGES}

SEPARATE_BUILD =	Yes
CONFIGURE_STYLE =	gnu
CONFIGURE_ARGS =	--disable-maintainer-mode
CONFIGURE_ARGS +=	--disable-doc	# requires doxygen

.include <bsd.port.mk>

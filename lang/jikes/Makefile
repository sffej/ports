COMMENT=compile Java source into .class files (quickly!)

# Jikes, a fast Java compiler.

DISTNAME=	jikes-1.22
REVISION =	10
CATEGORIES=	lang
HOMEPAGE=	https://jikes.sourceforge.net/
SITES=		${SITE_SOURCEFORGE:=jikes/}
EXTRACT_SUFX=	.tar.bz2

MAINTAINER=	Yozo TODA <yozo@v007.vaio.ne.jp>

# IBM Public License
PERMIT_PACKAGE=	Yes

WANTLIB=		c iconv m ${COMPILER_LIBCXX}

COMPILER =		base-clang ports-gcc base-gcc

LIB_DEPENDS=	converters/libiconv

SEPARATE_BUILD=	Yes
CONFIGURE_STYLE=gnu

CONFIGURE_ENV=	CPPFLAGS="${CPPFLAGS} -I${LOCALBASE}/include" \
		LDFLAGS="${LDFLAGS} -L${LOCALBASE}/lib"

FAKE_FLAGS+=	docdir=${PREFIX}/share/doc/jikes/

.include <bsd.port.mk>

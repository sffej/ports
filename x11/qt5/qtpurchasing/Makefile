QT5NAME =		QtPurchasing
COMMENT-main =		in-app purchases in Qt5 and Qt5 Quick applications

MULTI_PACKAGES =	-main -examples

SHARED_LIBS +=  Qt5Purchasing                 1.0 # 5.9

WANTLIB += ${COMPILER_LIBCXX} GL Qt5Core Qt5Gui Qt5Network Qt5Qml
WANTLIB += Qt5QmlModels Qt5Quick m

LIB_DEPENDS =		x11/qt5/qtdeclarative>=${QT5_VERSION},<${QT5_NEXT_VERSION}

FLAVORS =		debug

.include <bsd.port.mk>

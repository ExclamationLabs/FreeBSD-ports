# $FreeBSD$

PORTNAME=	kalgebra
DISTVERSION=	${KDE_APPLICATIONS_VERSION}
CATEGORIES=	math kde kde-applications

MAINTAINER=	kde@FreeBSD.org
COMMENT=	KDE graph calculator

LIB_DEPENDS=	libAnalitza.so:math/analitza
BUILD_DEPENDS=	${LOCALBASE}/share/xsl/docbook/html/docbook.xsl:textproc/docbook-xsl \
		docbook-xml>0:textproc/docbook-xml

CMAKE_ARGS=	-DBUILD_mobile:BOOL=FALSE
USES=		cmake:outsource gettext kde:5 qt:5 tar:xz
USE_GL=		glu
USE_KDE=	auth codecs config configwidgets coreaddons doctools ecm i18n \
		kio service widgetsaddons xmlgui
USE_QT=		core dbus gui location network opengl printsupport qml quick \
		svg testlib webchannel webengine widgets xml \
		buildtools_build qmake_build

.include <bsd.port.mk>

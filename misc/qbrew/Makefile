# $NetBSD: Makefile,v 1.29 2016/03/05 11:28:57 jperkin Exp $

DISTNAME=	qbrew-0.4.1
PKGREVISION=	3
CATEGORIES=	misc
MASTER_SITES=	http://www.usermode.org/code/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://www.usermode.org/code.html
COMMENT=	Homebrewer's recipe calculator

USE_LANGUAGES=	c c++
USE_TOOLS+=	gmake
HAS_CONFIGURE=	yes
USE_LIBTOOL=	yes

BUILDLINK_DEPMETHOD.libXt?=	build

CONFIGURE_ARGS+=	--prefix=${DESTDIR}${PREFIX}
CONFIGURE_ARGS+=	--qtdir=${QTDIR}

.include "../../x11/libSM/buildlink3.mk"
.include "../../x11/libX11/buildlink3.mk"
.include "../../x11/libXt/buildlink3.mk"
.include "../../x11/qt4-tools/buildlink3.mk"
.include "../../x11/qt4-libs/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"

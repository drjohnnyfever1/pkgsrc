# $NetBSD: Makefile,v 1.2 2014/09/27 10:11:20 jperkin Exp $

DISTNAME=	HElib-20130501
CATEGORIES=	security
MASTER_SITES=	${MASTER_SITE_LOCAL}
EXTRACT_SUFX=	.zip

MAINTAINER=	agc@NetBSD.org
HOMEPAGE=	http://github.com/shaih/HElib/
COMMENT=	Homeomorphic Encryption library
LICENSE=	gnu-gpl-v2

WRKSRC=		${WRKDIR}/HElib-master/src

USE_LANGUAGES+=	c++
USE_TOOLS+=	gmake

TEST_TARGET=	check

AUTO_MKDIRS=	yes

pre-patch:
	for f in ${WRKSRC}/Makefile ${WRKSRC}/NumbTh.h; do	\
		${TR} -d '\r' < $${f} > $${f}.new;		\
		${MV} $${f}.new $${f};				\
	done

.include "../../devel/gmp/buildlink3.mk"
.include "../../math/ntl/buildlink3.mk"

.include "../../mk/bsd.pkg.mk"

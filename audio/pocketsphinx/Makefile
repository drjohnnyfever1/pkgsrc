# $NetBSD: Makefile,v 1.1 2014/09/05 10:13:20 fhajny Exp $

DISTNAME=	pocketsphinx-0.8
CATEGORIES=	audio
MASTER_SITES=	${MASTER_SITE_SOURCEFORGE:=cmusphinx/}

MAINTAINER=	filip@joyent.com
HOMEPAGE=	http://cmusphinx.sourceforge.net/
COMMENT=	CMUSphinx speech recognition C library
LICENSE=	2-clause-bsd

GNU_CONFIGURE=	yes
USE_LIBTOOL=	yes
USE_TOOLS+=	pkg-config

PKGCONFIG_OVERRIDE+=	pocketsphinx.pc.in

CONFIGURE_ARGS+=	--without-python

.include "../../audio/sphinxbase/buildlink3.mk"
.include "../../lang/python/application.mk"
.include "../../mk/bsd.pkg.mk"

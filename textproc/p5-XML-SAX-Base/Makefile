# $NetBSD: Makefile,v 1.12 2017/06/05 14:24:58 ryoon Exp $

DISTNAME=	XML-SAX-Base-1.09
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	1
CATEGORIES=	textproc perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=XML/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/XML-SAX-Base/
COMMENT=	Perl base class SAX Drivers and Filters
LICENSE=	${PERL5_LICENSE}

PERL5_PACKLIST=	auto/XML/SAX/Base/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"

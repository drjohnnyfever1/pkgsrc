# $NetBSD: Makefile,v 1.30 2017/06/05 14:23:30 ryoon Exp $
#

DISTNAME=	Proc-Daemon-0.23
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	2
CATEGORIES=	devel perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Proc/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://www.mhonarc.org/~ehood/earlsperls.html
COMMENT=	Provide capability for a Perl program to run as a daemon
LICENSE=	${PERL5_LICENSE}

BUILD_DEPENDS=	p5-Proc-ProcessTable>=0:../../devel/p5-Proc-ProcessTable

PERL5_PACKLIST=		auto/Proc/Daemon/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"

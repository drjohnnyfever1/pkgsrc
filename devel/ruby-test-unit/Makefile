# $NetBSD: Makefile,v 1.28 2017/06/12 17:10:23 taca Exp $

DISTNAME=	test-unit-3.2.4
CATEGORIES=	devel

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/test-unit/test-unit/
COMMENT=	Improved version of Test::Unit
LICENSE=	ruby-license

USE_LANGUAGES=	# none

.include "../../lang/ruby/rubyversion.mk"

.if ${RUBY_VER} == "21"
DEPENDS+=	${RUBY_PKGPREFIX}-power_assert>=0:../../devel/ruby-power_assert
.endif

.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"

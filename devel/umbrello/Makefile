# $NetBSD: Makefile,v 1.38 2017/04/30 01:21:34 ryoon Exp $

DISTNAME=	umbrello-${_KDE_VERSION}
PKGREVISION=	6
CATEGORIES=	devel
COMMENT=	UML Modeller

PYTHON_VERSIONS_INCOMPATIBLE=	34 35 36 # not yet ported as of 4.11.3

.include "../../meta-pkgs/kde4/Makefile.kde4"

REPLACE_PERL+= \
	umbrello/headings/heading.pm

REPLACE_PYTHON+= \
	umbrello/headings/heading.py

REPLACE_RUBY+= \
	umbrello/headings/heading.rb

#BUILDLINK_DEPMETHOD.qt4-tools=	full
.include "../../meta-pkgs/kde4/kde4.mk"

.include "../../devel/boost-libs/buildlink3.mk"
#.include "../../devel/libltdl/buildlink3.mk"
#.include "../../devel/subversion-base/buildlink3.mk"
.include "../../graphics/hicolor-icon-theme/buildlink3.mk"
.include "../../lang/python/application.mk"
.include "../../lang/ruby/replace.mk"
#.include "../../misc/kdepimlibs4/buildlink3.mk"
#.include "../../security/qca2/buildlink3.mk"
.include "../../sysutils/desktop-file-utils/desktopdb.mk"
#.include "../../textproc/hunspell/buildlink3.mk"
.include "../../x11/kdelibs4/buildlink3.mk"
#.include "../../x11/kde-baseapps4/buildlink3.mk"
#.include "../../x11/kde-runtime4/buildlink3.mk"
#.include "../../x11/kde-workspace4/buildlink3.mk"

.include "../../mk/bsd.pkg.mk"

# Contributor: Anonymous
# Generator  : CPANPLUS::Dist::Arch 1.21

pkgname='perl-rdf-vcard-babelfish'
pkgver='0.007'
pkgrel='1'
pkgdesc="convert between myriad contact formats"
arch=('any')
license=('PerlArtistic' 'GPL')
options=('!emptydirs')
depends=('perl>=5.008' 'perl-common-sense' 'perl-digest-sha1' 'perl-html-microformats>=0.103' 'perl-json>=2.00' 'perl-rdf-rdfa-generator' 'perl-rdf-rdfa-parser>=1.094' 'perl-rdf-trine>=0.130' 'perl-rdf-vcard>=0.007' 'perl-xml-libxml>=1.70')
makedepends=('perl-module-signature>=0.66')
url='http://search.cpan.org/dist/RDF-vCard-Babelfish'
source=('http://search.cpan.org/CPAN/authors/id/T/TO/TOBYINK/RDF-vCard-Babelfish-0.007.tar.gz')
md5sums=('2f18e7f122a5e451f8aff56bcc638904')
sha512sums=('041eabfa9c37a5245228fd613952e4bf78143eddd75d1451b872050a1573e2ef5935694913e1c5aa80a9fbc465e1006f9748a62a777b09393117c155ce037292')
_distdir="${srcdir}/RDF-vCard-Babelfish-0.007"

build() {
  ( export PERL_MM_USE_DEFAULT=1 PERL5LIB=""                 \
      PERL_AUTOINSTALL=--skipdeps                            \
      PERL_MM_OPT="INSTALLDIRS=vendor DESTDIR='$pkgdir'"     \
      PERL_MB_OPT="--installdirs vendor --destdir '$pkgdir'" \
      MODULEBUILDRC=/dev/null

    cd "$_distdir"
    /usr/bin/perl Makefile.PL
    make
  )
}

#check() {
#  cd "$_distdir"
#  ( export PERL_MM_USE_DEFAULT=1 PERL5LIB=""
#    make test
#  )
#}

package() {
  cd "$_distdir"
  make install
  find "$pkgdir" -name .packlist -o -name perllocal.pod -delete
}

# Local Variables:
# mode: shell-script
# sh-basic-offset: 2
# End:
# vim:set ts=2 sw=2 et:

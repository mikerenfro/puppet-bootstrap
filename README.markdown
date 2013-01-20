Mike Renfro's shell script and supporting files to bootstrap a
puppet client on a new Debian install. Currently uses:

  * puppet packages from apt.puppetlabs.com
  * an already-configured puppetmaster (see https://github.com/mikerenfro/puppetmaster-bootstrap for scripts to build one if you don't already have one)

Installation:

  1. mkdir (target); cd (target)
  2. wget -O puppet-bootstrap.tgz https://github.com/mikerenfro/puppet-bootstrap/tarball/master
  3. tar --strip-components=1 -zxvpf puppet-bootstrap.tgz 
  4. ./bootstrap fqdn.of.puppet.master

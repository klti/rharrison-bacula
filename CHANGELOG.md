## 2012-10-24  Russell Harrison <rharrison@fedoraproject.org> - 0.0.4
* Fix MySQL database management
* Specify perms for file resources
* Clean up resource relationships
* Simplify and update documentation
* Migrate `bacula::config::client` to `bacula::client::config`
* Allow `bacula::client::config` to be called directly to allow configuring
  clients with exported resources
* Proper application of the ASL 2.0
* Move to using fqdn instead of shorter names to simplify management and prevent
  name collisions
* Stop using scope.lookupvar and allow vars to be passed in as params
* Merge [pull request](https://github.com/rharrison10/rharrison-bacula/pull/1)
  from [Erik Smit](https://github.com/erik-smit)
* Syntax cleanup

### 2012-10-24  erik-smit <smite@zylon.net>
* Config default plugin directory for file daemon
* Fix bconsole director name (this is _NOT_ Console)
* Fixing catalog support for postgres
* Add Debian/Ubuntu package naming
* Add minimalistic postgres support

### 2012-09-21  Russell Harrison <rharrison@fedoraproject.org>
* Moving db management out of common to director and creating subclasses for each backend

### 2012-09-20  Russell Harrison <rharrison@fedoraproject.org>
* Changing variables to not be puppet reserved words
* Make sure packages are installed before baclula user and group are defined

## Wed Sep 19 2012 Russell Harrison <rharrison@fedoraproject.org> - 0.0.3

* Documenting this is a fork under my name.
* Simple script to update installed module by hand.
* Modified to work properly with RHEL.
* Remove God aweful global variables. Imposible to maintain.
* Move bacula::config::validate to bacula::params::validate.
* Clean up formating to comply with the style guide.
* Update documentation to reflect changes.

## Thu Dec 15 2011 Carl Caum <carl@puppetlabs.com> - 0.0.2

* Support multiple DB backends
* Support Managing databases through 3rd party modules
* Ability to declare clients through class parameters
  or ENC variables
* Documentation improvements

## Thu Dec  8 2011 Carl Caum <carl@puppetlabs.com> - 0.0.1

* Manage a Bacula director
* Manage Bacula clients
* Manage a Bacula storage daemon
* Manage console installations
* Customize configuration files with custom templates
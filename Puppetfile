# This file manages Puppet module dependencies.
#
# It works a lot like Bundler. We provide some core modules by
# default. This ensures at least the ability to construct a basic
# environment.

def github(name, version, options = nil)
  options ||= {}
  options[:repo] ||= "boxen/puppet-#{name}"
  mod name, version, :github_tarball => options[:repo]
end

# Includes many of our custom types and providers, as well as global
# config. Required.

github "boxen",      "3.0.2"

# Core modules for a basic development environment. You can replace
# some/most of these if you want, but it's not recommended.

github "autoconf",   "1.0.0"
github "gcc",        "2.0.1"
github "git",        "1.2.5"
github "homebrew",   "1.4.1"
github "hub",        "1.0.3"
github "inifile",    "1.0.0", :repo => "puppetlabs/puppetlabs-inifile"
github "openssl",    "1.0.0"
github "repository", "2.2.0"
github "ruby",       "6.3.4"
github "stdlib",     "4.1.0", :repo => "puppetlabs/puppetlabs-stdlib"
github "sudo",       "1.0.0"
github "xquartz",    "1.1.0"

# Optional/custom modules. There are tons available at
# https://github.com/boxen.
github "adium",      "1.2.0"
github "skype",      "1.0.6"
github "dropbox",    "1.1.1"
github "chrome",     "1.1.1"
github "alfred",     "1.1.5"
github "caffeine",   "1.0.0"
github "air_server", "1.0.1", :repo => "febbraro/puppet-air_server"
github "googlevoiceandvideoplugin", "1.0.0", :repo => "phase2/puppet-googlevoiceandvideoplugin"
github "property_list_key", "0.1.0", :repo => "glarizza/puppet-property_list_key"

# Some local, private modules
mod    "iwork",     :git => "git@bitbucket.org:phase2tech/puppet-iwork.git", :ref => "1.0.2"
mod    "msoffice",  :git => "git@bitbucket.org:phase2tech/puppet-msoffice.git", :ref => "1.0.1"
mod    "p2fonts",   :git => "git@bitbucket.org:phase2tech/puppet-p2fonts.git", :ref => "1.0.1"
mod    "confroom_osx",    :git => "git@bitbucket.org:phase2tech/puppet-confroom_osx.git", :ref => "master"
mod    "purge_downloads", :git => "git@bitbucket.org:phase2tech/puppet-purge_downloads.git", :ref => "master"




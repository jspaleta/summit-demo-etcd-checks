## Sensu-Plugins-etcd

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-etcd.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-etcd)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-etcd.svg)](http://badge.fury.io/rb/sensu-plugins-etcd)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-etcd/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-etcd)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-etcd/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-etcd)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-etcd.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-etcd)
[![Sensu Bonsai Asset](https://img.shields.io/badge/Bonsai-Download%20Me-brightgreen.svg?colorB=89C967&logo=sensu)](https://bonsai.sensu.io/assets/jspaleta/sensu-plugins-etcd)

## Sensu Asset  
  The Sensu assets packaged from this repository are built against the Sensu ruby runtime environment. When using these assets as part of a Sensu Go resource (check, mutator, handler or hook), make sure you include the corresponding Sensu ruby runtime asset in the list of assets needed by the resource.  The current ruby-runtime assets can be found [here](https://bonsai.sensu.io/assets/sensu/sensu-ruby-runtime) in the [Bonsai Asset Index](bonsai.sensu.io).


## Functionality

## Files
 * bin/check-etcd.rb
 * bin/check-etcd-peer-count.rb
 * bin/check-flannel-subnet-count.rb
 * bin/metrics-etcd.rb

## Usage

### check-etcd.rb
    Usage: check-etcd.rb (options)
           --ca CA                      SSL CA file
           --cert CERT                  client SSL cert
           --insecure                   change SSL verify mode to false
           --key KEY                    client SSL key
           --passphrase PASSPHRASE      passphrase of the SSL key
       -p, --port PORT                  Etcd port, defaults to 2379
       -h, --host HOST                  Etcd host, defaults to localhost
           --ssl                        use HTTPS (default false)

### check-etcd-peer-count.rb
    Usage: check-etcd-peer-count.rb (options)
           --ca CA                      SSL CA file
           --cert CERT                  client SSL cert
           --insecure                   change SSL verify mode to false
           --key KEY                    client SSL key
           --passphrase PASSPHRASE      passphrase of the SSL key
       -c, --count NUMBER               Number of expected etcd peers (required)
       -p, --port PORT                  Etcd port, defaults to 2379
       -h, --host HOST                  Etcd host, defaults to localhost
           --ssl                        use HTTPS (default false)
### check-flannel-subnet-count.rb
    Usage: /home/jspaleta/.rvm/gems/ruby-2.4.1/bin/check-flannel-subnet-count.rb (options)
           --ca CA                      SSL CA file
           --cert CERT                  client SSL cert
           --insecure                   change SSL verify mode to false
           --key KEY                    client SSL key
           --passphrase PASSPHRASE      passphrase of the SSL key
       -p, --port PORT                  Etcd port, defaults to 2379
       -h, --host HOST                  Etcd host, defaults to localhost
           --ssl                        use HTTPS (default false)
       -w, --warn COUNT                 Warn when number of subnets exceeds the max minus this threshold

### metrics-etcd.rb
    Usage: metrics-etcd.rb (options)
           --ca CA                      SSL CA file
           --cert CERT                  client SSL cert
       -h, --host HOST                  Etcd host, defaults to localhost
       -p, --port PORT                  Etcd port, defaults to 2379
           --insecure                   change SSL verify mode to false
           --key KEY                    client SSL key
       -l, --leader-stats               Show leader stats
           --passphrase PASSPHRASE      passphrase of the SSL key
       -s, --scheme SCHEME              Metric naming scheme
           --ssl                        use HTTPS (default false)


## Installation

[Installation and Setup](http://sensu-plugins.io/docs/installation_instructions.html)

## Notes

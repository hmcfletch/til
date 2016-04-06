# dnsmasq

## Setup dnsmasq

1. `brew install dnsmasq`
2. Do what ever it tells you in the post install
3. Add `address=/<YOUR LOCAL DOMAIN OR TLD>/127.0.0.1` to `/usr/local/etc/dnsmasq.conf`.
4. `sudo launchctl stop homebrew.mxcl.dnsmasq`
5. `sudo launchctl start homebrew.mxcl.dnsmasq`
6. Test
    * `dig testing.<YOUR LOCAL DOMAIN OR TLD> @127.0.0.1`
    * There should be an `;; ANSWER SECTION:` in the output that lists the url you tested.

## Setup OSX

1. `sudo mkdir -p /etc/resolver`
2. Add `nameserver 127.0.0.1` to `/etc/resolver/<YOUR LOCAL DOMAIN OR TLD>`
3. Test
    * ping -c 1 www.google.com
    * ping -c 1 this.is.a.test.&lt;YOUR LOCAL DOMAIN OR TLD&gt;

### Notes
* Don't use `.dev`, [It's a real TLD](https://iyware.com/dont-use-dev-for-development/)
* If you are using Rails 4.2+, you'll have to use `rails s -b 0.0.0.0` to make use of this

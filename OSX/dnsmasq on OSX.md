# dnsmasq on OSX
When you want to use your laptop as a DNS router, so you test mobile web on a real device.

# Essential setup for OSX and iPhone
https://stackoverflow.com/questions/7473939/iphone-add-entry-to-etc-hosts-without-jailbreaking#20628104

## check that everything is working as expected
- do you get the correct IP for expected domain?
`dig <domain> @127.0.0.1`

- can you still resolve DNS names that dnsmasq is not handling?
ping -c 1 google.com

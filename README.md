pfloghtml
=========

pfloghtml is a simple and quick log parsing program for Packet Filter
log files. pfloghtml can be used for viewing PF logs via web interface.

Copy pfloghtml file from distribution directory to /usr/local/sbin.
Create /var/www/htdocs/pflog directory. Add the following line in
crontab:

	*/5 * * * * /usr/local/sbin/pfloghtml

If done as a non-root user, make sure to use sudo.

Point your webserver to /var/www/htdocs/pflog. Following example for
Apache.

	<VirtualHost _default_:80>
	    DocumentRoot /var/www/htdocs/pflog
	</VirtualHost>

pfloghtml is written by Dmitry Alenichev <mitya@rockers.su> and licensed
under a ISC/BSD licence.


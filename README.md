# etc.vonahsen

configuration files and preferences

mostly self-explanitory

apt/apt.conf.d/00nophases:
* disable ubuntu phased updates

fail2ban/filter.d/wordpress-scammers.conf:
* almost anyone going straight at wp-admin or wp-includes files is up to no good, log 400 and 500 codes, and ka-block
fail2ban/filter.d/wordpress-eme-scammers.conf:
* for one particular module, our use-case does not use payments, anyone going straight to those files is up to no good.
fail2ban/jail.d/vonahsen-wordpress.conf:
* enable the filters above

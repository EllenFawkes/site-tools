# site-tools
Apache2 site tools for creating, editing or removing virtual hosts

## How to install

Clone site-tools git repository and copy scripts into `/usr/sbin`

```bash
git clone https://github.com/EllenFawkes/site-tools.git
sudo cp site-* /usr/sbin
```

## Usage

```bash
site-create <sitename> # Create an APACHE2 site (virtual host)
site-edit <sitename> # Edit virtual host config
site-remove <sitename> # Remove a site (virtual host)
```

## Configuration

### Default configuration

```bash
SITENAME=$1 # Do not change it
CONF=/etc/apache2/sites-available/${SITENAME}.conf # Path to site's virtual host config file 
WWW_PATH=/var/www # Path to WWW dir of sites
EDITOR=vim # Editor for editing virtual host config file (default VIM)
```

### Custom configuration

Do you want customize site-tools configuration, create a config file `/etc/site-tools.conf` and redefine properties from defaults.

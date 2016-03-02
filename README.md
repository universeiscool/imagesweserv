[![Author](https://img.shields.io/badge/author-andrieslouw-blue.svg?style=flat-square)](https://github.com/andrieslouw)
[![Author](https://img.shields.io/badge/author-kleisauke-blue.svg?style=flat-square)](https://github.com/kleisauke)
[![Source Code](https://img.shields.io/badge/source-andrieslouw/imagesweserv-blue.svg?style=flat-square)](https://github.com/andrieslouw/imagesweserv)
[![Software License](https://img.shields.io/badge/license-BSD3-brightgreen.svg?style=flat-square)](https://tldrlegal.com/license/bsd-3-clause-license-%28revised%29)

<a href="https://github.com/php"><img src="https://images.weserv.nl/?url=nl3.php.net/images/logos/php-med-trans.png&h=40" align="right" /></a>
<img src="https://images.weserv.nl/?url=upload.wikimedia.org/wikipedia/commons/thumb/f/f7/Slash.svg/200px-Slash.svg.png&h=35" align="right" />
<a href="https://github.com/nginx"><img src="https://images.weserv.nl/?url=nginx.org/nginx.gif&w=150&h=38&t=square" align="right" /></a>
# Images.weserv.nl

Source code of images.weserv.nl, to be used on your own server(s).

## Setup with DigitalOcean
Setup with a 512MB / 1CPU  – Ubuntu (14.04.4 x64)
``` bash
apt-get install nginx
apt-get install php5-fpm
```

``` bash
mkdir /var/www
chown -R www-data:www-data /var/www
cd /var/www
git clone https://github.com/universeiscool/imagesweserv.git
```

``` bash
mv /etc/nginx/nginx.conf /etc/nginx/nginx.conf.backup
ln -s /var/www/imagesweserv/nginx/nginx.conf /etc/nginx/nginx.conf

mv /etc/php5/fpm/pool.d/www.conf /etc/php5/fpm/pool.d/www.conf.backup
ln -s /var/www/imagesweserv/php-fpm/php-fpm.conf /etc/php5/fpm/pool.d/images-php-fpm.conf
```

``` bash
apt-get install php5-intl
apt-get install php5-curl
apt-get install php5-gd
```

## Documentation

Full documentation can be found at [images.weserv.nl](https://images.weserv.nl/).

## Support

[UserVoice forum](https://imagesweserv.uservoice.com/).

## Credits
[![Andries Louw Wolthuizen](https://avatars2.githubusercontent.com/u/11487455?v=3&s=120)](https://github.com/andrieslouw) | [![Kleis Auke Wolthuizen](https://avatars2.githubusercontent.com/u/12746591?v=3&s=120)](https://github.com/kleisauke)
------------- | -------------
[Andries Louw Wolthuizen](https://github.com/andrieslouw) | [Kleis Auke Wolthuizen](https://github.com/kleisauke)

## License

The BSD 3-Clause License. Please see [LICENSE.md](https://github.com/andrieslouw/imagesweserv/blob/master/LICENSE.md) for more information.

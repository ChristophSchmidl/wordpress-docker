# Wordpress installation based on Docker and Docker-Compose

## What should it contain?

* Docker with Docker-Compose for easy containerization
* Webserver: Nginx
* Database: MySQL, MariaDB, PostgreSQL
* PHP: php7.3-fpm
* Let's Encrypt for free SSL/TLS certificates
* Router: Traefik (https://docs.traefik.io/) or nginx-proxy (https://github.com/nginx-proxy/nginx-proxy)
* Bedrock (Optional): https://roots.io/bedrock/
* WP-CLI (command-line interface for WordPress): https://wp-cli.org/
* PhpMyAdmin if MySQL or MariaDB is used, PgAdmin if PostgreSQL is used
* Should support multi-website setup (traefik or jwilder/nginx-proxy)

## Similar repositories

* https://github.com/evertramos/docker-wordpress-letsencrypt
	* 300 Stars
* https://github.com/bitnami/bitnami-docker-wordpress-nginx
	* 51 Stars	
* https://github.com/mjstealey/wordpress-nginx-docker
	* 373 Stars
* https://github.com/eugeneware/docker-wordpress-nginx
	* 857 Stars
* https://github.com/urre/wordpress-nginx-docker-compose
	* 159 Stars
* https://github.com/TrafeX/docker-wordpress
	* 121 Stars
* https://github.com/raulr/nginx-wordpress-docker
	* 44 Stars
* https://github.com/gabidavila/docker-wordpress-ssl-nginx-mysql
	* 3 Stars	

## Tutorials 

* http://geekyplatypus.com/dockerise-your-php-application-with-nginx-and-php7-fpm/ (looks good)
* https://urre.me/writings/docker-for-local-wordpress-development/ (good, with bedrock)
* https://www.howtoforge.com/tutorial/dockerizing-wordpress-with-nginx-and-php-fpm/	
* https://welaunch.io/de/2018/02/docker-tutorial/
* https://medium.com/today-i-solved/wordpress-over-https-with-docker-ssl-ecaf02a47fea
* https://jimfrenette.com/2018/05/wordpress-from-development-to-production-using-docker/

### Multi-website Setup 

* https://blog.ssdnodes.com/blog/host-multiple-ssl-websites-docker-nginx/
* https://blog.ssdnodes.com/blog/install-traefik-multiple-ssl-websites/
* https://medium.com/@francoisromain/set-a-local-web-development-environment-with-custom-urls-and-https-3fbe91d2eaf0
* https://medium.com/@francoisromain/host-multiple-websites-with-https-inside-docker-containers-on-a-single-server-18467484ab95
* https://blog.programster.org/hosting-multiple-dockerized-websites-on-a-single-host
* https://blog.florianlopes.io/host-multiple-websites-on-single-host-docker/
* https://blog.maqe.com/creating-multi-site-development-environment-with-docker-570a382dd295

## TODO

- [ ] Work through the tutorial and come up with a simple docker/docker-compose file: http://geekyplatypus.com/dockerise-your-php-application-with-nginx-and-php7-fpm/
- [ ] What is better for a multi-website setup? Traefik or nginx-proxy?
- [ ] Create prototypes with both setups
- [ ] How do both setups handle the creation of ssl certificates? Let's encrypt integration
- [ ] How to backup wordpress and import it into another docker container?
- [ ] How to restart multi-website docker setup automatically after restart?
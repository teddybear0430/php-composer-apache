FROM amazonlinux:1

RUN yum -y install sudo
RUN yum -y install php73.x86_64 php73-bcmath.x86_64 php73-cli.x86_64 php73-common.x86_64 php73-gd.x86_64 php73-json.x86_64 php73-mbstring.x86_64 php73-mysqlnd.x86_64 php73-pdo.x86_64 php73-intl.x86_64 php73-xml.x86_64
RUN yum -y install vim
COPY --from=composer /usr/bin/composer /usr/bin/composer

COPY php.ini /etc/php.ini

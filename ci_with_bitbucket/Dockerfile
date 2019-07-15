FROM mysql:5.6.40

# Python 3.5
RUN apt-get update
RUN apt-get install -y --allow-unauthenticated libmysqlclient-dev libcurl4-openssl-dev libssl-dev python3-pip

# Flake8
RUN pip3 install flake8

# Copy files
COPY script/common.sql /
COPY script/ec.sql /
COPY script/user_glowmee.sql /
COPY script/privilege.sql /
COPY script/common.ini /


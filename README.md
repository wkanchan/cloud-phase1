== How to set up 

Amazon Linux AMI (HVM) 2013.09.2 - ami-e9a18d80
# This is an H1

## This is an H2

###### This is an H6
# Install git, rails, mysql, sqlite #

\curl -sSL https://get.rvm.io | bash - s stable
source ~/.profile
rvm install 1.9.3
rvm alias create default 1.9.3
sudo yum -y install rubygems sqlite-devel git gcc mysql-devel ruby-devel mysql
gem install rails --no-ri --no-rdoc
gem install mysql2 --no-ri --no-rdoc

# Run rails on port 80
rvmsudo rails s -p 80
</code>

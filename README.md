# demo-berkshelf-17

# Requirements

# Usage
vagrant plugin install vagrant-lxc
vagrant plugin install vagrant-berkshelf
vagrant up --provider=lxc # This will complete successfully
vagrant ssh
  ls /tmp/vagrant-chef-1/chef-solo-1/cookbooks/ # will show cookbooks have been loaded on guest
  exit
vagrant provision # this will fail, unable to find any cookbooks
vagrant ssh
  ls /tmp/vagrant-chef-1/chef-solo-1/cookbooks/ # will show no cookbooks loaded, empty dir instead
  exit

# Attributes

# Recipes

# Author

Author:: YOUR_NAME (<YOUR_EMAIL>)

# demo-berkshelf-17
Repo to demo berkshelf issue 17: https://github.com/RiotGames/vagrant-berkshelf/issues/17

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

vagrant halt

vagrant up # works again

# Attributes

# Recipes

# Author

Author:: YOUR_NAME (<YOUR_EMAIL>)

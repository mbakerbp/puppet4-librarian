Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
 
  # match the hiera node file from earlier
  config.vm.hostname = "nagios"

  config.vm.synced_folder ".", "/tmp/puppet"

#  config.vm.provision "shell",
#    inline: "
#	cd ~ && wget https://apt.puppetlabs.com/puppetlabs-release-pc1-trusty.deb
#	sudo dpkg -i puppetlabs-release-pc1-trusty.deb
#        puppet apply /etc/puppet/environments/production/manifests/site.pp --confdir=/etc/puppet/ --environment=production --environmentpath=/etc/puppet/environments/
#    "
end

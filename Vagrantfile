# -*- mode: ruby -*-
# vi: set ft=ruby :

last_key = ""
hosts = IO.readlines("./hosts").inject({}) do |r, line|
  if md = line.match(/^\[(.*)\]$/)
    r.store md[1], []
    last_key = md[1]
  elsif md = line.match(/^([[0-9]\.]*).*$/)
    r[last_key] << md[1]
  end
  r
end
Vagrant.configure("2") do |config|
  config.vm.box = "https://googledrive.com/host/0B4tZlTbOXHYWVGpHRWZuTThGVUE/centos65_virtualbox_50G.box"

  config.vm.network :private_network, ip: hosts["vagrant"].first

  config.vm.provision :ansible do |ansible|
    ansible.playbook = 'playbook.yml'
    ansible.inventory_path = 'hosts'
    ansible.limit = 'all'
  end
end

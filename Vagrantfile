# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant::Config.run do |config|
  config.vm.define :TestServer do |cfg|
    cfg.vm.box = "base64"
    cfg.vm.network :hostonly, "192.168.50.101"
    cfg.vm.host_name = "TestServer"
    cfg.vm.forward_port 80, 9090
    cfg.vm.provision "shell", path: "provision.sh"
  end
end

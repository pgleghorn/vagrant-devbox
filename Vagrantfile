Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.network "forwarded_port", guest: 8080, host: 8080, auto_correct: true, id: "jenkins"
  config.vm.network "forwarded_port", guest: 8081, host: 8081, auto_correct: true, id: "nexus"
  config.vm.network "forwarded_port", guest: 3000, host: 3000, auto_correct: true, id: "gitea-http"
  config.vm.network "forwarded_port", guest: 8222, host: 8222, auto_correct: true, id: "gitea-ssh"

  config.vm.provision "ansible_local" do |ansible|
    ansible.galaxy_role_file = "requirements.yml"
    ansible.verbose = "true"
    ansible.playbook = "main.yml"
    ansible.install_mode = "default"
  end
end

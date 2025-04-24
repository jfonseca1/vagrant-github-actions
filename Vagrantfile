Vagrant.configure("2") do |config|
    config.vm.box = "generic/ubuntu1804"

    config.vm.define 'ubuntu'

    # Prevent SharedFoldersEnableSymlinksCreate errors
    config.ssh.insert_key = false
    config.ssh.private_key_path = "~/.vagrant.d/insecure_private_key"
    config.vm.synced_folder ".", "/vagrant", disabled: true
end

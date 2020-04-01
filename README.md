# Server Setup with Ansible

1. the Remote server needs to get updated
2. the ssh-keys needs to get copied with `ssh-copy-id -i ~/.ssh/id_ed25519`
3. the user need sudo rights without password. Add `chris ALL=(ALL) NOPASSWD: ALL` to `visudo`. Alternatively, the command can be passed with the angular-playbook command with `--extra-vars "ansible_sudo_pass={PASSWORD}"`
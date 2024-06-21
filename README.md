# Ansible To SSH Config

Simple and small ansible playbook to create ssh config based on ansible hosts

## Usage
### Variables:
- ansible_user — user which used to connect to server
- atsc_path — path where ssh config[s] will be saved
- ansible_ssh_key — local path to private ssh key
- atsc_confirm — confirmation variable

### Command
`ansible-playbook -e ansible_user='user' -e atsc_path='~/.ssh/config.d/atsc' -e ansible_ssh_key='~/.ssh/my_ed25519' -e atsc_confirm=true path/to/ssh_config.yaml`

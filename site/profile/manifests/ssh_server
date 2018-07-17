class profile::ssh_server {
	package {'openssh-server':
		ensure => present,
	}
	service { 'sshd':
		ensure => 'running',
		enable => 'true',
	}
	ssh_authorized_key { 'root@master.puppet.vm':
		ensure => present,
		user   => 'root',
		type   => 'ssh-rsa',
		key    => 'AAAAB3NzaC1yc2EAAAADAQABAAABAQCwZcW10nkSXMcn9hrN+pFBZm2wCmzxZJiBvBpU5Etych+IonyyF89VR5D6QPZGniMnbsaG6zcYx84hnQczax/oUY0+KwpP/KOsPBc6kbJxTGimT23w9x9wpDDRDprckEWNqOtCI6BF5AJVXX55FYeYfdWF9+KR4RUryOxXNDaAxaP7oBa4KzOuetoOPVdqP/oBRTBt0TQJRGH29yIN3TGY3QyqsnFe/eJrh688ECvG7ct//0qXogt+Fts56aibaxoDSIbrZXkbtnm13LYGtZcMuwC3DpasF5O4G9IDx3jYZM1WfkVkFg8SBJIYlBP+y/43OMXJ+TrGUYqD9Lm+LlWD',
	}  
}

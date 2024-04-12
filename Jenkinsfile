pipeline {

		agent {
				label {
						label "built-in"
						customWorkspace "/mnt/project/"
				}
		}
		stages {
		
				stage ('stage1') {
					
						steps {
								sh "rm -rf *"
								sh "sudo git clone https://github.com/mahesh591w/repo2.git"
								sh "sudo cp -r /mnt/project/repo2/index.html /var/www/html/"
								sh "sudo systemctl restart httpd"
						}
				}
		}
}

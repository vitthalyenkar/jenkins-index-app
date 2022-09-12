pipeline{
       label{
	           label "built-in"
			   customWorkspace "/data/pipeline"
	stages{
	       stage ('Install-apache'){
				    steps {
						sh 'yum install httpd -y'
										 
					}
				}
				
			stage ('deploy-index'){
				    steps {
						sh 'cp -r index.html /var/www/html'
						sh 'chmod 755 /var/www/html/index.html'
										 
					}
				}

			stage ('Restart-apache'){
				    steps {
						sh 'service httpd restart'
										 
					}
				}
			
			}
		}			

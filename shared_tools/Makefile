b:	
	docker   build   -t  bbekzod/my_tools           .
	docker   push        bbekzod/my_tools
	docker   run         bbekzod/my_tools   terraform  --version
	docker   run         bbekzod/my_tools   packer     --version
	docker   run         bbekzod/my_tools   gcloud     --version
	docker   run         bbekzod/my_tools   aws        --version
cleanup:
	docker  image prune  -f 


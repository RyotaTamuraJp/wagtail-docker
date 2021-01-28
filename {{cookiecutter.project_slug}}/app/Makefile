setup:
	wagtail start mysite
	cp -r preconfigured/mysite mysite
	make migrate
	python mysite/manage.py createsuperuser
migrate:
	python mysite/manage.py migrate
run:
	python mysite/manage.py runserver 0.0.0.0:8000
delete:
	rm -rf mysite
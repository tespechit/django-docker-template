web: gunicorn --pythonpath {{ project_name}} {{ project_name}}.wsgi -w 4
worker: celery --workdir={{ project_name}} -c 4 -A {{ project_name}} -l info worker
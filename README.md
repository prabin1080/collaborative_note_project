### Building and running application

Initialize Submodules
```bash
git submodule update --init --recursive
```
Update Submodules
```bash
git submodule update --remote --merge
```

Build Docker Container
```bash
docker compose build
```
Migrate DB:
```bash
docker compose run server ./manage.py migrate
```
Create Superuser (Optional):
```bash
docker compose run server ./manage.py createsuperuser
```
Run:
```bash
docker compose up

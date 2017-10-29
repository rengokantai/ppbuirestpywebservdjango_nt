# ppbuirestpywebservdjango_nt
```
python -m venv --without-pip C:\to\path
pip install django-filter
activate.bat
deactivate.bat
```

### Creating the Models
```
sqlite3
.open db.sqlite3
.databases
.tables
```

### Managing Serialization and Deserialization
```
python manage.py shell
```
```
from datetime import datetime
from django.utils import timezone
from django.utils.six import BytesIO
from rest_framework.renderers import JSONRenderer
from rest_framework.parsers import JSONParser
from games.models import Game
from games.serializers import GameSerializer
```

then
```
game1 = Game(name='',release_date=gamedatetime, game_category='testname',played=False)
game1.save()
game_serializer1 = GameSerializer(game1)
print(game_serializer1.data)
```

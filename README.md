# django-admin-theme-collection
django-admin-theme-collection

# django theme
1. django-admin-bootstrapped
   - Looks like the last update was 8 years ago
   - Decided to ignore project testing
2. Django WP Admin
   - Looks like the last update was 3 years ago
   - Decided to ignore project testing
3. django-admin-tools :star: :star:
   - Freeware
   - doc : [django-admin-tools](https://django-admin-tools.readthedocs.io/en/latest/index.html)
   - git : [django-admin-tools](https://github.com/django-admin-tools/django-admin-tools)
   - setting :
        ```
        TEMPLATES = [
                {
                    'BACKEND': 'django.template.backends.django.DjangoTemplates',
                    'DIRS': [os.path.join(BASE_DIR, 'templates')],
                    # 'APP_DIRS': True,
                    'OPTIONS': {
                        'context_processors': [
                            'django.template.context_processors.debug',
                            'django.template.context_processors.request',
                            'django.contrib.auth.context_processors.auth',
                            'django.contrib.messages.context_processors.messages',
                        ],
                        'loaders': [
                            'admin_tools.template_loaders.Loader',
                            'django.template.loaders.app_directories.Loader',
                            'django.template.loaders.filesystem.Loader',
                        ],
                    },
                },
            ]
        ```
3. django-grappelli :star: :star:
   - Freeware
   - doc : [django-grappelli](https://django-grappelli.readthedocs.io/en/latest/)
   - github : [django-grappelli](https://github.com/sehmaschine/django-grappelli)
   - reference : [Django grappelli로 쓸만한 어드민 만들기](https://show-me-the-money.tistory.com/entry/Django-grappelli%EB%A1%9C-%EC%93%B8%EB%A7%8C%ED%95%9C-%EC%96%B4%EB%93%9C%EB%AF%BC-%EB%A7%8C%EB%93%A4%EA%B8%B0-1)
   - setting :
        ```
        INSTALLED_APPS = [
        'grappelli',
        "django.contrib.admin",
        "django.contrib.auth",
        "django.contrib.contenttypes",
        "django.contrib.sessions",
        "django.contrib.messages",
        "django.contrib.staticfiles",
        ]

        TEMPLATES = [
            {
                "BACKEND": "django.template.backends.django.DjangoTemplates",
                "DIRS": [],
                "APP_DIRS": True,
                "OPTIONS": {
                    "context_processors": [
                        "django.template.context_processors.debug",
                        "django.template.context_processors.request",
                        "django.contrib.auth.context_processors.auth",
                        "django.contrib.messages.context_processors.messages",
                    ],
                },
            },
        ]

        STATIC_URL = "static/"
        STATIC_ROOT = 'static'

        ```
4. Django JET
   - Looks like the last update was 4 years ago
   - Decided to ignore project testing
5. Django jazzmin :star: :star: :star:
   - Freeware
   - doc : [django-jazzmin](https://django-jazzmin.readthedocs.io/)
   - github : [django-jazzmin](https://github.com/farridav/django-jazzmin)
   - reference : 
     - [Making Django Admin Jazzy With django-jazzmin](https://djangocentral.com/making-django-admin-jazzy-with-django-jazzmin/)
     - [Setup Custom Django Admin using Jazzmin](https://www.youtube.com/watch?v=K7odN1MwyAA)

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
   - setting :
        ```
        #settings.py
        INSTALLED_APPS = [
            'jazzmin',
            "django.contrib.admin",
            "django.contrib.auth",
            "django.contrib.contenttypes",
            "django.contrib.sessions",
            "django.contrib.messages",
            "django.contrib.staticfiles",
        ]

        from .jazzmin import JAZZMIN_SETTINGS, JAZZMIN_UI_TWEAKS 

        JAZZMIN_SETTINGS  = JAZZMIN_SETTINGS
        JAZZMIN_UI_TWEAKS  = JAZZMIN_UI_TWEAKS 

        #jazzmin.py
        JAZZMIN_UI_TWEAKS = {
            "navbar_small_text": False,
            "footer_small_text": False,
            "body_small_text": False,
            "brand_small_text": False,
            "brand_colour": "navbar-success",
            "accent": "accent-teal",
            "navbar": "navbar-dark",
            "no_navbar_border": False,
            "navbar_fixed": False,
            "layout_boxed": False,
            "footer_fixed": False,
            "sidebar_fixed": False,
            "sidebar": "sidebar-dark-info",
            "sidebar_nav_small_text": False,
            "sidebar_disable_expand": False,
            "sidebar_nav_child_indent": False,
            "sidebar_nav_compact_style": False,
            "sidebar_nav_legacy_style": False,
            "sidebar_nav_flat_style": False,
            "theme": "cyborg",
            "dark_mode_theme": None,
            "button_classes": {
                "primary": "btn-primary",
                "secondary": "btn-secondary",
                "info": "btn-info",
                "warning": "btn-warning",
                "danger": "btn-danger",
                "success": "btn-success",
            },
        }
        ```
6. Django Suit
   - Looks like the last update was 3 years ago
   - Decided to ignore project testing
7. django-baton :star: 
   - Freeware
   - doc : [django-baton](https://django-baton.readthedocs.io/en/latest/)
   - github : [django-baton](https://github.com/otto-torino/django-baton)
   - reference :
     - [오픈소스를 활용한 어드민 스타일링(Theme)](https://velog.io/@ansalstmd/Django3-7.-%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4%EB%A5%BC-%ED%99%9C%EC%9A%A9%ED%95%9C-%EC%96%B4%EB%93%9C%EB%AF%BC-%EC%8A%A4%ED%83%80%EC%9D%BC%EB%A7%81-feat.%ED%8E%98%EC%8A%A4%ED%8A%B8%EC%BA%A0%ED%8D%BC%EC%8A%A4#05-title-%EB%B3%80%EA%B2%BDroot%ED%8F%B4%EB%8D%94%EC%9D%98-setting%EC%97%90%EC%84%9C-%EB%B3%80%EA%B2%BD)

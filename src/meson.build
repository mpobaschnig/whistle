whistle_sources = [
  'main.c',
  'whistle-application.c',
  'whistle-window.c',
]

whistle_deps = [
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.2'),
]

whistle_sources += gnome.compile_resources('whistle-resources',
  'whistle.gresource.xml',
  c_name: 'whistle'
)

executable('whistle', whistle_sources,
  dependencies: whistle_deps,
       install: true,
)

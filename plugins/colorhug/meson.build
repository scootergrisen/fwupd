cargs = ['-DG_LOG_DOMAIN="FuPluginColorHug"']

install_data([
  'colorhug.quirk',
  ],
  install_dir: join_paths(datadir, 'fwupd', 'quirks.d')
)

shared_module('fu_plugin_colorhug',
  fu_hash,
  sources : [
    'fu-colorhug-common.c',
    'fu-colorhug-device.c',
    'fu-plugin-colorhug.c',
  ],
  include_directories : [
    include_directories('../..'),
    include_directories('../../src'),
    include_directories('../../libfwupd'),
  ],
  install : true,
  install_dir: plugin_dir,
  link_with : [
    libfwupdprivate,
  ],
  c_args : cargs,
  dependencies : [
    plugin_deps,
  ],
)

application_id = 'io.github.drvonmiau.Museic'

# App icon (512x512): the muse logo tile, cut out with transparent rounded
# corners. Masters live in design/icon/ (icon-master-tile.png is the
# uncut original).
png_dir = 'hicolor' / '512x512' / 'apps'
install_data(
  png_dir / ('@0@.png').format(application_id),
  install_dir: get_option('datadir') / 'icons' / png_dir
)

symbolic_dir = 'hicolor' / 'symbolic' / 'apps'
install_data(
  symbolic_dir / ('@0@-symbolic.svg').format(application_id),
  install_dir: get_option('datadir') / 'icons' / symbolic_dir
)

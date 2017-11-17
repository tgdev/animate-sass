# CHANGELOG

All notable changes, updates, approved pull requests, etc will be noted here.

### v0.8.2
- Added CHANGELOG to better document changes
- Bumped version to account for recent updates since last version.
- PR #23 @cfv1000 Added bulk management for animation groups
- PR #26 @dennis-f Added `package.json`
- PR #32 @blowsie Updated README formatting
- PR #33 @lougreenwood Added calc() for `$base-duration` multipliers

### v0.6.5
- Removed old vendor prefixes (-moz, -o) from all animations and mixin helper.

### v0.6.4
- Adding missing slide enter/exit animation modules.

### v0.6.3
- Removed Sass deprecation warnings about unquote().
- PR #17 @jmcnevin

### v0.6.2
- Fixed mixin issue with Firefox and IE adding quotes to the animation-name property.

### v0.6.1
- PR #11 @mcnasby fixed issue with animate filename.

### v0.6.0
- PR #9 @benhodgson87 Added new `Zoom` animations and made mixins DRYer.
- Updating bower version.

### v0.5.0
- PR #8 @oller fixed issue with Libsass library and `fadeInDownBig`

### v0.4.0
- PR #7 @lencioni Fixed issues with 3rd party framework Bourbon.
- Added override option of all variables.
- Made sass file a partial to be imported into projects stylesheet without generating a standalone css file.
- Removed base helper partial in favour of copying the css into projects sass stylesheet.

### v0.3.0
- Added bower support.

### v0.2.0
- Removed css source files.
- Restructured repo for better compatibility with user projects.

### v0.1.0
- Initial port of animate.css to Sass.

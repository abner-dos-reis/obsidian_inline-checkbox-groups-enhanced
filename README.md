# Inline Checkbox Groups - Enhanced Version

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Note:** This is an enhanced adaptation of the original [Inline-Checkbox-Groups](https://github.com/bwya77/Inline-Checkbox-Groups) plugin by [Bradley Wyatt](https://github.com/bwya77). All credit for the original concept and implementation goes to the original author.

## Overview

This Obsidian plugin allows you to create multiple checkboxes on a single line with enhanced functionality. The main improvement in this adaptation is that you can now create multiple checkboxes **without requiring a separator character** like `|`.

## Features

### ✨ **New in this adaptation:**
- **No separator required**: Create multiple checkboxes simply by writing them sequentially
- **Reduced spacing**: Checkboxes are positioned closer together for a cleaner look
- **Improved parsing**: Enhanced regex-based detection of multiple checkboxes

### 🔧 **Original features maintained:**
- Create multiple checkboxes on a single line
- Automatic cross-out when all checkboxes are checked
- Customizable separator character (backward compatibility)
- Live preview and edit mode support

## Usage

### Simple Multiple Checkboxes (New!)
You can now create multiple checkboxes without any separator:

```markdown
[ ] Task 1 [x] Task 2 [ ] Task 3
```
Or just:

```markdown
[ ] [x] [ ] 
```
```markdown
NameHere [ ] [x] [ ] 
```

This will render as three individual checkboxes on the same line with minimal spacing.

### Traditional Separator Method (Still Supported)
The original separator-based method still works:

```markdown
[ ] Task 1 | [x] Task 2 | [ ] Task 3
```

### Cross-out Feature
When all checkboxes in a line are checked, the entire line will be crossed out (if enabled in settings):

```markdown
[x] Completed Task 1 [x] Completed Task 2 [x] Completed Task 3
```

## Installation

### Manual Installation
1. Download the latest release files
2. Copy `main.js`, `manifest.json`, and `styles.css` to your vault's plugins folder:
   ```
   VaultFolder/.obsidian/plugins/inline-checkbox-groups/
   ```
3. Reload Obsidian
4. Enable the plugin in Settings → Community Plugins

### From Community Plugins
*Note: This enhanced version is not yet available in the official community plugins repository*

## Settings

Access the plugin settings in **Settings → Community Plugins → Inline Checkbox Groups**:

- **Separator**: Character used to separate checkboxes (default: `|`)
- **Cross out completed items**: Toggle automatic strikethrough when all checkboxes are checked

## Examples

### Before (Original Plugin)
Required separator for multiple checkboxes:
```markdown
[ ] Buy groceries | [x] Walk the dog | [ ] Read book
```

### After (Enhanced Version)
No separator needed:
```markdown
[ ] Buy groceries [x] Walk the dog [ ] Read book
```

Both methods work, but the new approach is more natural and requires less typing.

## Technical Changes

This adaptation includes the following improvements:

1. **Enhanced Parsing Logic**: 
   - Uses regex-based detection to identify multiple checkboxes
   - Maintains backward compatibility with separator-based syntax

2. **Improved Spacing**:
   - Reduced gap between checkboxes from 4px to 1px
   - Reduced margins for a more compact appearance

3. **Robust Item Reconstruction**:
   - Better handling of checkbox states and content
   - Preserved original text formatting

## Contributing

Feel free to submit issues, feature requests, or pull requests to improve this enhanced version.

## Credits

- **Original Plugin**: [Inline-Checkbox-Groups](https://github.com/bwya77/Inline-Checkbox-Groups) by [Bradley Wyatt](https://github.com/bwya77)
- **Enhanced Version**: Adapted with improved functionality and user experience

## License

This project maintains the same license as the original project.

## Support

If you find this enhanced version useful, please consider:
- ⭐ Starring this repository
- 🐛 Reporting issues or suggesting improvements
- 💕 Supporting the original author: [Bradley Wyatt](https://github.com/bwya77)

---

**Disclaimer**: This is an independent adaptation. For the official version and support, please refer to the [original repository](https://github.com/bwya77/Inline-Checkbox-Groups).

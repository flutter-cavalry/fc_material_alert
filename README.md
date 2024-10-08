**Deprecated**: Moved to [fc_quick_dialog](https://github.com/flutter-cavalry/fc_quick_dialog).

# fc_material_alert

[![pub package](https://img.shields.io/pub/v/fc_material_alert.svg)](https://pub.dev/packages/fc_material_alert)

A simple wrapper around Flutter Material Design alert dialogs.

## Usage

```dart
// Confirm dialog.
final result = await FcMaterialAlert.confirm(context,
    title: 'Confirm',
    yesText: 'Yes',
    noText: 'No',
    cancelText: 'Cancel',
    content: 'Are you sure?');

// Standard dialog.
await FcMaterialAlert.standard(context,
    title: 'Info',
    okText: 'OK',
    content: 'You selected $result');

// Error dialog.
await FcMaterialAlert.error(
    context, 'Exception: Test plugin error',
    title: 'Error', okText: 'OK');
```

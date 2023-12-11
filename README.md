# fc_material_alert

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

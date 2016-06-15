# Code Peek

This package allows you to quickly peek and edit functions contained in other
files instead of having to open the file separately. This was inspired by
[Brackets](http://brackets.io/)'s quick edit feature and Maushundb's [Quick Editor](https://atom.io/packages/quick-editor) for CSS/LESS/SCSS.

![Code Peek Demo](https://github.com/DFreds/code-peek-atom/blob/master/code-peek.gif?raw=true)

# Supported files
Currently, supported files include:
* JavaScript
* TypeScript
* Java
* C#.
More will be coming soon.

# Installation
```
apm install code-peek
```
Or search for <code>code-peek</code> in the Atom settings view.

# Key Bindings
The default <code>cmd-alt-e</code> or <code>ctrl-alt-e</code>will toggle code-peek while the cursor is over a function of a supported type.

This can be edited by defining key bindings as shown below.

```coffee
'.platform-darwin atom-text-editor':
  'cmd-alt-e': 'code-peek:peekFunction'
  'shift-escape': 'code-peek:toggleCodePeekOff'

'.platform-linux atom-text-editor, .platform-win32 atom-text-editor':
  'ctrl-alt-e': 'code-peek:peekFunction'
  'shift-escape': 'code-peek:toggleCodePeekOff'

```

# Release Notes
## 1.0.0
* Support for JavaScript, TypeScript, Java, and C#

### Full change log [here](./CHANGELOG.md).

# Coming Soon
* Multiple files with same function definition
* Additional language support

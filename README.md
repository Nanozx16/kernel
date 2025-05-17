# kernel

## Usage

For detailed information on how to use the OCAP Kernel, please refer to the [OCAP Kernel Usage Guide](docs/usage.md) which provides comprehensive documentation on setting up, configuring, and using the kernel in both browser and Node.js environments.

### Kernel Control Panel

You can launch a browser-based Kernel Control Panel to interact with and manage vats:

1. Navigate to the extension package:

```bash
cd packages/extension
```

2. Start the development server:

```bash
yarn start
```

3. This will:
   - Launch a development server serving the extension
   - Set up a default cluster configuration
   - Serve sample vat bundles
   - Provide a UI for managing and interacting with the kernel and vats

The control panel allows you to:

- Launch vats
- View vat status
- Test kernel functionality
- Send messages to objects in vats
- **Inspect the database**: The control panel includes a built-in SQLite database inspector powered by SQLite WASM, allowing you to directly view and query the kernel's database through the browser interface. This is especially valuable since the kernel uses SQLite for persistence and would otherwise be difficult to inspect.

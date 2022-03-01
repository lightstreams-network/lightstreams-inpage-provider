# Lightstreams Wallet In-Page Provider

Used to initialize the inpage Lightstreams provider injected by Lightstreams Wallet.

## Usage

```javascript
// Create a stream to a remote provider:
const stream = new LocalMessageDuplexStream({
  name: 'lightstreams-inpage',
  target: 'lightstreams-contentscript',
})

// compose the inpage provider
const inpageProvider = new MetaMaskInpageProvider(stream, {jsonRpcStreamName: 'lightstreams-provider'})
```

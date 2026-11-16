<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-voyage 1.2.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-voyage.git", from: "1.2.0")
```

Products: `SwiftAIVoyage`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Voyage AI for Swift

`SwiftAIVoyage` adds Voyage AI to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/voyage` and supports embeddings and reranking.

Provider guide with models, options, streaming and errors:

- [Voyage AI](https://swiftaisdk.github.io/SwiftAISDK/providers/voyage/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIVoyage` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIVoyage

let provider = try AIProviders.voyage(configuration: VoyageProviderSettings())
```

By default the provider reads `VOYAGE_API_KEY` from the environment; values set in `VoyageProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-voyage` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.

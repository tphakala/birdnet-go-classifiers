# BirdNET-Go Classifiers

Custom TensorFlow Lite format AI model classifiers for enhanced bird and wildlife identification, designed for use with [BirdNET-Go](https://github.com/tphakala/birdnet-go) and BirdNET Analyzer.

## Overview

This repository contains specialized BirdNET classifier models that extend the capabilities of the base BirdNET v2.4 model. These classifiers focus on improving detection accuracy for specific species and adding support for new species not included in the original model.

## Current Model Version

**BirdNET-Go_classifier_20250907**

- Base Model: BirdNET v2.4
- Format: TensorFlow Lite (.tflite)
- Release Date: September 9, 2025

## Supported Species

### Augmented Classes
These species have enhanced detection capabilities compared to the base BirdNET model:

- **Certhia familiaris** - Eurasian Treecreeper
- **Corvus corax** - Common Raven
- **Cyanistes caeruleus** - Eurasian Blue Tit
- **Dendrocopos major** - Great Spotted Woodpecker
- **Dog** - Dog
- **Engine** - Engine
- **Garrulus glandarius** - Eurasian Jay
- **Glaucidium passerinum** - Eurasian Pygmy Owl
- **Human vocal** - Human vocal sounds
- **Loxia curvirostra** - Common Crossbill
- **Parus major** - Great Tit
- **Picus Canus** - Grey-headed Woodpecker
- **Pyrrhula pyrrhula** - Eurasian Bullfinch
- **Siren** - Siren (added to improve siren detection and reduce false matches with Eastern Screech-Owl)
- **Tetrastes bonasia** - Hazel Grouse

### New Species
Species added to extend the base model's capabilities:

- **Ovis aries** - Sheep
- **Vulpes vulpes** - Red Fox

## Installation & Usage

### With BirdNET-Go
1. Download the latest classifier model from the releases section
2. Place the `.tflite` file in your BirdNET-Go models directory (birdnet-go-app/data/models/)
3. Place the `*_Labels.txt` next to `.tflite` file in models directory
4. Configure BirdNET-Go to use the custom classifier in config.yaml
     - Set modelpath to "models/BirdNET-Go_classifier_20250907.tflite"
     - Set labelpath to "models/BirdNET-Go_classifier_20250907_Labels.txt"
     - Restart BirdNET-Go
5. Refer to the [BirdNET-Go documentation](https://github.com/tphakala/birdnet-go) for detailed setup instructions

## Changelog

### 20250909
- Updated augmented species list to 15 species total
- Added new augmented species:
  - **Certhia familiaris** - Eurasian Treecreeper
  - **Corvus corax** - Common Raven
  - **Cyanistes caeruleus** - Eurasian Blue Tit
  - **Parus major** - Great Tit
- Added **Siren** class to improve siren detection and reduce false matches with Eastern Screech-Owl
- Enhanced detection for existing species:
  - **Dendrocopos major** - Great Spotted Woodpecker
  - **Dog** - Dog
  - **Engine** - Engine
  - **Garrulus glandarius** - Eurasian Jay
  - **Glaucidium passerinum** - Eurasian Pygmy Owl
  - **Human vocal** - Human vocal
  - **Loxia curvirostra** - Common Crossbill
  - **Ovis aries** - Sheep
  - **Picus Canus** - Grey-headed Woodpecker
  - **Pyrrhula pyrrhula** - Eurasian Bullfinch
  - **Tetrastes bonasia** - Hazel Grouse
  - **Vulpes vulpes** - Red Fox

### 20250825
- Initial release based on BirdNET v2.4
- Added augmented species list with 12 species:
  - **Dendrocopos major** - Great Spotted Woodpecker
  - **Dog** - Dog
  - **Engine** - Engine
  - **Garrulus glandarius** - Eurasian Jay
  - **Glaucidium passerinum** - Eurasian Pygmy Owl
  - **Human vocal** - Human vocal
  - **Loxia curvirostra** - Common Crossbill
  - **Ovis aries** - Sheep
  - **Picus Canus** - Grey-headed Woodpecker
  - **Pyrrhula pyrrhula** - Eurasian Bullfinch
  - **Tetrastes bonasia** - Hazel Grouse
  - **Vulpes vulpes** - Red Fox
- Optimized for BirdNET-Go and BirdNET Analyzer compatibility

## License

This project follows the same licensing terms as the base BirdNET model. Please refer to the BirdNET project for license details.

## Acknowledgments

- Built upon the excellent work of the [BirdNET](https://github.com/birdnet-team/BirdNET-Analyzer) project
- Designed for seamless integration with [BirdNET-Go](https://github.com/tphakala/birdnet-go)
- Community contributions and feedback
  - *Ovis aries* audio samples provided by Martin HinzundKunz @HinzundKunz

## Support

For issues and questions:
- BirdNET-Go specific: [BirdNET-Go Issues](https://github.com/tphakala/birdnet-go/issues)
- Model-specific issues: Use this repository's issue tracker
- General BirdNET questions: Refer to the main BirdNET project

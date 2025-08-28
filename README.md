# BirdNET-Go Classifiers

Custom TensorFlow Lite format AI model classifiers for enhanced bird and wildlife identification, designed for use with [BirdNET-Go](https://github.com/tphakala/birdnet-go) and BirdNET Analyzer.

## Overview

This repository contains specialized BirdNET classifier models that extend the capabilities of the base BirdNET v2.4 model. These classifiers focus on improving detection accuracy for specific species and adding support for new species not included in the original model.

## Current Model Version

**BirdNET-Go_classifier_28082025**

- Base Model: BirdNET v2.4
- Format: TensorFlow Lite (.tflite)
- Release Date: August 28, 2025

## Supported Species

### Augmented Classes
These species have enhanced detection capabilities compared to the base BirdNET model:

- **Certhia familiaris** - Eurasian Treecreeper
- **Dendrocopos major** - Great Spotted Woodpecker
- **Dog** - Dog
- **Garrulus glandarius** - Eurasian Jay
- **Glaucidium passerinum** - Eurasian Pygmy Owl
- **Human non-vocal** - Human non-vocal sounds
- **Human vocal** - Human vocal sounds
- **Loxia curvirostra** - Common Crossbill
- **Picus canus** - Grey-headed Woodpecker
- **Pyrrhula pyrrhula** - Eurasian Bullfinch
- **Tetrastes bonasia** - Hazel Grouse

### New Species
Species added to extend the base model's capabilities:

- **Ovis aries** - Sheep
- **Vulpes vulpes** - Red Fox

## Installation & Usage

### With BirdNET-Go
1. Download the latest classifier model from the releases section
2. Place the `.tflite` file in your BirdNET-Go models directory
3. Configure BirdNET-Go to use the custom classifier
4. Refer to the [BirdNET-Go documentation](https://github.com/tphakala/birdnet-go) for detailed setup instructions

### With BirdNET Analyzer
1. Download the classifier model
2. Load the custom model in BirdNET Analyzer
3. Configure the species list to include the supported species

## Model Performance

These custom classifiers have been trained and optimized for:
- Enhanced accuracy for the listed augmented species
- Reliable detection of new species not in the base model
- Compatibility with existing BirdNET workflows
- Efficient inference on edge devices

## Technical Specifications

- **Model Format**: TensorFlow Lite (.tflite)
- **Base Architecture**: BirdNET v2.4

## Contributing

We welcome contributions to improve model accuracy and add support for additional species. Please:

1. Open an issue to discuss proposed changes
2. Provide sample audio data for new species
3. Include validation results for model improvements
4. Follow the contribution guidelines

## Changelog

### v28082025
- Initial release based on BirdNET v2.4
- Added 11 augmented species with enhanced detection
- Added 2 new species: Sheep and Red Fox
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
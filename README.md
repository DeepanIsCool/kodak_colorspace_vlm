# Kodak Color Space VLM Project

This repository contains color space transformations of the Kodak image dataset and VLM (Vision Language Model) inference results.

## Project Overview

This project processes images from the Kodak dataset through various color space transformations and analyzes them using Vision Language Models. The repository is organized into two main directories:

1. **kodak_color_spaces**: Contains the original Kodak images and their color space transformations
2. **vlm_inferences_kodak**: Contains VLM model responses and analysis data for each transformed image

## Directory Structure

### 1. kodak_color_spaces/

Complete tree structure of the color space outputs:

```
kodak_color_spaces/
├── processing_summary.txt
├── color_space_output/
│   ├── kodim01/
│   │   ├── kodim01_original_rgb.png
│   │   ├── kodim01_grayscale.png
│   │   ├── kodim01_comprehensive_comparison.png
│   │   ├── kodim01_cmyk_cyan.png
│   │   ├── kodim01_cmyk_magenta.png
│   │   ├── kodim01_cmyk_yellow.png
│   │   ├── kodim01_cmyk_black.png
│   │   ├── kodim01_hsv_hue.png
│   │   ├── kodim01_hsv_hue_pure.png
│   │   ├── kodim01_hsv_hue_realistic.png
│   │   ├── kodim01_hsv_saturation.png
│   │   ├── kodim01_hsv_value.png
│   │   ├── kodim01_lab_lightness.png
│   │   ├── kodim01_lab_a_channel.png
│   │   ├── kodim01_lab_a_colored.png
│   │   ├── kodim01_lab_b_channel.png
│   │   └── kodim01_lab_b_colored.png
│   ├── kodim02/
│   │   └── [Same structure as kodim01]
│   ├── kodim03/
│   │   └── [Same structure as kodim01]
│   ├── kodim04/
│   │   └── [Same structure as kodim01]
│   ├── kodim05/
│   │   └── [Same structure as kodim01]
│   ├── kodim09/
│   │   └── [Same structure as kodim01]
│   ├── kodim10/
│   │   └── [Same structure as kodim01]
│   ├── kodim11/
│   │   └── [Same structure as kodim01]
│   ├── kodim15/
│   │   └── [Same structure as kodim01]
│   ├── kodim16/
│   │   └── [Same structure as kodim01]
│   ├── kodim17/
│   │   └── [Same structure as kodim01]
│   ├── kodim18/
│   │   └── [Same structure as kodim01]
│   ├── kodim19/
│   │   └── [Same structure as kodim01]
│   ├── kodim20/
│   │   └── [Same structure as kodim01]
│   ├── kodim21/
│   │   └── [Same structure as kodim01]
│   ├── kodim22/
│   │   └── [Same structure as kodim01]
│   ├── kodim23/
│   │   └── [Same structure as kodim01]
│   └── kodim24/
│       └── [Same structure as kodim01]
└── downloaded_images/
    └── kodakimagecollection-master/
        ├── kodim01.png
        ├── kodim02.png
        ├── kodim03.png
        ├── kodim04.png
        ├── kodim05.png
        ├── kodim09.png
        ├── kodim10.png
        ├── kodim11.png
        ├── kodim15.png
        ├── kodim16.png
        ├── kodim17.png
        ├── kodim18.png
        ├── kodim19.png
        ├── kodim20.png
        ├── kodim21.png
        ├── kodim22.png
        ├── kodim23.png
        ├── kodim24.png
        └── README.md
```

**Color Space Transformations:**

Each Kodak image (kodim01-kodim24) is processed into 17 different color space representations:

- **Original**: `*_original_rgb.png` - Original RGB image
- **Grayscale**: `*_grayscale.png` - Grayscale conversion
- **CMYK (4 channels)**:
  - `*_cmyk_cyan.png`
  - `*_cmyk_magenta.png`
  - `*_cmyk_yellow.png`
  - `*_cmyk_black.png`
- **HSV (5 variations)**:
  - `*_hsv_hue.png` - Hue channel
  - `*_hsv_hue_pure.png` - Pure hue visualization
  - `*_hsv_hue_realistic.png` - Realistic hue visualization
  - `*_hsv_saturation.png` - Saturation channel
  - `*_hsv_value.png` - Value/Brightness channel
- **LAB (5 variations)**:
  - `*_lab_lightness.png` - Lightness channel
  - `*_lab_a_channel.png` - A channel (green-red)
  - `*_lab_a_colored.png` - Colored A channel visualization
  - `*_lab_b_channel.png` - B channel (blue-yellow)
  - `*_lab_b_colored.png` - Colored B channel visualization
- **Comparison**: `*_comprehensive_comparison.png` - Side-by-side comparison of all transformations

### 2. vlm_inferences_kodak/

Complete tree structure of the VLM inference results:

```
vlm_inferences_kodak/
├── tree.txt
├── kodim01/
│   ├── kodim01_original_rgb/
│   │   ├── kodim01_original_rgb.png
│   │   ├── analysis_data.json
│   │   ├── gemini_flash_latest_responses.txt
│   │   ├── llama4_scout_responses.txt
│   │   └── llama4_maverick_responses.txt
│   ├── kodim01_grayscale/
│   │   └── [Same file structure]
│   ├── kodim01_cmyk_cyan/
│   │   └── [Same file structure]
│   ├── kodim01_cmyk_magenta/
│   │   └── [Same file structure]
│   ├── kodim01_cmyk_yellow/
│   │   └── [Same file structure]
│   ├── kodim01_cmyk_black/
│   │   └── [Same file structure]
│   ├── kodim01_hsv_hue/
│   │   └── [Same file structure]
│   ├── kodim01_hsv_hue_pure/
│   │   └── [Same file structure]
│   ├── kodim01_hsv_hue_realistic/
│   │   └── [Same file structure]
│   ├── kodim01_hsv_saturation/
│   │   └── [Same file structure]
│   ├── kodim01_hsv_value/
│   │   └── [Same file structure]
│   ├── kodim01_lab_lightness/
│   │   └── [Same file structure]
│   ├── kodim01_lab_a_channel/
│   │   └── [Same file structure]
│   ├── kodim01_lab_a_colored/
│   │   └── [Same file structure]
│   ├── kodim01_lab_b_channel/
│   │   └── [Same file structure]
│   └── kodim01_lab_b_colored/
│       └── [Same file structure]
├── kodim02/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim03/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim04/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim05/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim09/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim10/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim11/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim15/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim16/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim17/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim18/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim19/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim20/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim21/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim22/
│   └── [Same structure as kodim01 with 16 subdirectories]
├── kodim23/
│   └── [Same structure as kodim01 with 16 subdirectories]
└── kodim24/
    └── [Same structure as kodim01 with 16 subdirectories]
```

**VLM Analysis Files:**

Each color space variant contains:

- `*.png` - The transformed image
- `analysis_data.json` - Structured analysis data
- `gemini_flash_latest_responses.txt` - Google Gemini Flash model responses
- `llama4_scout_responses.txt` - Llama 4 Scout model responses
- `llama4_maverick_responses.txt` - Llama 4 Maverick model responses

## Statistics

- **Total Images**: 18 Kodak images (kodim01-05, 09-11, 15-24)
- **Color Space Variants per Image**: 16 transformations (plus 1 original)
- **Total Color Space Images**: 306 (18 images × 17 variants)
- **VLM Models Used**: 3 (Gemini Flash Latest, Llama 4 Scout, Llama 4 Maverick)
- **Total VLM Analyses**: 918 (306 images × 3 models)

## File Organization

### kodak_color_spaces/

- Original images are stored in `downloaded_images/kodakimagecollection-master/`
- Processed color space transformations are in `color_space_output/[image_name]/`
- Processing summary available in `processing_summary.txt`

### vlm_inferences_kodak/

- Organized by image name first, then by color space transformation
- Each transformation has its own subdirectory containing:
  - The transformed image
  - Analysis data in JSON format
  - Text responses from three different VLM models

## Usage

This dataset can be used for:

- Studying color space transformations
- Analyzing VLM performance on different color space representations
- Comparing how different VLMs interpret color-transformed images
- Research on color perception in vision-language models
- Benchmarking VLM capabilities across color spaces

## Color Space Information

### CMYK

Cyan, Magenta, Yellow, and Key (Black) - A subtractive color model used in color printing.

### HSV

Hue, Saturation, Value - A cylindrical color model that represents colors in terms of their hue (color type), saturation (color intensity), and value (brightness).

### LAB

A color space that is designed to approximate human vision, consisting of:

- L: Lightness (0-100)
- A: Green-Red axis
- B: Blue-Yellow axis

---

_Generated: October 26, 2025_

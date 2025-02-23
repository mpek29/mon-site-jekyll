---
layout: page
title: BichonImageSynthesizer
description: 🖼️ Image synthesis using bichons
full_name: mpek29/BichonImageSynthesizer
img: assets/img/projects/BichonImageSynthesizer/main.png
importance: 1
git: https://github.com/mpek29/BichonImageSynthesizer
category: Electronics
subcategory: Signal and Image Processing
---


**BichonImageSynthesizer** is an open-source project that leverages a database of dog and cat photos ("bichon" database) to generate a synthetic image from a selected original image. The project applies mathematical techniques to express the original image in an orthonormal Euclidean space based on the bichon dataset.

## 🎯 Purpose

- 🖼️ **Image Synthesis**: Reconstruct an image using a weighted combination of bichon images.
- 📊 **Mathematical Projection**: Represent images in an orthonormal Euclidean space to facilitate synthesis.
- 🧮 **Scalar Product Utilization**: Use inner product calculations to project the target image onto the bichon basis.

## 📝 Features

| 🏷️ Feature         | 🔍 Description |
|----------------|-------------|
| 📷 **Bichon Database** | A collection of dog and cat images used as the basis |
| 🔢 **Euclidean Projection** | Express the original image in an orthonormal basis |
| 🎨 **Image Synthesis** | Approximate the original image using a linear combination of bichons |
| 🧮 **Mathematical Model** | Utilizes scalar product operations for optimal projection |
| 📉 **Dimensional Reduction** | Enhances efficiency by limiting synthesis to a subset of basis images |
| 🖥️ **Open-Source** | Fully customizable and modifiable |

## 📐 Image Processing Approach

| 🎭 Orthonormal Basis | 🧮 Scalar Product Projection | 🖼️ Synthetic Image |
|-----------|-----------|-----------|
| {% include image.html path="assets/img/projects/BichonImageSynthesizer/basis.png" width="300" %} | {% include image.html path="assets/img/projects/BichonImageSynthesizer/projection.png" width="300" %} | {% include image.html path="assets/img/projects/BichonImageSynthesizer/synthetic_image.png" width="300" %} |


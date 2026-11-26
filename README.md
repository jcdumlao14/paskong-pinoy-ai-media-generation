# Paskong Pinoy: A Visual Celebration of Christmas in the Philippines

# Paskong Pinoy — AI Media Generation

<p align="center">
  <img src="assets/paskong-pinoy-cover.png" alt="Paskong Pinoy AI Media Generation Cover" width="100%">
</p>

<p align="center">
  <strong>A visual celebration of Christmas traditions in the Philippines, powered by Generative AI.</strong>
</p>

---

## Project Overview

Paskong Pinoy is an AI-powered media generation project that celebrates the warmth, cultural identity, and unique traditions of Christmas in the Philippines.

Using the Sana 1600M text-to-image model deployed on Nebius Serverless GPU infrastructure, this project generates a collection of ten images illustrating Filipino Christmas scenes, from traditional parols and Simbang Gabi to Noche Buena, Christmas caroling, and family celebrations.

The project demonstrates a practical generative AI workflow, including model deployment, serverless GPU inference, image generation, performance measurement, and GPU cost estimation.

## Creative Concept

The Philippines is known for its distinctive Christmas traditions and festive celebrations. This project translates those cultural experiences into AI-generated visual assets.

The collection highlights:

- Traditional Filipino Christmas parols
- Paskong Barangay celebrations
- Simbang Gabi
- Noche Buena and Filipino Christmas delicacies
- The Giant Lantern Festival
- Family Christmas preparations
- Christmas caroling
- The joy of giving
- A Filipino Christmas night

## Generated Media Gallery

Ten AI-generated images celebrating Filipino Christmas traditions.

| Scene | Generated Image |
|---|---|
| The Filipino Parol | ![The Filipino Parol](runs/paskong-pinoy-20261126T043156Z/01-the-filipino-parol.png) |
| Paskong Barangay | ![Paskong Barangay](runs/paskong-pinoy-20261126T043156Z/02-paskong-barangay.png) |
| Simbang Gabi | ![Simbang Gabi](runs/paskong-pinoy-20261126T043156Z/03-simbang-gabi.png) |
| Noche Buena | ![Noche Buena](runs/paskong-pinoy-20261126T043156Z/04-noche-buena.png) |
| Filipino Christmas Delicacies | ![Filipino Christmas Delicacies](runs/paskong-pinoy-20261126T043156Z/05-filipino-christmas-delicacies.png) |
| Giant Lantern Festival | ![Giant Lantern Festival](runs/paskong-pinoy-20261126T043156Z/06-giant-lantern-festival.png) |
| Family Christmas Preparations | ![Family Christmas Preparations](runs/paskong-pinoy-20261126T043156Z/07-family-christmas-preparations.png) |
| Christmas Caroling | ![Christmas Caroling](runs/paskong-pinoy-20261126T043156Z/08-christmas-caroling.png) |
| The Joy of Giving | ![The Joy of Giving](runs/paskong-pinoy-20261126T043156Z/09-the-joy-of-giving.png) |
| A Filipino Christmas Night | ![A Filipino Christmas Night](runs/paskong-pinoy-20261126T043156Z/10-a-filipino-christmas-night.png) |

## Model and Infrastructure

| Component | Configuration |
|---|---|
| Model | `Efficient-Large-Model/Sana_1600M_1024px_diffusers` |
| Modality | Image generation |
| Deployment | Nebius Serverless GPU Endpoint |
| GPU | NVIDIA L40S |
| GPU Region | `eu-north1` |
| Generation batch | 10 images |

## Performance and Cost Analysis

The following measurements are based on the original ten-image generation batch.

| Metric | Result |
|---|---:|
| Successful generations | 10 / 10 |
| Failed generations | 0 |
| Median generation time | 8.226 seconds |
| GPU hourly rate used | $0.65/hour |
| Fixed run cost | $0.062978 |
| Marginal compute cost per image | $0.001485 |
| Projected compute cost per image at N = 1,000 | **$0.001548** |

The projected cost uses the fixed run cost amortized across 1,000 images, plus the estimated marginal compute cost per image.

These figures are compute estimates based on the GPU rate used in the analysis. Actual provider charges may vary depending on billing intervals and additional infrastructure costs.

## Project Structure

```text
paskong-pinoy-module1/
│
├── assets/
│   └── paskong-pinoy-cover.png
│
├── notebooks/
│   ├── generate_paskong_pinoy.ipynb
│   └── paskong_pinoy_gallery.ipynb
│
├── runs/
│   └── paskong-pinoy-20261126T043156Z/
│       ├── 01-the-filipino-parol.png
│       ├── 02-paskong-barangay.png
│       ├── 03-simbang-gabi.png
│       ├── 04-noche-buena.png
│       ├── 05-filipino-christmas-delicacies.png
│       ├── 06-giant-lantern-festival.png
│       ├── 07-family-christmas-preparations.png
│       ├── 08-christmas-caroling.png
│       ├── 09-the-joy-of-giving.png
│       ├── 10-a-filipino-christmas-night.png
│       └── metrics.json
│
├── prompts.json
├── .gitignore
└── README.md
```

## Notebooks

- **Image Generation Notebook:** `notebooks/generate_paskong_pinoy.ipynb` — contains the generation workflow and GPU inference process.
- **Gallery Notebook:** `notebooks/paskong_pinoy_gallery.ipynb` — presents the generated images, run information, and performance and cost analysis.

## Key Learnings

This project provided hands-on experience with:

- Deploying a text-to-image model on serverless GPU infrastructure.
- Running GPU-powered inference through an Endpoint.
- Generating and organizing multiple AI media assets.
- Measuring generation latency and execution performance.
- Estimating fixed and marginal GPU compute costs.
- Documenting and publishing a reproducible AI project using Jupyter Notebook and GitHub.

## Homework 1 — GPU Media Worker

This project was developed as part of Homework 1: GPU Media Worker.

**Question 1. What is the creative idea behind your asset? Why did you choose this topic?**

My creative idea is to create a collection of ten AI-generated images celebrating the Filipino Christmas season, featuring traditional parols, Simbang Gabi, Noche Buena, barangay celebrations, Christmas caroling, and Filipino family traditions. I chose this topic to showcase the warmth, cultural identity, and unique traditions of Christmas in the Philippines through generative AI.

**Question 2. Which model did you use?**

`Efficient-Large-Model/Sana_1600M_1024px_diffusers`

**Question 3. Which modality?**

Image

**Question 4. How did you run it?**

Endpoint (Nebius Serverless GPU)

**Question 5. Which GPU did you run on?**

NVIDIA L40S (L40S)

**Question 6. What was your median generation time per media asset, in seconds?**

8.226 seconds

**Question 7. What is your projected cost per asset at N = 1000, in USD?**

$0.001548 USD per asset.

## Project Context and Acknowledgment

This project was developed as part of the **Production AI Agents for Media Generation** course by [DataTalks.Club](https://datatalks.club/).

It demonstrates practical experience with serverless GPU infrastructure, generative media workflows, model inference, performance measurement, and GPU cost estimation.

---

**Created by Jocelyn C. Dumlao**

[GitHub Profile](https://github.com/jcdumlao14) · [Project Repository](https://github.com/jcdumlao14/paskong-pinoy-ai-media-generation)
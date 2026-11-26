# Paskong Pinoy: A Visual Celebration of Christmas in the Philippines

## Project overview

Paskong Pinoy is a generative media project celebrating the visual traditions,
culture, food, family, and community spirit of Christmas in the Philippines.

The project generates a collection of ten culturally inspired images using
the Sana 1600M model through a Nebius Serverless GPU Endpoint.

## Model

- Model: Efficient-Large-Model/Sana_1600M_1024px_diffusers
- GPU: NVIDIA L40S (subject to endpoint configuration)
- Output format: PNG
- Image count: 10

## Image collection

1. The Filipino Parol
2. Paskong Barangay
3. Simbang Gabi
4. Noche Buena
5. Filipino Christmas Delicacies
6. Giant Lantern Festival
7. Family Christmas Preparations
8. Christmas Caroling
9. The Joy of Giving
10. A Filipino Christmas Night

## Visual direction

Cinematic digital illustration, detailed realistic elements, warm golden
lighting, rich festive colors, tropical Philippine surroundings, balanced
composition, and professional editorial quality.

## Experiment objectives

- Measure endpoint startup time.
- Measure model readiness/load time.
- Record the generation latency of each of the ten images.
- Calculate fixed and marginal GPU costs using the actual endpoint rate.
- Estimate projected cost per image for a batch of 1,000 images.
- Evaluate image quality, cultural relevance, and visual consistency.

## Project structure

- `prompts.json`: the ten image prompts and shared visual style.
- `notebooks/`: the generation and measurement notebook.
- `runs/`: generated PNG files and experiment metrics.
- `assets/`: supporting project materials.

## Measurement integrity

All timing and cost figures will come from actual experiment measurements
and the actual GPU price shown by the provider.

The separately created project hero illustration is a visual reference,
not one of the ten Sana benchmark generations.

## Important

Endpoint credentials must remain private in a local `.env` file.
Never commit credentials, generated secrets, or private endpoint information.

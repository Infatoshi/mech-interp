# mech-interp

> the header of this repo "mech-interp", is short for mechanistic interpretability.

## What is Mechanistic interpretability? 

Well, before we dive into jupyter notebooks, its important to understand where this term originates. It essentially means "the inner working/mechanics" (mechanistic) and "how do we interpret something such that humans can understand it". We look inside the mechanics of neural networks to help understand which patterns correspond to features we might recognize in our own thinking/reasoning.

## Examples
To start, I've created two notebooks here. One is for visualizing the learned weights and activations from those weights. Seeing a heatmaps of the weights helps us understand which features of an input image should be active in order to propagate a signal to the end in order to score a high probabilty of the correct prediction. We can later train a sparse autoencoder to help us directly map sparse activation firings to patterns we recognize with our own eyes.

The second notebook `gpt2_attn.ipynb` is for visualizing the attention scores of gpt2 under different input prompts. We might notice different patterns in each attn head for each type of prompt (trianglar for coding VS rectangular for poems). Since there is much more we can visualize and attempt to interpret in GPTs, I leave the notebook open for experimentation. One cool option would be to train a SAE on the hidden MLP layer to extract "non-linear filters/projections" or signals which may not be obvious in the attn heads.

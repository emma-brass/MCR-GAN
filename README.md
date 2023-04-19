# MCR-GAN
Mapping of trust regions with a generative adversarial network resolves rotational ambiguity prevalent in multivariate curve resolution  

1. import spectral sequence  
2. obtain single solution for concentration and spectral matrices using pyMCR (available on GitHub)  
3. Add noise to single solution (20%) along a solution dimension axis (specified) - this will be the input dataset  
TRAINING  
4. apply constraints as needed (with loss functions) 
5. calculate reconstruction error (MSE(conc*spec, input))
6. backpropagate  
7. calculate adversarial loss (G + D): fit latent space to a gaussian distribution using z-score standardization  
8. backpropagate  
9. Map trust regions  
  trust regions mapped as standard deviations  
  

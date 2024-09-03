# Comparative Analysis of C-VAE and C-GAN for Japanese Character Generation

This project explores the use of Conditional Variational Autoencoders (C-VAE) and Conditional Generative Adversarial Networks (C-GAN) in the generation of Japanese character images. The focus of the project is to evaluate and compare the performance of these two deep learning models in terms of both visual quality and quantitative metrics. By incorporating conditional information such as character class and style, both models aim to generate realistic and stylistically accurate images.

# Key Highlights

1. **Model Architectures:** The C-VAE model includes an encoder-decoder structure that encodes input images along with their corresponding class and style into a latent space, from which it reconstructs the image. The C-GAN model, on the other hand, utilizes a generator-discriminator setup where the generator produces images conditioned on class and style, and the discriminator evaluates the realism and correctness of these images.

2. **Training Process:** Both models were trained on the Kuzushiji-49 dataset, which contains images of Japanese characters. The training process for the C-VAE involved optimizing the model over 40 epochs using the Adam optimizer, focusing on minimizing reconstruction loss. Similarly, the C-GAN model was trained for 40 epochs, with both the generator and discriminator being updated iteratively to improve the quality of the generated images.

3. **Results and Comparison:** The analysis revealed that the C-VAE model outperformed the C-GAN in generating visually consistent and high-quality images. The C-VAE captured finer details, particularly in the "thick" and "thin" styles, resulting in lower mean squared error and more accurate reconstructions. However, both models demonstrated the ability to generate conditional outputs that align with the specified class and style, showcasing their utility in generative tasks.

## Conclusion

This project provides valuable insights into the strengths and weaknesses of C-VAE and C-GAN models in the context of character generation. The findings suggest that while both models are capable of generating conditional images, C-VAE offers better reconstruction quality, making it more suitable for tasks that require high fidelity. The dataset used in this project is publicly available and can be accessed here: https://github.com/rois-codh/kmnist (Deep Learning for Classical Japanese Literature. Tarin Clanuwat et al. Paper: https://arxiv.org/abs/1812.01718).

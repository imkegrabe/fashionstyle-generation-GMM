# Fashion Style Generation: Evolutionary Search with Gaussian Mixture Models in the Latent Space <br>
[Imke Grabe](mailto:imgr@itu.dk), [Jichen Zhu](mailto:jicz@itu.dk), [Manex Agirrezabal](mailto:manex.aguirrezabal@hum.ku.dk)

IT University of Copenhagen & University of Copenhagen, Copenhagen, Denmark

## Description

This repository contrains the code for the above mentioned paper. The project suggests to guide the generation of a P-GAN with a GMM via a genetic algorithm to generate images that correspond to fashion styles.

![teaser](https://github.com/imkegrabe/fashionstyle-generation-GMM/blob/main/images/ev-model.png)

## Requirements

Python 3.6.9 <br/> 
numpy <br/> 
matplotlib <br/> 
torch <br/> 
torchvision <br/> 
h5py <br/> 
sklearn <br/> 
pickle <br/> 
deap <br/> 
Pytorch GAN Zoo: https://github.com/facebookresearch/pytorch_GAN_zoo <br/> 
MMFashion: https://github.com/open-mmlab/mmfashion <br/> 
FashionGen dataset: https://fashion-gen.com/ <br/> 

## Dataset
Rostamzadeh, N., Hosseini, S., Boquet, T., Stokowiec, W., Zhang, Y., Jauvin, C., Pal, C.: Fashion-Gen: The Generative Fashion Dataset and Challenge. arXiv preprint arXiv:1806.08317 (2018)

## Bugs
If you get the bug "can't convert cuda:0 device type tensor to numpy. Use Tensor.cpu() to copy the tensor to host memory first.",
run the function "extract_embedding" once with line "print(img.is_cuda)" uncommented.

## Citation
--------
If you use our code for your research, please cite:
```bibtex
@inproceedings{grabe_fashion_2022,
	title = {Fashion {Style} {Generation}: {Evolutionary} {Search} with {Gaussian} {Mixture} {Models} in the {Latent} {Space}},
	booktitle = {International {Conference} on {Computational} {Intelligence} in {Music}, {Sound}, {Art} and {Design} : {EvoMUSART} 2022},
	author = {Grabe, Imke and Zhu, Jichen and Agirrezabal, Manex},
	year = {2022},
	pages = {16},
}
